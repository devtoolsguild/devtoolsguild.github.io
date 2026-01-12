---
slug: devtoolsguild-november-update
title: Dev Tools Guild November update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild November update

_**TL;DR**: 60M gas limit, mainnet upgrades to Fusaka on December 3 and Optimism's Retro Funding continues to support member projects._

<!-- truncate -->

## Dev Tools Guild members

* Optimism's [Retro Funding: Dev Tooling](https://atlas.optimism.io/missions/retro-funding-dev-tooling) continues to support [Solidity](https://atlas.optimism.io/project/0xcc8d03e014e121d10602eeff729b755d5dc6a317df0d6302c8a9d3b5424aaba8), [Vyper](https://atlas.optimism.io/project/0x9ca1f7b0e0d10d3bd2619e51a54f2e4175e029c87a2944cf1ebc89164ba77ea0), [alloy](https://atlas.optimism.io/project/0x56ce7cbc27852a8d8ef5869dc9033a215c8893f799468f61527dacb9f92be790), [ethers.js](https://atlas.optimism.io/project/0xa3d07f453f70d844196d89d79848aa2e70a0bd8b38bf0f493cba1547bb3bca5e), [viem](https://atlas.optimism.io/project/0x6bd057da522918a4675396313ae33a2f2788a1ceeb3bd7ae228015e3eb317a7d), [web3.py](https://atlas.optimism.io/project/0xebe03c3d6d33cad60124b9b05ef6e2ff056293a1de3c5fa51dfbb90c86c14bf7), [Ape Framework](https://atlas.optimism.io/project/0xa0b16714baef75d97ec07fd48eaf42e79df92fe2a3c2d725d2388ede587ea54c), [Foundry](https://atlas.optimism.io/project/0x4562c0630907577f433cad78c7e2cc03349d918b6c14ef982f11a2678f5999ad), [Scaffold-ETH](https://atlas.optimism.io/project/0x154a42e5ca88d7c2732fda74d6eb611057fc88dbe6f0ff3aae7b89c2cd1666ab) and [Sourcify](https://atlas.optimism.io/project/0x51cda5996ef1a2ccd8fcf4ee5792337695599454c83eb1218c3ad4388dcb5bf5).
* [Gitcoin Grants 24](https://gov.gitcoin.co/t/gg24-oss-quadratic-funding-results/24782) results.  Thanks to everyone who donated to the Dev Tools Guild.
* [Deep funding round](https://x.com/dripsnetwork/status/1989354692586139993) hosted by Drips.

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/) 
* [Core Solidity deep dive](https://www.soliditylang.org/blog/2025/11/14/core-solidity-deep-dive/).  [Feedback](https://forum.soliditylang.org/t/call-for-feedback-core-solidity-deep-dive/3643) on the Solidity forum.
* Solidity is in [Octant Epoch 10](https://x.com/OctantApp/status/1993802455038218415) (top 25 projects from nine epochs), allocation is January 6-20, 2026.

#### [Vyper](https://vyperlang.org/)
* [Mastering Ethereum](https://masteringethereum.xyz/) second edition: [Vyper chapter](https://masteringethereum.xyz/chapter_8.html).

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v1.1.0](https://github.com/alloy-rs/alloy/releases/tag/v1.1.0) - [v1.1.2](https://github.com/alloy-rs/alloy/releases/tag/v1.1.2).

#### [viem](https://viem.sh/) (TypeScript)
* viem [2.39.0](https://github.com/wevm/viem/releases/tag/viem%402.39.0) - [2.40.3](https://github.com/wevm/viem/releases/tag/viem%402.40.3). 
* wagmi [3.0.0](https://github.com/wevm/wagmi/releases/tag/wagmi%403.0.0): connector dependencies are optional, only install what you need.  v2 to v3 [migration guide](https://wagmi.sh/react/guides/migrate-from-v2-to-v3).
* [Feedback wanted](https://x.com/wevm_dev/status/1989174962092142688) to improve viem/wagmi.

#### [Web3j](https://docs.web3j.io/) (Java)
* [web3j-maven-plugin integration tips](https://blog.web3labs.com/integration-tips-for-web3j-maven-plugin-in-java-projects/) in Java projects.

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* ape [0.8.42](https://github.com/ApeWorX/ape/releases/tag/v0.8.42)

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.5.0](https://github.com/foundry-rs/foundry/releases/tag/v1.5.0): improved fuzzer with Solar AST analysis, browser wallet support & ERC20 interaction in cast and all binaries as npm packages.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* [Over 10.5 million contracts verified](https://sourcify.dev/#/#contract-stats), including ~1.3 million on mainnet.
* ~7.5 million signatures in [4byte](https://4byte.sourcify.dev) database.  2.5M function signatures came from [Etherface.io database](https://x.com/SourcifyEth/status/1989317288227455119).
* [Sourcify data on Google BigQuery](https://x.com/SourcifyEth/status/1991908836467409241) for analysis and integration.
* Kaan Uzdogan [why contract verification needs to open up](https://www.youtube.com/watch?v=S8QarbmvpcA) presentation at Trustless conference (Devconnect).

## Ethereum Layer 1

### Gas limit increase
* [60M gas limit](https://x.com/nero_eth/status/1993659827969458296) reached. [Gas benchmarking framework](https://www.nethermind.io/blog/measuring-ethereums-execution-limits-the-gas-benchmarking-framework) used to validate clients can handle heavier blocks.

### :zebra: [Fusaka upgrade](https://forkcast.org/upgrade/fusaka) (December 3 2025)

* Headliner: L2 scaling via [EIP-7594 PeerDAS](https://forkcast.org/upgrade/fusaka#eip-7594) and [EIP-7892 Blob parameter only upgrades](https://forkcast.org/upgrade/fusaka#eip-7892).
* [mainnet upgrades to Fusaka](https://ethereum-magicians.org/t/all-core-devs-consensus-acdc-168-october-30-2025/25893/2) on December 3.
* [Blob Parameter Only (BPO) upgrades](https://notes.ethereum.org/@bbusa/fusaka-bpo-timeline) (increase blobs per block target and maximum parameters):
    * BPO1: 10/15 (target/max blobs per block) December 9.
    * BPO2: 14/21 (target/max blobs per block) January 7, 2026.

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target 2026)

* Headliners: 
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/upgrade/glamsterdam#eip-7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/upgrade/glamsterdam#eip-7928).
  * [EIP-7805 FOCIL](https://eips.ethereum.org/EIPS/eip-7805) (Fork-choice enforced Inclusion Lists) [not included in Glamsterdam](https://forkcast.org/calls/acdc/170), non-headliner upgrade scope still being decided by All Core Devs.

## EF Devcon
* [Devcon 8 location](https://devcon.org/en/) is Mumbai, India in Q4 2026.
* [Devconnect Argentina videos](https://www.youtube.com/playlist?list=PLaM7G4Llrb7wViZDimf6uFLCJaDEkpe0k) available on YouTube.

## EF Ecosystem Support Program (ESP)
* [ESP new grants program](https://blog.ethereum.org/2025/11/03/new-esp-grants): pathways are via wishlist or requests for proposals (RFPs).

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.  
