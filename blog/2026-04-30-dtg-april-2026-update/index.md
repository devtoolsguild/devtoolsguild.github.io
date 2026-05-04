---
slug: devtoolsguild-april-2026-update
title: Dev Tools Guild April 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild April 2026 update

_**TL;DR**: Support Vyper & Sourcify in Ethereum security QF round, Solidity 0.8.35 and Foundry 1.7.0._

<!-- truncate -->

## Dev Tools Guild members

* TheDAO Security Fund [Ethereum security quadratic funding round](https://qf.giveth.io/qf/ethereum-security) is live on Giveth, with a 500 ETH matching pool.  Donate to [Vyper](https://qf.giveth.io/project/vyper?roundId=16) and [Sourcify](https://qf.giveth.io/project/sourcify?roundId=16).

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* Solidity [v0.8.35](https://www.soliditylang.org/blog/2026/04/29/solidity-0.8.35-release-announcement/): adds `erc7201` comptime builtin, `--experimental` flag to gate in-development features, experimental SSA CFG codegen and deprecation warnings for upcoming 0.9.0 keywords.
* [Solidity Developer Survey 2025 results](https://www.soliditylang.org/blog/2026/04/15/solidity-developer-survey-2025-results/): 
  * Pain points: stack-too-deep 47% , bytecode size limits 33% and debugging 33%.
  * Dev framework usage: Foundry 57% and Hardhat 33%.
  * Client library usage: ethers.js 70%, viem 39% and wagmi 33%.

#### [Vyper](https://vyperlang.org/)
* [Vyper Chinese community](https://x.com/vyper_cn/status/2044710249119285430) launched.
* Charles Cooper: [formal verification and the Holy Grail of software correctness](https://ethcc.io/archives/formal-verification-and-the-holy-grail-of-software-correctness) (EthCC presentation).

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v2.0.0](https://github.com/alloy-rs/alloy/releases/tag/v2.0.0) - [v2.0.4](https://github.com/alloy-rs/alloy/releases/tag/v2.0.4).

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.47.10](https://github.com/wevm/viem/releases/tag/viem%402.47.10) - [v2.48.4](https://github.com/wevm/viem/releases/tag/viem%402.48.4).
* wagmi [v3.6.1](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.1) - [v3.6.8](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.8).
* [wagmi-swift and viem-swift](https://x.com/backseats_eth/status/2046956704353468829) ported to Swift by Backseats.

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* Ape [v0.8.49](https://github.com/ApeWorX/ape/releases/tag/v0.8.49).

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.7.0](https://github.com/foundry-rs/foundry/releases/tag/v1.7.0): parallelized stateless fuzzing, invariant optimization mode, Osaka default EVM hardfork, improved browser wallet support and immutable versioning.
* Forge Standard Library [v1.16.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.16.0) - [v1.16.1](https://github.com/foundry-rs/forge-std/releases/tag/v1.16.1).

#### [Scaffold-ETH](https://scaffoldeth.io/)
* SpeedRun Ethereum [build prompts](https://speedrunethereum.com/build-prompts): project specs for AI agents to scaffold apps using Scaffold-ETH 2.
* Speedrun Ethereum: [Foundry support added](https://x.com/buidlguidl/status/2044836179540131942) for challenges 0 to 4

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Kaan Uzdogan: [how Sourcify is reshaping Ethereum contract security](https://www.youtube.com/watch?v=XZDInjWp0Fo) (ECH Institute podcast: ecosystem project demo).
* EVM now (block explorer) [using Sourcify dataset](https://x.com/evmnow/status/2042735005034778897) to show verified contract source code.

## Ethereum Layer 1

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target mid 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
  * Execution layer: no headliner selected.
* Non-headliner EIPs are being proposed for inclusion.

### Ethereum Foundation (EF)

* Ecosystem Support Program: 
  * [Glamsterdam grants round](https://esp.ethereum.foundation/applicants/wishlist/glamsterdam-round) includes dev tooling.
  * [Q1 allocation](https://blog.ethereum.org/2026/04/29/allocation-q1-26): 57 projects shared $9.9M.
* Ethereum Protocol Fellowship: 
  * [EPF cohort 7](https://blog.ethereum.org/2026/04/30/epf-7), apply by May 13. 
  * [EPF cohort 6 recap](https://ps.ethereum.foundation/blog/epf6-recap)
* EF protocol support: [Checkpoint #9](https://blog.ethereum.org/2026/04/10/checkpoint-9).
* [ETH Rangers Program recap](https://blog.ethereum.org/2026/04/16/eth-rangers-recap): 17 recipients, $5.8M recovered/frozen, 785+ vulnerabilities reported, 100 state-sponsored operatives identified, 14 bugs found across major execution clients.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
