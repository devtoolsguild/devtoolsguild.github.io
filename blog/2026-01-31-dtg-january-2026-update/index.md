---
slug: devtoolsguild-january-2026-update
title: Dev Tools Guild January 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild January 2026 update

_**TL;DR**: BPO2 increases blobs to 14/21 (target/max), Octant Epoch 10 supports Solidity and Hegotá upgrade headliner proposals begin._

<!-- truncate -->

## Dev Tools Guild members

* Octant's [StreamVote](https://streamvote.octant.build/) supporting [ethers.js](https://streamvote.octant.build/project-details/0x8ba1f109551bd432803012645ac136ddd64dba72) (0.5 ETH), [Solidity](https://streamvote.octant.build/project-details/0xe2f7cf9c2b12c0bfcdab571f9e50418fc08f4ad1) (1.4 ETH) and [Vyper](https://streamvote.octant.build/project-details/0xd6e245ba9e1f71e629d6988d225a34542474a56a) (1.7 ETH); pilot streaming 25 ETH via quadratic voting to 7 public goods projects.
* Deep funding (infrastructure & dev tools) [update](https://gov.gitcoin.co/t/deep-funding-gg24-web3-tooling-and-infra-round/25040), anyone with an ENS can evaluate projects.

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* [Octant Epoch 10](https://octant.app/project/10/0xe2F7cF9C2b12c0BfcdAB571F9E50418fC08F4AD1) (top 25 projects from nine epochs): 46.3 ETH donated to Solidity.
* Solidity [Q1/Q2 2026 roadmap](https://www.argot.org/blog/2026-01-15-argot-roadmap-update-2026-1#solidity).

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v1.3.0](https://github.com/alloy-rs/alloy/releases/tag/v1.3.0) - [v1.5.2](https://github.com/alloy-rs/alloy/releases/tag/v1.5.2).

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.43.5](https://github.com/wevm/viem/releases/tag/viem%402.43.5) - [v2.45.1](https://github.com/wevm/viem/releases/tag/viem%402.45.1).
* wagmi [v3.1.4](https://github.com/wevm/wagmi/releases/tag/wagmi%403.1.4) - [v3.4.1](https://github.com/wevm/wagmi/releases/tag/wagmi%403.4.1).

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* ape [v0.8.44](https://github.com/ApeWorX/ape/releases/tag/v0.8.44) - [v0.8.47](https://github.com/ApeWorX/ape/releases/tag/v0.8.47).

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.6.0-rc1](https://github.com/foundry-rs/foundry/releases/tag/v1.6.0-rc1): Osaka default EVM, parallelized stateless fuzzing & configurable invariant check intervals, improved reentrancy detection and time-based invariant fuzzing.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Sourcify [Q1/Q2 2026 roadmap](https://www.argot.org/blog/2026-01-15-argot-roadmap-update-2026-1#sourcify).
* [Parquet Export v2](https://x.com/SourcifyEth/status/2008856171621540086) live, append-only exports, S3 compatible API, file metadata from Google Cloud Storage API and ~85% compression saving.
* Echidna [v2.3.1](https://github.com/crytic/echidna/releases/tag/v2.3.1): adds Sourcify support.
* [15k system paths found](https://x.com/apoorveth/status/2016801200965112146) in verified contracts.
  * Use [Sourcify dataset playground](https://sourcify.dev/#dataset-playground) to check.

## Ethereum Layer 1

### :zebra: [Fusaka upgrade](https://forkcast.org/upgrade/fusaka) (live on mainnet December 3 2025)

* [Blob Parameter Only (BPO) upgrades](https://forkcast.org/eips/7892) (increase blobs per block target and maximum parameters):
    * [BPO2](https://lab.ethpandaops.io/ethereum/forks/bpo2): 14/21 (target/max blobs per block) live January 7.

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target mid 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/upgrade/glamsterdam#eip-7732). 
    * [epbs-devnet-0](https://notes.ethereum.org/@ethpandaops/epbs-devnet-0) planned for late February.
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/upgrade/glamsterdam#eip-7928).
    * [bal-devnet-2](https://notes.ethereum.org/@ethpandaops/bal-devnet-2) launching early February.
* Non-headliner EIPs: [Considered for Inclusion](https://forkcast.org/upgrade/glamsterdam/#considered-for-inclusion) scope finalized with 18 EIPs.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Hegotá [scoping timeline](https://blog.ethereum.org/2025/12/22/hegota-timeline):
  * Headliner proposals (deadline February 4):
    * [EIP-7805](https://ethereum-magicians.org/t/hegota-headliner-proposal-focil-eip-7805/27604) Fork-choice enforced Inclusion Lists.
    * [EIP-8141](https://ethereum-magicians.org/t/hegota-headliner-proposal-frame-transaction/27618) Frame transaction (post-quantum security, native account abstraction and gas sponsorship).
    * [EIP-8105](https://ethereum-magicians.org/t/hegota-headliner-proposal-eip-8105-universal-enshrined-encrypted-mempool-eem/27448) Universal enshrined encrypted mempool.
    * [EIP-7807](https://ethereum-magicians.org/t/hegota-headliner-proposal-ssz-execution-blocks/27619) SSZ execution blocks.
  * Headliner selection: February 5–26.
  * Non-headliner EIP proposals: 30 day window.

### Ethereum Foundation

* EF Protocol Support team [Checkpoint #8](https://blog.ethereum.org/2026/01/20/checkpoint-8).
* [EF Post Quantum](https://x.com/drakefjustin/status/2014791629408784816) initiatives.
* EF Ecosystem Support Program [Q4 grants](https://blog.ethereum.org/2026/01/27/allocation-q4-25), 51 projects shared $7.4M.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
