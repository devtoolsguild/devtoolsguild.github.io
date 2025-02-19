---
sidebar_position: 4
---

# Architecture

This section describes the Guild’s current smart contract architecture.

## Modules

The DevTools Guild plans to follow the precedent set by the [Protocol Guild](https://protocol-guild.readthedocs.io/en/latest/03-onchain-architecture.html) with respect to the smart contract infrastructure it utilizes.

Following are the two core contracts that DevTools Guild will utilize.

- **The Splits contract** is used for splitting fund distributions to multiple addresses.
- **The Vesting contract** is used to vest funds over a defined period of time before they can be released to the Splits contract.

### Vesting Contract

[Vesting Contract Repository](https://github.com/0xSplits/splits-vesting/tree/master)

Vesting contracts enable the gradual release of funds to a designated beneficiary over a predetermined period. Each Vesting contract can manage multiple, isolated streams of tokens, all sharing the same vesting period but capable of starting and releasing independently.

The process involves:

- **Funding the Vesting Contract**: ETH and ERC20 tokens are sent to the Vesting contract, where they are held until a vesting stream is initiated.

- **Starting a Vesting Stream**: A vesting stream for a specific token is initiated, beginning the linear vesting process over the set period. Multiple streams can operate simultaneously within the same contract.

- **Releasing Vested Funds**: At any time, anyone can release the vested portion of tokens to the beneficiary. This mechanism ensures that funds are distributed gradually, aligning with predefined vesting schedules.

#### How it works:
- Donated tokens will accrue in a per-asset queue until a vesting stream is started for that batch of tokens by triggering the `startStream` function.
    - This function is **permissionless**, meaning **any actor** can trigger it, regardless of whether they are a Guild member.
- Once the vesting stream is started, the tokens will vest **linearly over 12 months** (or any predefined period set during contract deployment).
- Anyone can **permissionlessly** trigger `releaseStream` to push vested tokens into the **SplitsV2** contract. *(Note: This must be done per vesting stream.)*


### SplitV2 Contract

[SplitV2 Contract Repository](https://github.com/0xSplits/splits-contracts-monorepo/tree/main/packages/splits-v2)

SplitV2 contracts allow you to distribute payments to multiple recipients. Each Split is a payable smart contract wallet with multiple recipients, each assigned a specific ownership percentage. When ETH or ERC20 tokens are sent to the Split, they are held in the contract’s balance until a distribution is initiated.

SplitV2 offers two types of splitters:

- **Pull Splits**: After distribution, funds are held in a central contract called the Warehouse. Recipients can withdraw their allocated funds from the Warehouse at their convenience. This method is efficient for managing distributions to a large number of recipients.

- **Push Splits**: Upon distribution, funds are sent directly to recipients. To manage gas costs, these transfers are hard gas-capped; if a transfer fails, the funds are deposited into the Warehouse for later withdrawal. This approach ensures immediate fund delivery when possible.

#### How it works:
- The `distribute` function allocates tokens in the Split contract to Guild members **according to their weights** (it does not move the funds into the member wallets).
- Once `distribute` has been triggered, members can call the `withdrawForMyself` function to deposit their allocated tokens into their wallets.

For the **DTG pilot**, we intend to use **Pull Splits**. This approach, currently used by Protocol Guild (PG), allows recipients to withdraw funds at their convenience after the `distribute` function has been called.

### Updating Guild Members and Their Weights

The **controller** of the SplitV2 contract has the permission to update guild members and their weights using the **Splits app**.

Adjusting the list of guild members is **independent** of other functions like `startVestingStream`, `releaseVestingStream`, or `distribute`. Guild members can be updated at any time; however, once the distribution of vested tokens begins, the funds will be **allocated according to the current guild members’ shares at the time of distribution**.

#### Prerequisites

Before updating weights or the member list, it is **recommended** to:

1. **Release any ongoing vesting streams** using the `releaseVestingStream` function.
2. **Distribute funds** via the **Splits app** to the existing member list.

This ensures that the **current members receive their rightful share of the funds**. Once the distribution is completed, the member list can be **safely updated**.

## Resources

- [Splits Documentation](https://docs.splits.org/)
- [Splits Contracts Repository](https://github.com/0xSplits/splits-contracts)
- [Protocol Guild Onchain Architecture](https://protocol-guild.readthedocs.io/en/latest/03-onchain-architecture.html)
- [Protocol Guild Pilot Smart Contract Architecture](https://protocol-guild.readthedocs.io/en/latest/07-resources.html#pilot-smart-contract-architecture)  
