---
slug: devtoolsguild-february-2026-update
title: Dev Tools Guild February 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild February 2026 update

_**TL;DR**: Solidity developer survey, 20+ million contracts verified on Sourcify and strawmap (strawman roadmap) for next seven network upgrades._

<!-- truncate -->

## Dev Tools Guild members

* Deep Funding (infrastructure & dev tools): [jurors wanted](https://deepfundingjury.com) to evaluate and compare open source projects. Anyone with an ENS name can participate.  Thanks to the [jurors who have already contributed](https://deepfundingjury.com/juror-roll).
* Octant's [StreamVote](https://streamvote.octant.build/) supporting [ethers.js](https://streamvote.octant.build/project-details/0x8ba1f109551bd432803012645ac136ddd64dba72) (0.7 ETH), [Solidity](https://streamvote.octant.build/project-details/0xe2f7cf9c2b12c0bfcdab571f9e50418fc08f4ad1) (2.2 ETH) and [Vyper](https://streamvote.octant.build/project-details/0xd6e245ba9e1f71e629d6988d225a34542474a56a) (2.5 ETH); pilot streaming ETH via quadratic voting to public goods projects.
* Argot Collective (including Solidity & Sourcify) [transparency report](https://www.argot.org/reports/transparency-report-2025).

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* Annual [Solidity developer survey](https://www.soliditylang.org/blog/2026/02/10/solidity-developer-survey-2025-announcement/), takes 5 minutes to complete, with a chance to win a ticket to Devcon.
* Solidity [v0.8.34](https://github.com/ethereum/solidity/releases/tag/v0.8.34): fix for [transient storage clearing helper collision bug](https://www.soliditylang.org/blog/2026/02/18/transient-storage-clearing-helper-collision-bug/).  Three deployed contracts found with affected pattern.
* [revertStrings strip](https://x.com/solidity_lang/status/2026349594691645537) behavior is being aligned between legacy and IR pipelines to remove both strings and custom errors from require statements.
* [Jacob](https://x.com/_czepluch/status/2026315378096320932) joined as Developer Advocate.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v1.6.0](https://github.com/alloy-rs/alloy/releases/tag/v1.6.0) - [v1.7.3](https://github.com/alloy-rs/alloy/releases/tag/v1.7.3).

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.45.2](https://github.com/wevm/viem/releases/tag/viem%402.45.2) - [v2.46.3](https://github.com/wevm/viem/releases/tag/viem%402.46.3).
* wagmi [v3.4.3](https://github.com/wevm/wagmi/releases/tag/wagmi%403.4.3) - [v3.5.0](https://github.com/wevm/wagmi/releases/tag/wagmi%403.5.0).

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* ape [v0.8.48](https://github.com/ApeWorX/ape/releases/tag/v0.8.48).

#### [Foundry](https://getfoundry.sh/)
* forge-std [v1.15.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.15.0).

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* [20+ million contracts verified](https://stats.sourcify.dev/), including 6.5 million on mainnet.
* [Sourcify documentation](https://x.com/SourcifyEth/status/2022224841559232622) revamped.
* [ETHPrague hackathon](https://x.com/EthPrague/status/2023714253258011000): $4k bounty for builders working with Sourcify.

## Ethereum Layer 1

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target mid 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/upgrade/glamsterdam#eip-7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/upgrade/glamsterdam#eip-7928).
* Implementation progress: bal-devnet-3 ([spec](https://notes.ethereum.org/@ethpandaops/bal-devnet-3)) and epbs-devnet-0 ([spec](https://notes.ethereum.org/@ethpandaops/epbs-devnet-0)) targeting early March.
* Gas repricing: [info website](https://gasrepricing.com/) and [stakeholder survey](https://docs.google.com/forms/d/e/1FAIpQLScmhDCX1I8-RPFL-AEEBJkBkAtbCq_M9quXHspF_OltTbGCGw/viewform).

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://ethereum-magicians.org/t/hegota-headliner-proposal-focil-eip-7805/27604) (Fork-choice enforced Inclusion Lists).
  * Execution layer still deciding: [EIP-8141 Frame Transactions](https://ethereum-magicians.org/t/hegota-headliner-proposal-frame-transaction/27618) is leading candidate.

### Ethereum Foundation (EF)

* [Strawmap](https://strawmap.org/faq): strawman roadmap for next seven network upgrades.
* EF [leadership update](https://blog.ethereum.org/2026/02/13/leadership-update): Tomasz Stańczak [stepped down](https://blog.ethereum.org/2026/02/13/tomasz-update) as Co-Executive Director; Bastian Aue interim Co-Executive Director.
* Updated [protocol priorities](https://blog.ethereum.org/2026/02/18/protocol-priorities-update-2026): three tracks - Scale, Improve UX and Harden the L1.
* EF [treasury staking](https://blog.ethereum.org/2026/02/24/staking): ~70k ETH being staked.
* New [Platform team](https://blog.ethereum.org/2026/02/17/platform): focused on strongest possible platform (L1 + L2).
* [Ethereum protocol studies](https://blog.ethereum.org/2026/02/17/ethereum-protocol-studies-26): new cryptography and zkEVM tracks.
* Ecosystem Support Program wishlist: [existing dev tooling](https://esp.ethereum.foundation/applicants/wishlist/existing-devtool), seeking proposals to sustain, improve & extend existing dev tools, application deadline is April 15.
* [Project Odin](https://blog.ethereum.org/2026/02/27/project-odin): sustainability planning & execution for strategic EF grantees.  Vyper core team (Foundation for Verified Software) is piloting.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
