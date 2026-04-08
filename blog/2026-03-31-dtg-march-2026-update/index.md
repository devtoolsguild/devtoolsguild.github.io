---
slug: devtoolsguild-march-2026-update
title: Dev Tools Guild March 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild March 2026 update

_**TL;DR**: Nethereum 6, EF post-quantum website & EF bug bounty $1M max payout._

<!-- truncate -->

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* Solidity [v0.8.35-pre.1](https://github.com/argotorg/solidity/releases/tag/v0.8.35-pre.1) (prerelease): experimental mode enabled by explicit flag and recorded in JSON & CBOR metadata, builtin computes base slot of storage namespace using ERC7201, experimental SSA CFG codegen and performance fix in Yul EVM code transform.
* Jacob: [Solidity vision](https://x.com/solidity_lang/status/2034636973290439107) on ECH Institute podcast.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v1.7.4](https://github.com/alloy-rs/alloy/releases/tag/v1.7.4) - [v1.8.3](https://github.com/alloy-rs/alloy/releases/tag/v1.8.3).

#### [Nethereum](https://nethereum.com/)
* Nethereum [6.0.0](https://github.com/Nethereum/Nethereum/releases/tag/6.0.0) - [6.1.0](https://github.com/Nethereum/Nethereum/releases/tag/6.1.0): adds in process node, dev network with SQLite persistence, multinode app chain, account abstraction, block explorer, multiprovider storage, .NET Aspire orchestration, full stack app template, zk proof infrastructure, Groth16 proof generation, Privacy Pools integration, Merkle tree libraries, SSZ model improvements, cross-platform BLS runtime updates and demo apps.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.47.0](https://github.com/wevm/viem/releases/tag/viem%402.47.0) - [v2.47.6](https://github.com/wevm/viem/releases/tag/viem%402.47.6).
* wagmi [v3.6.0](https://github.com/wevm/wagmi/releases/tag/wagmi%403.6.0).

### Frameworks and Dev Environments
#### [Scaffold-ETH](https://scaffoldeth.io/)
* [Scaffold-ETH shifted to AI native developer stack](https://x.com/buidlguidl/status/2030977075226480821): agent first docs, skills rather than scripts & AI-assisted code review.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* [Hardhat ignition](https://x.com/SourcifyEth/status/2036062580553265555) submits to all verifiers in parallel, including Sourcify.
* [Sourcify top Open Labels labeller](https://x.com/SourcifyEth/status/2029442916574196201) attesting to 21M verified contracts.
* [Ethereum history added Sourcify](https://x.com/cartoonitunes/status/2038419155649446296) for earlier Solidity versions support.

## Ethereum Layer 1

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target mid 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* [glamsterdam-devnet-0](https://notes.ethereum.org/@ethpandaops/glamsterdam-devnet-0) targeting second half of April.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target late 2026)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
  * Execution layer: no headliner selected.  
* [EIP-8141 Frame Transactions](https://forkcast.org/eips/8141) considered for inclusion as non-headliner.

### Ethereum Foundation (EF)

* [Bug bounty maximum payout](https://x.com/fredrik0x/status/2031094726271672488) increased to $1M, up from $250k.
* Post-quantum: 
  * [Post-quantum website](https://pq.ethereum.org): overview, roadmap, resources and FAQ.
  * Justin Drake: [overview of quantum breakthrough papers](https://x.com/drakefjustin/status/2038847732152996108).
* [Fast confirmation rule](https://fastconfirm.it/) info website, confirm transactions in ~13 seconds, no network upgrade required.
* Platform team: [L1 + L2 relationship](https://blog.ethereum.org/2026/03/23/l1-l2-ethereum).
* Protocol cluster priority: [hardness overview](https://x.com/ethereum/status/2034307029272293478).
* Protocol support: [EIP champions handbook](https://ps.ethereum.foundation/guides/champion).
* Ecosystem Support Program [funded projects explorer](https://esp.ethereum.foundation/funded-projects).
* [EF Mandate](https://blog.ethereum.org/2026/03/13/ef-mandate): Ethereum must remain censorship resistant, open source, private and secure (CROPS).
* [Synthesis](https://x.com/synthesis_md/status/2039980188323488054) AI + human hackathon winners.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
