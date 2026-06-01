---
slug: devtoolsguild-may-2026-update
title: Dev Tools Guild May 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild May 2026 update

_**TL;DR**: Vyper 0.5.0 first alphas, Foundry 1.7.1 and pattern matching in Core Solidity._

<!-- truncate -->

## Dev Tools Guild members

* TheDAO Security Fund [Ethereum security quadratic funding round results](https://forum.giveth.io/t/ethereum-security-qf-round-results-april-23-may-14-2026/2201) (April 23 - May 14): 134 projects shared $315k from ~4k donors plus a 637 ETH matching pool.  Thanks to everyone who donated to [Vyper](https://qf.giveth.io/project/vyper?roundId=16) and [Sourcify](https://qf.giveth.io/project/sourcify?roundId=16).

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* [Pattern matching in Core Solidity](https://www.soliditylang.org/blog/2026/05/05/pattern-matching-in-core-solidity/): algebraic data types and exhaustiveness-checked pattern matching to eliminate classes of bugs at compile time (part of the Road to Core Solidity series).

#### [Vyper](https://vyperlang.org/)
* Vyper [v0.5.0a1](https://github.com/vyperlang/vyper/releases/tag/v0.5.0a1) and [v0.5.0a2](https://github.com/vyperlang/vyper/releases/tag/v0.5.0a2) (prereleases): first 0.5.0 alphas.
  * Language: underscores in numeric literals, single-line multi-import syntax, multi-interface implementation, abstract methods and flag member access in pure functions.
  * Breaking: `isqrt` moved from builtin to stdlib math module, duplicate interface implementations forbidden, default parameter values deprecated for interfaces and Python 3.10 support dropped.
  * Venom IR optimizations: memory allocation, stack spilling, assert elimination, memcpy elision and tail-merge passes.
* [Vyper-HOL](https://github.com/verifereum/vyper-hol#readme): machine-checked formal semantics for Vyper in HOL4.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v2.0.5](https://github.com/alloy-rs/alloy/releases/tag/v2.0.5).

#### [Web3j](https://docs.web3j.io/) (Java)
* web3j [v5.0.3](https://github.com/LFDT-web3j/web3j/releases/tag/v5.0.3): ENS resolution routed through the Universal Resolver (ENSv2 readiness), ClassLoader leak fix in the async executor, async executor lifecycle improvements and Jackson `tools.jackson` imports.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.48.6](https://github.com/wevm/viem/releases/tag/viem%402.48.6) - [v2.51.3](https://github.com/wevm/viem/releases/tag/viem%402.51.3).
* wagmi [v3.6.9](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.9) - [v3.6.16](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.16).

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* [ApeWorX Collective](https://paragraph.com/@apeworx/introducing-the-apeworx-collective) launched: a new nonprofit to maintain Python development tooling, with the Ethereum Foundation's web3.py and related Python packages being transferred to the collective.  Ape (dev framework) and Silverback (bots) continue active maintenance.
* Ape [v0.8.50](https://github.com/ApeWorX/ape/releases/tag/v0.8.50): removes unnecessary Safe proxy calls, contract cache control (`replace=True` and `fetch_from_disk=True`), aragonapp proxy detection, interactive retry on account unlock and a Brownie-to-Ape migration guide.

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.7.1](https://github.com/foundry-rs/foundry/releases/tag/v1.7.1): correctness fixes for cheatcodes and EVM (reverter address in CREATE frames, payable mock call value transfers, fork state-snapshot lookups and `expectEmit` revert preservation), Tempo template network config and release pipeline hardening (cosign-signed archives and Docker images, SHA256 checksums, SBOMs and SLSA provenance).

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* [Clear Signing Playground](https://clear-signing.sourcify.dev/): interactive tool for developing ERC-7730 clear signing descriptors.
* [Hedera mainnet and testnet](https://hedera.com/blog/smart-contract-verification-sourcify-dev-now-supported/) now verifiable on the main Sourcify instance, no Hedera-specific config required.
* [Migrate to the v2 API before July 7](https://x.com/SourcifyEth/status/2051982425169731932): legacy v1 API brownouts begin, pushing remaining traffic onto v2.

## Ethereum Layer 1

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target mid 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* [Soldøgn interop](https://blog.ethereum.org/2026/05/02/soldogn-interop-recap): 100+ core developers in Longyearbyen, Svalbard stabilized multi-client ePBS with external builders, benchmarked BAL parallel execution and finalized EIP-8037 gas repricing with a fixed `cost_per_state_byte`.
* [Protocol cluster update](https://blog.ethereum.org/2026/05/11/protocol-update-may-26): multi-client Glamsterdam devnets operational, EIP-8037 repricing numbers delivered on bal-devnet-6 and a 200M gas limit floor set as a post-Glamsterdam target.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
  * Execution layer: no headliner selected.
* FOCIL prototypes functional and native account abstraction requirements being scoped.

### Ethereum Foundation (EF)

* [Protocol cluster update](https://blog.ethereum.org/2026/05/11/protocol-update-may-26): new coordinators Will Corcoran, Kev Wedderburn and Fredrik take over from Barnabé Monnot, Tim Beiko and Alex Stokes.
* Ethereum Protocol Fellowship: [cohort 7](https://blog.ethereum.org/2026/04/30/epf-7) applications closed May 13, with a town hall held May 6.
* Vitalik: the [Foundation will become smaller and more opinionated](https://x.com/VitalikButerin/status/2058583593102844111), positioned as one node among many, doubling down on censorship resistance, open source, privacy and security.
* Researchers Carl Beekhuizen and Julian Ma are leaving the Ethereum Foundation.

### Ecosystem

* Ben Edgington: [upgrading finality](https://consensus.ethereum.foundation/blog/upgrading-finality-edition-1), a plan to cut finality from ~1000s to ~10s (100x), a candidate for a post-Hegotá upgrade.
* Vitalik: [formal verification explainer](https://vitalik.eth.limo/general/2026/05/18/fv.html).
* [Devcon 8](https://devcon.org/supporters/): supporter and student applications open, early bird tickets live ($349, ETH only).
* [25 million blocks](https://etherscan.io/block/25000000) reached on mainnet.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
