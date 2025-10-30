---
slug: devtoolsguild-october-update
title: Dev Tools Guild October update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild October update

_**TL;DR**: Fusaka upgrade on mainnet December 3, Gitcoin Grants 24 included quadratic & deep funding for developer tooling and Optimism's Retro Funding continues to support member projects._

<!-- truncate -->

## Dev Tools Guild members

* [Gitcoin Grants 24](https://www.gitcoin.co/blog/announcing-gitcoin-grants-24) (GG24) included [quadratic funding](https://giveth.io/qf/gg24dti) and deep funding for developer tooling & infrastructure projects/repositories.
* Optimism's [Retro Funding: Dev Tooling](https://atlas.optimism.io/missions/retro-funding-dev-tooling) continues to support [Solidity](https://atlas.optimism.io/project/0xcc8d03e014e121d10602eeff729b755d5dc6a317df0d6302c8a9d3b5424aaba8), [Vyper](https://atlas.optimism.io/project/0x9ca1f7b0e0d10d3bd2619e51a54f2e4175e029c87a2944cf1ebc89164ba77ea0), [alloy](https://atlas.optimism.io/project/0x56ce7cbc27852a8d8ef5869dc9033a215c8893f799468f61527dacb9f92be790), [ethers.js](https://atlas.optimism.io/project/0xa3d07f453f70d844196d89d79848aa2e70a0bd8b38bf0f493cba1547bb3bca5e), [viem](https://atlas.optimism.io/project/0x6bd057da522918a4675396313ae33a2f2788a1ceeb3bd7ae228015e3eb317a7d), [web3.py](https://atlas.optimism.io/project/0xebe03c3d6d33cad60124b9b05ef6e2ff056293a1de3c5fa51dfbb90c86c14bf7), [Ape Framework](https://atlas.optimism.io/project/0xa0b16714baef75d97ec07fd48eaf42e79df92fe2a3c2d725d2388ede587ea54c), [Foundry](https://atlas.optimism.io/project/0x4562c0630907577f433cad78c7e2cc03349d918b6c14ef982f11a2678f5999ad), [Scaffold-ETH](https://atlas.optimism.io/project/0x154a42e5ca88d7c2732fda74d6eb611057fc88dbe6f0ff3aae7b89c2cd1666ab) and [Sourcify](https://atlas.optimism.io/project/0x51cda5996ef1a2ccd8fcf4ee5792337695599454c83eb1218c3ad4388dcb5bf5).

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/) 
* [Road to Core Solidity](https://www.soliditylang.org/blog/2025/10/21/the-road-to-core-solidity/):  
  * Core Solidity is a planned revamp of the language with a minimalist standard library, Classic Solidity is the language supported by solc today with planned breaking releases.
  * [Call for feedback](https://forum.soliditylang.org/t/call-for-feedback-the-long-term-solidity-roadmap/3530).
* Solidity added [pre-releases](https://x.com/solidity_lang/status/1979169207016153111) for developers to try out experimental features: 
  * Solidity [v0.8.31-pre.1](https://github.com/argotorg/solidity/releases/tag/v0.8.31-pre.1): adds EIP-7939 CLZ opcode support which results in cheaper compute & ZK proving costs and smaller bytecode size.
* [Solidity Summit](https://www.soliditylang.org/summit/) November 18 at Devconnect in Buenos Aires: apply for your ticket to attend.

#### [Vyper](https://vyperlang.org/)
* [Institutional adoption of Vyper](https://www.youtube.com/watch?v=gzlxgMNqDz8) presentation at Stablecoin Summit.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v1.0.38](https://github.com/alloy-rs/alloy/releases/tag/v1.0.38) - [v1.0.41](https://github.com/alloy-rs/alloy/releases/tag/v1.0.41).

#### [viem](https://viem.sh/) (TypeScript)
* viem [2.37.10](https://github.com/wevm/viem/releases/tag/viem%402.37.10) - [2.38.5](https://github.com/wevm/viem/releases/tag/viem%402.38.5); v2.38.0 added `sendTransactionSync`, `sendRawTransactionSync`, `writeContractSync` and `sendCallsSync`.
* App devs using [viem & wagmi for ENS resolution](https://x.com/gregskril/status/1975302868078109068) should update to v2.35+ for automatic support when ENSv2 launches.

### [Web3j](https://docs.web3j.io/)
* [New Smart Account Tutorial With Web3j](https://www.lfdecentralizedtrust.org/blog/erc-4337-smart-account-tutorial-with-web3j).

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* Ape Framework [adding support for Python 3.14](https://x.com/ApeFramework/status/1976413892399202816) (where possible) and deprecating support for Python 3.9 (end of life).
* ape-safe MultiSend [add from receipt](https://x.com/fubuloubu/status/1980346349548892593): improves creating multi-step calls in Safe.

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.3.7](https://github.com/foundry-rs/foundry/releases/tag/v1.3.7) - [v1.4.3](https://github.com/foundry-rs/foundry/releases/tag/v1.4.3); v1.4.0 is Fusaka upgrade ready, forge is published as an npm package, improves performance up to 11% for forge coverage & fuzzed tests, adds a formatter built on Solar, improved handling of multichain configs and deployments and improved testing/debugging with backtraces & custom network precompiles.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Remix [v1.1.0](https://ethereumremix.substack.com/p/remix-release-v1-1-0) adds Deploy & Verify: verify when deploying contracts with all verifiers.
* samczsun's [openchain signature database](https://x.com/SourcifyEth/status/1980657962990600647) being taken over by Sourcify.

## Ethereum Layer 1

### Gas limit increase

* Clients are increasing default gas limit to 60M (up from 45M): Erigon [v3.2.1](https://github.com/erigontech/erigon/releases/tag/v3.2.1), Nethermind [v1.35.0](https://github.com/NethermindEth/nethermind/releases/tag/1.35.0) and Teku [25.10.0](https://github.com/Consensys/teku/releases/tag/25.10.0).


### :zebra: [Fusaka upgrade](https://forkcast.org/upgrade/fusaka) (December 3 2025)

* Headliner: L2 scaling via [EIP7594 PeerDAS](https://forkcast.org/upgrade/fusaka#eip-7594) and [EIP7892 Blob parameter only upgrades](https://forkcast.org/upgrade/fusaka#eip-7892).
* mainnet upgrades to Fusaka on December 3.
* [Blob Parameter Only (BPO) upgrades](https://notes.ethereum.org/@bbusa/fusaka-bpo-timeline) (increase blobs per block target and maximum parameters):
    * BPO1: 10/15 (target/max blobs per block) December 9.
    * BPO2: 14/21 (target/max blobs per block) January 7, 2026.
* Holešky, Sepolia & Hoodi testnets were all successfully upgraded.
* [Fusaka $2M audit contest](https://blog.ethereum.org/2025/09/15/fusaka-audit-content) ended, nothing to cause postponing upgrade.
* Note for devs: 
  * [EIP-7825: transaction gas limit cap](https://blog.ethereum.org/2025/10/21/fusaka-gascap-update) of ~16.8M gas
  * EIP-7594: PeerDAS [changes format for proofs](https://blog.ethereum.org/2025/10/15/fusaka-blob-update) from blob proofs to cell proofs.

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target 2026)

* Headliners: 
  * Consensus layer: [EIP7732 ePBS](https://forkcast.org/upgrade/glamsterdam#eip-7732).
  * Execution layer: [EIP7928 Block-level Access Lists](https://forkcast.org/upgrade/glamsterdam#eip-7928).
* Non-headliners:
  * EIPs [proposed for inclusion](https://forkcast.org/upgrade/glamsterdam#proposed-for-inclusion) (30+) will be reviewed by client teams.
  * [Rank non-headliner EIPs on Forkcast](https://forkcast.org/rank) and share on socials to signal your priorities. 

### H-star + Bogotá upgrade
* [H-star](https://ethereum-magicians.org/t/h-star-name-for-consensus-layer-upgrade-after-glamsterdam/24298) name needed, signal your favourite in the poll.

### Holešky testnet
* [Holešky was deprecated](https://blog.ethereum.org/2025/09/01/holesky-shutdown-announcement) after upgrading to Fusaka, BPO1 & BPO2 and is no longer finalizing.  Migrate to Hoodi testnet for infrastructure testing or Sepolia testnet for app layer testing.

### Privacy
* Ethereum Foundation [expanding privacy efforts](https://blog.ethereum.org/2025/10/08/privacy-commitment): initiatives include private reads & writes, private proving, private identities, privacy experince, institutional privacy task force and [Kohaku](https://notes.ethereum.org/@niard/KohakuRoadmap) (wallet SDK & reference implementation of a browser extension).

### EF internships
* [2026 EF Internships](https://blog.ethereum.org/2025/10/14/internship-2026): 12 weeks over Northern hemisphere summer, applications close December 1.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.  




