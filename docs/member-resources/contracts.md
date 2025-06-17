---
sidebar_position: 1
---

# Contracts

The guild uses [Splits](https://splits.org/) contracts for vesting and distributing funds to members, based on [Protocol Guild architecture](https://protocol-guild.readthedocs.io/en/latest/03-onchain-architecture.html).

## Vesting contract

Guild donations are made to the [Vesting contract](https://app.splits.org/accounts/0xB2Eb328c26de2d0A7F68198AA7813B287B3D06b4/?chainId=1).  

[donate.devtoolsguild.eth](https://app.ens.domains/donate.devtoolsguild.eth) & [vesting.devtoolsguild.eth](https://app.ens.domains/vesting.devtoolsguild.eth) resolve to the vesting contract.

Vesting streams have a 365 day vesting period.  The sole beneficiary is the guild pass-through wallet.  

[Splits docs: [Vesting](https://docs.splits.org/core/vesting)]

The process involves:

- **Donations**: ETH and ERC20 token donations are sent to the Vesting contract, where they are held until a vesting stream is initiated.

- **Starting a Vesting Stream**: A vesting stream for a specific token is initiated, beginning the linear vesting process over the vesting period. Multiple streams can operate simultaneously.

- **Releasing Vested Funds**: At any time, anyone can release the vested portion of tokens to the beneficiary.

#### How it works:
- Donated tokens will accrue in a per-asset queue until a vesting stream is started for that batch of tokens by triggering the `startStream` function.
    - This function is **permissionless**, meaning **anyone** can trigger it, regardless of whether they are a guild member.
- Once the vesting stream is started, the tokens will vest **linearly over 365 days**.
- Anyone can **permissionlessly** trigger `releaseStream` to push vested tokens to the Pass-through wallet. *(Note: This must be done per vesting stream.)*


## Pass-through wallet
[Pass-through wallet](https://app.splits.org/accounts/0xeEFf417993EaD1a5e75B3Cd42F4EC0eCca9e9dE7/?chainId=1) [Splits app] passes tokens on to the split contract.

[passthrough.devtoolsguild.eth](https://app.ens.domains/passthrough.devtoolsguild.eth) resolves to the pass-through wallet.

The wallet owner is the guild multi-sig.  The owner can pause the pass through of tokens or change the pass-through recipient.

[Splits docs: [Pass-through wallet](https://docs.splits.org/core/pass-through)]

## Split contract 

[Split contract](https://app.splits.org/accounts/0xe5136d651274F49d4fc7a39F01fd5025c2ca9384/?chainId=1) [Splits app] distributes ETH & ERC20 tokens to guild members according to pre-set percentages.  Funds are held in the Split's balance until `distribute` is called.

[Splits docs: [SplitV2](https://docs.splits.org/core/split-v2)]

[split.devtoolsguild.eth](https://app.ens.domains/split.devtoolsguild.eth) resolves to the split contract.

### Updating members and percentage share

The members and percentage share can be updated by the guild multi-sig at any time.

#### Prerequisites

Before updating members or percentage share, it is **recommended** to:

1. **Release any ongoing vesting streams** using the `releaseVestingStream` function.
2. **Distribute funds** via the **Splits app** to the existing member list.

This ensures that the **current members receive their rightful share of the funds**. Once the distribution is completed, the member list can be **safely updated**.

## Multi-sig

[Multi-sig](https://etherscan.io/address/0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70) [Etherscan] is 4/6.  The mulit-sig is the owner of the pass-through wallet.

## ENS

[devtoolsguild.eth](https://app.ens.domains/devtoolsguild.eth) [ENS]

## Resources

- [Splits Documentation](https://docs.splits.org/)
- [Splits Contracts Repository](https://github.com/0xSplits/splits-contracts)
- [Protocol Guild Onchain Architecture](https://protocol-guild.readthedocs.io/en/latest/03-onchain-architecture.html)
- [Protocol Guild Pilot Smart Contract Architecture](https://protocol-guild.readthedocs.io/en/latest/07-resources.html#pilot-smart-contract-architecture)  
