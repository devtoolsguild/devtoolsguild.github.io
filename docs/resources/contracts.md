---
sidebar_position: 1
---

# Contracts

## Overview

The guild uses [Splits](https://splits.org/) contracts for vesting and distributing funds to members, based on [Protocol Guild architecture](https://protocol-guild.readthedocs.io/en/latest/03-onchain-architecture.html).


| Contract Name       | Address (ENS)                              | App                                                                 | Docs                                              | Purpose                                                                 |
|---------------------|--------------------------------------------|--------------------------------------------------------------------------------|--------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| Vesting Contract    | [donate.devtoolsguild.eth](https://etherscan.io/address/donate.devtoolsguild.eth) & [vesting.devtoolsguild.eth](https://etherscan.io/address/vesting.devtoolsguild.eth) (mainnet) [0x81a72FCA7880bde5723c1d6229bDb9EB41C65155](https://arbiscan.io/address/0x81a72FCA7880bde5723c1d6229bDb9EB41C65155) (Arbitrum) [0x59441b123B7521a711A3D1491f55f9Bf54EB0751](https://basescan.org/address/0x59441b123B7521a711A3D1491f55f9Bf54EB0751) (Base) [0x2AE9883c593295A1D2aD8F0874fF741aA0244ABc](https://optimistic.etherscan.io/address/0x2AE9883c593295A1D2aD8F0874fF741aA0244ABc) (Optimism) | [mainnet](https://app.splits.org/accounts/0xB2Eb328c26de2d0A7F68198AA7813B287B3D06b4/?chainId=1) [Arbitrum](https://app.splits.org/accounts/0x81a72FCA7880bde5723c1d6229bDb9EB41C65155/?chainId=42161) [Base](https://app.splits.org/accounts/0x59441b123B7521a711A3D1491f55f9Bf54EB0751/?chainId=8453) [Optimism](https://app.splits.org/accounts/0x2AE9883c593295A1D2aD8F0874fF741aA0244ABc/?chainId=10) | [Vesting](https://docs.splits.org/core/vesting) (Splits) | Accepts ETH/ERC20 donations.  Vests linearly over 365 days to the pass-through wallet. |
| Pass-through Wallet | [passthrough.devtoolsguild.eth](https://etherscan.io/address/passthrough.devtoolsguild.eth) (mainnet) [0x0d59F510C0f9ba2FE4a76A90af857105aa9A57d7](https://arbiscan.io/address/0x0d59F510C0f9ba2FE4a76A90af857105aa9A57d7) (Arbitrum) [0x1a6590b1294059d589A3D3360eBE7303c108e705](https://basescan.org/address/0x1a6590b1294059d589A3D3360eBE7303c108e705) (Base) [0xc2728Bd177E6206030d2D4C376eA573efEc783e9](https://optimistic.etherscan.io/address/0xc2728Bd177E6206030d2D4C376eA573efEc783e9) (Optimism) | [mainnet](https://app.splits.org/accounts/0xeEFf417993EaD1a5e75B3Cd42F4EC0eCca9e9dE7/?chainId=1) [Arbitrum](https://app.splits.org/accounts/0x0d59F510C0f9ba2FE4a76A90af857105aa9A57d7/?chainId=42161) [Base](https://app.splits.org/accounts/0x1a6590b1294059d589A3D3360eBE7303c108e705/?chainId=8453) [Optimism](https://app.splits.org/accounts/0xc2728Bd177E6206030d2D4C376eA573efEc783e9/?chainId=10) | [Pass-through Wallet](https://docs.splits.org/core/pass-through) (Splits) | Passes tokens to the split contract. Guild multi-sig (owner) can pause or change recipient. |
| Split Contract      | [split.devtoolsguild.eth](https://etherscan.io/address/split.devtoolsguild.eth) (mainnet) [0x6f06ad3E6149A82d69f5a6d181659deBe7aB0A3a](https://arbiscan.io/address/0x6f06ad3E6149A82d69f5a6d181659deBe7aB0A3a) (Arbitrum) [0x5C888DBB40f1E5F712aE99dF44D232D89D33D319](https://basescan.org/address/0x5C888DBB40f1E5F712aE99dF44D232D89D33D319) (Base) [0x6f06ad3E6149A82d69f5a6d181659deBe7aB0A3a](https://optimistic.etherscan.io/address/0x6f06ad3E6149A82d69f5a6d181659deBe7aB0A3a) (Optimism) | [mainnet](https://app.splits.org/accounts/0xe5136d651274F49d4fc7a39F01fd5025c2ca9384/?chainId=1) [Arbitrum](https://app.splits.org/accounts/0x6f06ad3E6149A82d69f5a6d181659deBe7aB0A3a/?chainId=42161) [Base](https://app.splits.org/accounts/0x5C888DBB40f1E5F712aE99dF44D232D89D33D319/?chainId=8453) [Optimism](https://app.splits.org/accounts/0x6f06ad3E6149A82d69f5a6d181659deBe7aB0A3a/?chainId=10) | [SplitV2](https://docs.splits.org/core/split-v2) (Splits) | Distributes ETH/ERC20 to guild members per pre-set percentages. Guild multi-sig can update members and shares. |
| Multi-sig           | [devtoolsguild.eth](https://etherscan.io/address/devtoolsguild.eth) (mainnet) [0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70](https://arbiscan.io/address/0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70) (Arbitrum) [0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70](https://basescan.org/address/0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70) (Base) [0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70](https://optimistic.etherscan.io/address/0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70) (Optimism) | N/A                                                                            | N/A                                                          | 4/6 multi-sig.  Can pause or change recipient of pass-through wallet.  Can update split members & shares.  |

## Vesting contract

[Donations](../donate.md) to the guild can be made to the vesting contract at [donate.devtoolsguild.eth](https://etherscan.io/address/donate.devtoolsguild.eth) (mainnet).  

Vesting streams have a 365 day vesting period.  The sole beneficiary is the guild pass-through wallet.  

The process involves:

- **Donations**: ETH & ERC20 token donations are sent to the Vesting contract, where they are held until a vesting stream is initiated.

- **Starting a Vesting Stream**: A vesting stream for a specific token is initiated via the `startStream` function, beginning the linear vesting process over the 365 day vesting period. Anyone can trigger this.  Multiple streams can operate simultaneously.

- **Releasing Vested Funds**: At any time, anyone can release the vested portion of tokens to the pass through wallet via the `releaseStream` function.  *(Note: This must be done per vesting stream.)*

## Pass-through wallet
[Pass-through wallet](https://docs.splits.org/core/pass-through) passes tokens on to the split contract.

The guild multi-sig owns the wallet and can pause the pass through of tokens or change the pass-through recipient.

## Split contract 

[Split contract](https://docs.splits.org/core/split-v2) distributes ETH & ERC20 tokens to guild members according to pre-set percentages.  Funds are held in the Split's balance until `distribute` function is called.

### Updating members and percentage share

The members and percentage share can be updated by the guild multi-sig at any time.

#### Prerequisites

Before updating members or percentage share, it is **recommended** to:

1. **Release any ongoing vesting streams** using the `releaseVestingStream` function.
2. **Distribute funds** via the **Splits app** to the existing member list.

This ensures that the **current members receive their rightful share of the funds**. Once the distribution is completed, the member list can be **safely updated**.

## Multi-sig

[Multi-sig](https://etherscan.io/address/0x2cF5869Eac6D7809DcF867c0e5cae1E9c5648e70) (mainnet) is 4/6.  The multi-sig is the owner of the pass-through wallet.  
The multi-sig also owns the pass-through wallet and can pause the pass through of tokens or change the pass-through recipient.

## ENS

[devtoolsguild.eth](https://app.ens.domains/devtoolsguild.eth) [ENS] is owned by the guild multi-sig.

## Resources

- [Splits Documentation](https://docs.splits.org/)
- [Splits Contracts Repository](https://github.com/0xSplits/splits-contracts)
- [Protocol Guild Onchain Architecture](https://protocol-guild.readthedocs.io/en/latest/03-onchain-architecture.html)
- [Protocol Guild Pilot Smart Contract Architecture](https://protocol-guild.readthedocs.io/en/latest/07-resources.html#pilot-smart-contract-architecture)  
