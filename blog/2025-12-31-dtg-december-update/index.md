---
slug: devtoolsguild-december-update
title: Dev Tools Guild December update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild December update

_**TL;DR**: mainnet successfully upgraded to Fusaka & BPO1, Optimism's Retro Funding continues to support member projects and Octant's StreamVote supports ethers.js, Solidity & Vyper._

<!-- truncate -->

## Dev Tools Guild members

* Optimism's [Retro Funding: Dev Tooling](https://atlas.optimism.io/missions/retro-funding-dev-tooling) continues to support [Solidity](https://atlas.optimism.io/project/0xcc8d03e014e121d10602eeff729b755d5dc6a317df0d6302c8a9d3b5424aaba8), [Vyper](https://atlas.optimism.io/project/0x9ca1f7b0e0d10d3bd2619e51a54f2e4175e029c87a2944cf1ebc89164ba77ea0), [alloy](https://atlas.optimism.io/project/0x56ce7cbc27852a8d8ef5869dc9033a215c8893f799468f61527dacb9f92be790), [ethers.js](https://atlas.optimism.io/project/0xa3d07f453f70d844196d89d79848aa2e70a0bd8b38bf0f493cba1547bb3bca5e), [viem](https://atlas.optimism.io/project/0x6bd057da522918a4675396313ae33a2f2788a1ceeb3bd7ae228015e3eb317a7d), [web3.py](https://atlas.optimism.io/project/0xebe03c3d6d33cad60124b9b05ef6e2ff056293a1de3c5fa51dfbb90c86c14bf7), [Ape Framework](https://atlas.optimism.io/project/0xa0b16714baef75d97ec07fd48eaf42e79df92fe2a3c2d725d2388ede587ea54c), [Foundry](https://atlas.optimism.io/project/0x4562c0630907577f433cad78c7e2cc03349d918b6c14ef982f11a2678f5999ad), [Scaffold-ETH](https://atlas.optimism.io/project/0x154a42e5ca88d7c2732fda74d6eb611057fc88dbe6f0ff3aae7b89c2cd1666ab) and [Sourcify](https://atlas.optimism.io/project/0x51cda5996ef1a2ccd8fcf4ee5792337695599454c83eb1218c3ad4388dcb5bf5).
* Octant's [StreamVote](https://streamvote.octant.build/) supporting [ethers.js](https://streamvote.octant.build/project-details/0x8ba1f109551bd432803012645ac136ddd64dba72), [Solidity](https://streamvote.octant.build/project-details/0xe2f7cf9c2b12c0bfcdab571f9e50418fc08f4ad1) & [Vyper](https://streamvote.octant.build/project-details/0xd6e245ba9e1f71e629d6988d225a34542474a56a); pilot streaming 25 ETH via quadratic voting to 17 public goods projects.
* Deep funding (infrastructure & dev tools) [volunteer jurors wanted](https://x.com/devanshmehta/status/2001332858271780897): research & compare repositories, comparisons select winning AI models, which distribute funding.

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/) 
* Solidity [v0.8.31](https://www.soliditylang.org/blog/2025/12/03/solidity-0.8.31-release-announcement/): Fusaka support: osaka default EVM version & CLZ opcode; pre-releases; constants in storage layout specifiers; deprecation warnings for address send/transfer, ABI coder v1, virtual modifiers, contract comparison operators & memory-safe-assembly Natspec comment.
* Solidity [v0.8.32/33](https://www.soliditylang.org/blog/2025/12/18/solidity-0.8.32-0.8.33-release-announcement): fix for [lost storage array write on slot overflow](https://www.soliditylang.org/blog/2025/12/18/lost-storage-array-write-on-slot-overflow-bug/).
* [Solidity Summit recap](https://www.soliditylang.org/blog/2025/12/04/solidity-summit-2025-recap/): recordings and slides from Devconnect.
* [2025 recap](https://x.com/argotorg/status/2005987291194651129).
* Reminder: Solidity is in [Octant Epoch 10](https://x.com/OctantApp/status/1993802455038218415) (top 25 projects from nine epochs), allocation is January 6-20.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v1.1.3](https://github.com/alloy-rs/alloy/releases/tag/v1.1.3) - [v1.2.1](https://github.com/alloy-rs/alloy/releases/tag/v1.2.1).

#### [Nethereum](https://nethereum.com/)
* Nethereum [5.8.0](https://github.com/Nethereum/Nethereum/releases/tag/5.8.0): 10 year anniversary release; full consensus light client + execution state verification stack, Nethereum.Wallet reusable wallet platform, hardware wallet upgrade with end-to-end Trezor support, expanded protocol integrations (X402, Uniswap Permit2 + Universal Router, Circles & Safe utilities) and updated/expanded data services (ChainList, CoinGecko, Etherscan v2).

#### [ethers.js](https://ethers.org/) (TypeScript)
* ethers.js [v6.16.0](https://github.com/ethers-io/ethers.js/releases/tag/v6.16.0): Fusaka support: EIP7594 PeerDAS cell proofs.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.40.4](https://github.com/wevm/viem/releases/tag/viem%402.40.4) - [v2.43.4](https://github.com/wevm/viem/releases/tag/viem%402.43.4): includes [contract function/event/error parameter names](https://x.com/wevm_dev/status/2001328114182619244) in editor autocomplete, hover, typescript error messages and more.
* wagmi [v3.1.0](https://github.com/wevm/wagmi/releases/tag/wagmi%403.1.0) - [v3.1.4](https://github.com/wevm/wagmi/releases/tag/wagmi%403.1.4).

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* ape [v0.8.43](https://github.com/ApeWorX/ape/releases/tag/v0.8.43).
* [ape-dprc](https://github.com/ApeWorX/ape-drpc#readme): plugin for dRPC.

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.5.1](https://github.com/foundry-rs/foundry/releases/tag/v1.5.1): solc v0.8.31 support.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* [Sourcify: open source & open data in source code verification](https://x.com/PowerhouseDAO/status/1996598729210495292) Devconnect presentation.
* [2025 recap](https://docs.sourcify.dev/blog/recap-2025/).

## Ethereum Layer 1

### :zebra: [Fusaka upgrade](https://forkcast.org/upgrade/fusaka) (live on mainnet December 3 2025)

* Headliners: L2 scaling via [EIP-7594 PeerDAS](https://forkcast.org/upgrade/fusaka#eip-7594) and [EIP-7892 Blob parameter only upgrades](https://forkcast.org/upgrade/fusaka#eip-7892).
* mainnet upgraded to Fusaka on December 3.
* [Blob Parameter Only (BPO) upgrades](https://notes.ethereum.org/@bbusa/fusaka-bpo-timeline) (increase blobs per block target and maximum parameters):
    * BPO1: 10/15 (target/max blobs per block) completed December 9.
    * BPO2: 14/21 (target/max blobs per block) scheduled for January 7, 2026.

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target June 2026)

* Headliners: 
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/upgrade/glamsterdam#eip-7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/upgrade/glamsterdam#eip-7928).
* Non-headliner EIPs [Considered for Inclusion](https://forkcast.org/upgrade/glamsterdam/#considered-for-inclusion).

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Hegotá [scoping timeline](https://blog.ethereum.org/2025/12/22/hegota-timeline):
  * Fork focus & headliner proposals: January 8 – February 4.
  * Headliner selection: February 5–26.
  * Non-headliner EIP proposals: 30 day window.

### Ethereum Foundation

* [Devcon 8](https://blog.ethereum.org/2025/12/23/devcon-mumbai): November 3-6 at the JIO World Center in Mumbai, India
* [Devconnect Argentina recap](https://blog.ethereum.org/2025/12/04/devconnect-arg-wrap), 14k+ attendees, 45% from Argentina, 15 community hubs and 500+ side events.
* EF Ecosystem Support Program [Q3 grants](https://blog.ethereum.org/2025/12/02/allocation-q3-25), 80 projects shared $14.3M.
* [L1 zkEVM security milestones](https://blog.ethereum.org/2025/12/18/zkevm-security-foundations): soundcalc integration by end of February; 100-bit provable security with < 600 KiB proof size by end of May; 128-bit provable security with < 300 Kib proof size by end of 2026.
* EF Stateless Consensus team: [future of state](https://blog.ethereum.org/2025/12/16/future-of-state), challenges of state growth and who holds & serves state; broad directions of state expiry, state archive and making it easier to hold & serve state. 

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.

