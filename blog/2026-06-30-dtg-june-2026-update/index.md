---
slug: devtoolsguild-june-2026-update
title: Dev Tools Guild June 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild June 2026 update

_**TL;DR**: Argot Collective five year funding, Ethereum Foundation new structure, Ethlabs launched._

<!-- truncate -->

## Dev Tools Guild members
* Argot Collective and Ethereum Foundation [completed final phase of five year funding commitment](https://www.argot.org/blog/2026-06-30-ef-funding-final-part).   

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* [Argot Collective and Walnut implementing ethdebug](https://walnut.dev/blog/argot-announcement) inside Solidity compiler.
* [Solidity was part of Octant Epoch 12](https://epoch.octant.app/rounds/0xf9de7a09aebbbacba9a9f4a32874463b2ddc1b8e6b4f6b65014febacbfff13f5/project/1) (quadratic funding), 6.75 WETH raised from 48 backers.
* Jacob Czepluch: [A sneak peek at Core Solidity](https://www.youtube.com/watch?v=Z89lljEBZOE) Dappcon Berlin presentation.

#### [Vyper](https://vyperlang.org/)
* Vyper [v0.5.0a3](https://github.com/vyperlang/vyper/releases/tag/v0.5.0a3) (prerelease): adds custom errors.
* [vyupgrade stewarded by Vyper org](https://x.com/vyperlang/status/2071992809964311006) on GitHub, with banteg remaining as maintainer.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v2.1.0](https://github.com/alloy-rs/alloy/releases/tag/v2.1.0): adds provider watch blocks and SSZ encoding/decoding for payload envelopes.

#### [ethers.js](https://ethers.org/) (TypeScript)
* ethers.js [v6.17.0](https://github.com/ethers-io/ethers.js/releases/tag/v6.17.0): adds ENSv2 support & rate limiting for a provider.

#### [Web3j](https://docs.web3j.io/) (Java)
* Web3j [v6.0.0](https://github.com/LFDT-web3j/web3j/releases/tag/v6.0.0): adds EIP-7594 blob transaction support, EIP-7702 authorization signing & recovery, EIP-7918 blob base fee RPC and agent skills.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.52.0](https://github.com/wevm/viem/releases/tag/viem%402.52.0) - [v2.54.1](https://github.com/wevm/viem/releases/tag/viem%402.54.1).
* wagmi [v3.6.18](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.18) - [v3.6.21](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.21).

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* Ape [website and docs site](https://x.com/ApeFramework/status/2069557840209940711) revamped.

#### [Foundry](https://getfoundry.sh/)
* forge-std [v1.16.2](https://github.com/foundry-rs/forge-std/releases/tag/v1.16.2).

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Reminder: [Sourcify v1 API shuts down July 7](https://docs.sourcify.dev/blog/api-v1-brownouts/), migrate to v2 API.
* Kaan Uzdoğan [Goodbye YOLO Signing](https://www.youtube.com/watch?v=4DKnkMpJPmA) Dappcon Berlin presentation.

## Ethereum Layer 1

* [Strawmap](https://strawmap.org/) (strawman roadmap) updated.
* [Ethlabs launched](https://ethlabs.org/thesis.html): non-profit R&D lab for Ethereum and ETH, founded by Ansgar Dietrichs, Barnabé Monnot, Caspar Schwarz-Schilling, Josh Rudolf and Julian Ma.  Anchor funding by Bitmine, Sharplink & Joe Lubin.

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target H2 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* [glamsterdam-devnet-6](https://glamsterdam-devnet-6.ethpandaops.io/): launched with remaining EIPs (except [EIP-7688 forward compatible consensus data structures](https://forkcast.org/eips/7688/)).
* [EIP-8282 builder execution requests](https://forkcast.org/eips/8282/) system contracts will require external security review, estimated 1-2 months.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).

### Ethereum Foundation

* [EF new structure](https://blog.ethereum.org/2026/06/23/ef-structure): five domain clusters (protocol, access, user, community and institutional), plus clusters for operations and management.  EF parted ways with 54 colleagues (~20% of staff) and [~40% budget decrease](https://x.com/VitalikButerin/status/2069431500035023121).
* [Devcon 8 community hub applications](https://forum.devcon.org/t/rfp-13-devcon-8-india-community-hubs/8657) open, August 12 deadline
---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
