---
slug: devtoolsguild-july-2026-update
title: Dev Tools Guild July 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild July 2026 update

_**TL;DR**: Solidity 0.8.36 adds Amsterdam EVM support. Sourcify passes 42M+ verified contracts. Foundry adds symbolic testing._

<!-- truncate -->

## Dev Tools Guild members

Argot Collective [H1 2026 transparency report](https://www.argot.org/reports/transparency-report-2026-h1) includes Solidity & Sourcify.

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* Solidity [0.8.36](https://www.soliditylang.org/blog/2026/07/09/solidity-0.8.36-release-announcement): adds Amsterdam EVM version support, fixes for medium severity bugs ([unsound spill in mutual recursion](https://www.soliditylang.org/blog/2026/07/09/unsound-spill-in-mutual-recursion-bug/) & [inheritance order reversal on storage end warning](https://www.soliditylang.org/blog/2026/07/09/inheritance-order-reversal-on-storage-end-warning-bug/)) and experimental SSA CFG stack to memory spilling (mitigate stack too deep).
* Argot Collective [Solidity roadmap update](https://www.argot.org/blog/2026-07-01-argot-roadmap-update-2026-2#solidity), Q1/2 review & Q3/4 focus for Classic & Core Solidity.
* Jacob Czepluch: [What's next for Solidity](https://www.youtube.com/watch?v=1zqv1NiPWQM) & Moritz Hoffmann [Fixing Stack Too Deep](https://www.youtube.com/watch?v=AlIw_bsAju4) Ethereum Day Berlin blockchain week presentations.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v2.2.0](https://github.com/alloy-rs/alloy/releases/tag/v2.2.0): adds `FromStr` for `PayloadId`, `AnyRpcBlock` header conversion and block gas limit validation.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.54.2](https://github.com/wevm/viem/releases/tag/viem%402.54.2) - [v2.55.10](https://github.com/wevm/viem/releases/tag/viem%402.55.10): adds allowing onchain signature verification to be pinned to a specific block via EIP-1898, `depositNonce` & `depositReceiptVersion` to OP Stack transaction receipts, `filterChains` utility and `getRawTransaction`.
* [viem.sh/tokens](https://viem.sh/tokens): type-safe, chain-aware utilities for interacting with tokens.
* wagmi [v3.7.0](https://github.com/wevm/wagmi/releases/tag/wagmi%403.7.0) - [v3.7.5](https://github.com/wevm/wagmi/releases/tag/wagmi%403.7.5).

### Frameworks and Dev Environments
#### [Foundry](https://getfoundry.sh/)
* Foundry [symbolic testing](https://x.com/gakonst/status/2072674688359186681): started to make progress towards symbolic/concolic execution, `forge test --symbolic`.

#### [Ape Framework](https://docs.apeworx.io/ape)
* [Ape Sourcify](https://github.com/ApeWorX/ape-sourcify) (plugin): automatically verifies Solidity + Vyper contracts, fetches verified sources/ABIs without API keys, and installs them as Ape dependencies by chain + address (`ape plugins install sourcify`).

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* [Sourcify roadmap update](https://docs.sourcify.dev/blog/recap-2026-h1/), Q1/2 review & Q3/4 focus.
* [42+ million contracts verified](https://stats.sourcify.dev/), including 7+ million on mainnet.
* [Sourcify v1 API retired July 7](https://docs.sourcify.dev/blog/api-v1-brownouts/), following scheduled brownouts; full migration to the v2 API completed.

## Ethereum Layer 1

* Ethereum celebrated [11 years since genesis](https://x.com/LefterisJP/status/2082771162942075080).
* Vitalik: [updated Strawmap explainer](https://x.com/VitalikButerin/status/2073459000398463446) (strawman L1 roadmap).
* Cambridge Centre for Alternative Finance [Ethereum environmental footprint](https://www.jbs.cam.ac.uk/faculty-research/centres/alternative-finance/publications/ethereum-after-the-merge-a-change-in-power/).

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target H2 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* [19 EIPs](https://forkcast.org/upgrade/glamsterdam/#scheduled-for-inclusion) Scheduled for Inclusion (SFI).
* [glamsterdam-devnet-7](https://forkcast.org/devnets/glamsterdam-devnet-7/): launched with remaining EIPs
* [Platåberget](https://forkcast.org/devnets/glamsterdam-devnet-8/): short lived permissionless public testnet, targeting early August.
* Public testnets: [targeting upgrading first testnet in September](https://forkcast.org/calls/acdc/183/#t=1219).
* 🐻‍❄️ [Polar bear selected](https://ethereum-magicians.org/t/polar-bear-selected-as-mascot-for-glamsterdam-upgrade/26008) as Glamsterdam mascot.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target 2027)

* Headliner: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
* Native account abstraction (via [EIP-8141 Frame transaction](https://forkcast.org/eips/8141/)) Considered for Inclusion (CFI).
* [36+ non-headliner EIPs](https://forkcast.org/upgrade/hegota/#proposed-for-inclusion) Proposed for Inclusion (PFI).

### Ethereum Foundation

* Ben Edgington: [fast finality stakeholder research](https://consensus.ethereum.foundation/blog/upgrading-finality-edition-2).
* EF Global Policy Strategy team: [Ethereum basics for governments & institutions](https://blog.ethereum.org/2026/07/01/ethereum-for-institutions), non-technical primer.
* [EF Board update](https://blog.ethereum.org/2026/07/29/ef-board-update): pcaversaccio (SEAL 911 co-founder & lead) joined the board for initial one-year voluntary term.
* EF Protocol Security team [running AI agents on protocol code](https://blog.ethereum.org/2026/07/09/triage-is-the-product).
* [EF Protocol Support team](https://x.com/TMIYChao/status/2074907379930440014) dissolved.
* Devcon 8 (Mumbai, India, November 3-6):
  * [Devcon tickets](https://devcon.org/en/tickets/).
  * [Devcon community hub applications](https://forum.devcon.org/t/rfp-13-devcon-8-india-community-hubs/8657) close August 12.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.