---
slug: devtoolsguild-may-2026-update
title: Dev Tools Guild May 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild May 2026 update

_**TL;DR**: TheDAO Security Fund Ethereum security quadratic funding round results, Vyper 0.5.0 alpha prereleases, and pattern matching in Core Solidity._

<!-- truncate -->

## Dev Tools Guild members

* TheDAO Security Fund [Ethereum security quadratic funding round results](https://forum.giveth.io/t/ethereum-security-qf-round-results-april-23-may-14-2026/2201): 134 projects shared $315k from ~4k donors plus a 637 ETH matching pool.  Thanks to everyone who donated to [Vyper](https://qf.giveth.io/project/vyper?roundId=16) and [Sourcify](https://qf.giveth.io/project/sourcify?roundId=16).

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* [Pattern matching in Core Solidity](https://www.soliditylang.org/blog/2026/05/05/pattern-matching-in-core-solidity/): details of how algebraic data types and pattern matching work in Core Solidity, with code examples and a walkthrough of the internals.
* Jacob: [what's next for Solidity](https://www.youtube.com/watch?v=Z89lljEBZOE) ETHPrague presentation.
* growthepie: [Solidity versions by value secured](https://x.com/growthepie_eth/status/2052014166920028583).

#### [Vyper](https://vyperlang.org/)
* Vyper [v0.5.0a1](https://github.com/vyperlang/vyper/releases/tag/v0.5.0a1) - [v0.5.0a2](https://github.com/vyperlang/vyper/releases/tag/v0.5.0a2) (prereleases): adds abstract methods.
* banteg [vyupgrade](https://github.com/banteg/vyupgrade#readme): rewrites older Vyper contracts to modern Vyper and compiles the source & target versions and compares their ABI, method identifiers and storage layout.
* [Vyper-HOL](https://github.com/verifereum/vyper-hol#readme): machine-checked formal semantics for Vyper in HOL4.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v2.0.5](https://github.com/alloy-rs/alloy/releases/tag/v2.0.5).

#### [Web3j](https://docs.web3j.io/) (Java)
* Web3j [v5.0.3](https://github.com/LFDT-web3j/web3j/releases/tag/v5.0.3): ENS resolution routed through the Universal Resolver (ready for ENS v2).

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.48.6](https://github.com/wevm/viem/releases/tag/viem%402.48.6) - [v2.51.3](https://github.com/wevm/viem/releases/tag/viem%402.51.3).
* wagmi [v3.6.9](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.9) - [v3.6.16](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.16).

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* [ApeWorX Collective](https://paragraph.com/@apeworx/introducing-the-apeworx-collective) launched: nonprofit to maintain Python dev tooling, Ethereum Foundation Python packages including web3.py moved to the stewardship of the collective.  Ape (dev framework) and Silverback (bots) will continue to be actively maintained.
* Ape [v0.8.50](https://github.com/ApeWorX/ape/releases/tag/v0.8.50): adds Aragon proxy detection, better cache control for contract types and a Brownie to Ape migration guide.
* [ApeShift](https://github.com/vinod820/apeshift#readme): migrate projects from Brownie to Ape.

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.7.1](https://github.com/foundry-rs/foundry/releases/tag/v1.7.1).

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* [Clear Signing](https://x.com/SourcifyEth/status/2054233737840181291) working group includes Sourcify who are helping steward the libraries & dev tools around the registry and contributing Sourcify's open dataset of 28M+ verified contracts. 
  * [Clear Signing Playground](https://clear-signing.sourcify.dev/): decode transactions into human readable format using ERC-7730 and Sourcify clear signing library.
* [Migrate to the v2 API before July 7](https://x.com/SourcifyEth/status/2051982425169731932).
* Manuel Wedler: [open source & open data](https://www.youtube.com/watch?v=OFlBA826YXQ) ETHPrague presentation. 

## Ethereum Layer 1

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target mid 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* [Soldøgn interop](https://blog.ethereum.org/2026/05/02/soldogn-interop-recap): core protocol contributors met in Svalbard for a week focused on the Glamsterdam upgrade.  200M+ gas limit target post-Glamsterdam upgrade.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
  * Execution layer: no headliner selected.

### Ethereum Foundation (EF)

* Vitalik: [EF will be smaller and more opinionated](https://x.com/VitalikButerin/status/2058583593102844111).  Ethereum should be deeply impressive in CROPS (censorship resistant, open source, private and secure).
* [Protocol cluster update](https://blog.ethereum.org/2026/05/11/protocol-update-may-26): new coordinators Will Corcoran, Kev Wedderburn and Fredrik taking over from Barnabé Monnot, Tim Beiko and Alex Stokes.
* Devcon 8 [tickets](https://devcon.org/tickets/): student applications open now, general admission & community tickets open in June.  
* ethPandaOps [Fast Confirmation Rule simulator](https://ethpandaops.io/posts/fcr-simulator/): 12 months of mainnet data replayed through four implementations of the Fast Confirmation Rule.
* Ben Edgington: [upgrading finality](https://consensus.ethereum.foundation/blog/upgrading-finality-edition-1), plan to reduce time to finality from ~1000s to ~10s (100x).

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
