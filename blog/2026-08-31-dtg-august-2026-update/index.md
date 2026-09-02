---
slug: devtoolsguild-august-2026-update
title: Dev Tools Guild August 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild August 2026 update

_**TL;DR**: Platåberget testnet available for Glamsterdam upgrade testing. Foundry v1.8.0 symbolic testing preview. Ox v1 stable._

<!-- truncate -->

## Dev Tools Guild members

* [arrayref](https://blog.rust-lang.org/2026/08/20/supply-chain-attack-on-arrayref/) (Rust crate) supply chain attack: [Paradigm's open source Rust repositories were not affected](https://x.com/gakonst/status/2090448987824541864), including alloy & Foundry.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v2.3.0](https://github.com/alloy-rs/alloy/releases/tag/v2.3.0) - [v2.4.1](https://github.com/alloy-rs/alloy/releases/tag/v2.4.1).

#### [Web3j](https://docs.web3j.io/) (Java)
* Web3j [granted EF Ecosystem Support Program funding](https://blog.ethereum.org/2026/08/18/allocation-q2-26) to keep the JVM client library in sync with the Glamsterdam upgrade, plus AI-targeted documentation.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.55.11](https://github.com/wevm/viem/releases/tag/viem%402.55.11) - [v2.56.1](https://github.com/wevm/viem/releases/tag/viem%402.56.1).
* wagmi [v3.7.6](https://github.com/wevm/wagmi/releases/tag/wagmi%403.7.6) - [v3.7.7](https://github.com/wevm/wagmi/releases/tag/wagmi%403.7.7).
* [Ox v1](https://x.com/wevm_dev/status/2088030714696761369) (EVM standard library) stable, powers viem & wagmi.

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* Ape [v0.8.51](https://github.com/ApeWorX/ape/releases/tag/v0.8.51).
* Ape Sourcify [v0.8.1](https://github.com/ApeWorX/ape-sourcify/releases/tag/v0.8.1) (plugin).

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.8.0](https://github.com/foundry-rs/foundry/releases/tag/v1.8.0): opt-in preview of native symbolic testing, mutation testing and assembly robustness testing.  Isolate mode and dynamic test linking now default, Forge embeds Solar language server, `forge lint` gains security & gas detectors (nearing Slither/Aderyn parity) and `foundryup` rewritten in Rust.
* Foundry [v1.8.1](https://github.com/foundry-rs/foundry/releases/tag/v1.8.1): fixes regressions and removes v1.8.0 project trust warnings.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Sourcify server [v4.0.0](https://github.com/argotorg/sourcify/releases/tag/sourcify-server%404.0.0): API v1 removed, auto-recovery for stuck v2 verification jobs, EIP-1167 clone detection with immutable args and similarity API fixes.
* Kaan Uzdoğan: [Introduction to ERC-7730](https://docs.sourcify.dev/blog/intro-to-erc7730/), clear signing.  Wallet developer input wanted.
* [Sourcify dataset used to analyse quick slots potential impact](https://x.com/SourcifyEth/status/2086740760008012030) ([EIP-8198 quick slots](https://forkcast.org/eips/8198)): 20.6k of 7.7M mainnet contracts (0.27%) found relevant.
* [L2BEAT verified ~1000 smart contracts](https://x.com/SourcifyEth/status/2093055768673001621) on Sourcify, adding contracts used in L2 projects and bridges.

## Ethereum Layer 1

* [Strawmap](https://strawmap.org/) (strawman roadmap) updated August 4, covering proposed upgrades through 2029.

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target H2 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* [18 EIPs](https://forkcast.org/upgrade/glamsterdam/#scheduled-for-inclusion) Scheduled for Inclusion (SFI).
* [Platåberget](https://blog.ethereum.org/en/2026/08/17/plataberget-testnet) (glamsterdam-devnet-8): public testnet launched.
* [Gas repricing impact](https://blog.ethereum.org/2026/08/24/glamsterdam-repricing-testing): [EIP-8037](https://forkcast.org/eips/8037) increases the cost of creating new state and [EIP-8038](https://forkcast.org/eips/8038) increases the cost of accessing state.  A small set of contracts may break or degrade without preventative updates.
  * Contract developers: check whether contracts are in the [affected mainnet contracts](https://ethereum.github.io/repricing-impact/affected-contracts.html), then test fixes on Platåberget testnet.
  * Wallet, RPC & node tooling developers: update gas estimation for the new schedule.  Any tool that relies on a hardcapped maximum gas limit will break and needs updating.
* [200M gas limit](https://forkcast.org/calls/acde/243/) planned for Glamsterdam.
* Public testnets: proposal to upgrade Sepolia September 28 & Hoodi October 26.  mainnet potentially early December, tight timeline depending on testing & security reviews.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target 2027)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
* [Native account abstraction](https://x.com/nixorokish/status/2093021853036228665) Scheduled for Inclusion (SFI).
* [61 EIPs](https://forkcast.org/upgrade/hegota/#proposed-for-inclusion) Proposed for Inclusion (PFI).

### Ethereum Foundation

* Ecosystem Support Program [Q2 allocation](https://blog.ethereum.org/2026/08/18/allocation-q2-26): 70 projects shared $5.5M, including Web3j.
* [better.codes](https://blog.ethereum.org/en/2026/08/20/better-codes-challenge): open autoresearch challenge from the EF Formal Verification team, with Yukon & zkSecurity, to raise machine-checked soundness bounds for hash-based SNARKs.
* [Trillion Dollar Security grant for WEBCAT](https://blog.ethereum.org/2026/08/05/1ts-grant): transparency & code signing for web applications.
* Devcon 8 (Mumbai, India, November 3-6):
  * [Student discounted ticket applications](https://x.com/EFDevcon/status/2088469227040624921) extended to September 30.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
