---
slug: devtoolsguild-september-update
title: Dev Tools Guild September update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild September update

_**TL;DR**: Fusaka upgrade on testnets in October, ENS DAO granted $75k to Argot, Aerodrome donated $450k between various teams, Optimism's Retro Funding continues to support member projects._

<!-- truncate -->

## Dev Tools Guild members

* [ENS DAO public goods working group](https://discuss.ens.domains/t/ens-public-goods-working-group-funding-argot/21443) granted $75k to Argot Collective (includes Solidity and Sourcify).
* [Aerodrome](https://x.com/AerodromeFi/status/1962963079551156714) donated $450k between 7 teams, including Vyper, Viem and Ape Framework.
* Optimism's [Retro Funding: Dev Tooling](https://atlas.optimism.io/missions/retro-funding-dev-tooling) continues to support [Solidity](https://atlas.optimism.io/project/0xcc8d03e014e121d10602eeff729b755d5dc6a317df0d6302c8a9d3b5424aaba8), [Vyper](https://atlas.optimism.io/project/0x9ca1f7b0e0d10d3bd2619e51a54f2e4175e029c87a2944cf1ebc89164ba77ea0), [alloy](https://atlas.optimism.io/project/0x56ce7cbc27852a8d8ef5869dc9033a215c8893f799468f61527dacb9f92be790), [ethers.js](https://atlas.optimism.io/project/0xa3d07f453f70d844196d89d79848aa2e70a0bd8b38bf0f493cba1547bb3bca5e), [Nethereum](https://atlas.optimism.io/project/0x4a5e771af86cf1938056b43cddbf0018dca1376d578f631f7449fe10ac4958ed), [viem](https://atlas.optimism.io/project/0x6bd057da522918a4675396313ae33a2f2788a1ceeb3bd7ae228015e3eb317a7d), [web3.py](https://atlas.optimism.io/project/0xebe03c3d6d33cad60124b9b05ef6e2ff056293a1de3c5fa51dfbb90c86c14bf7), [Ape Framework](https://atlas.optimism.io/project/0xa0b16714baef75d97ec07fd48eaf42e79df92fe2a3c2d725d2388ede587ea54c), [Foundry](https://atlas.optimism.io/project/0x4562c0630907577f433cad78c7e2cc03349d918b6c14ef982f11a2678f5999ad), [Scaffold-ETH](https://atlas.optimism.io/project/0x154a42e5ca88d7c2732fda74d6eb611057fc88dbe6f0ff3aae7b89c2cd1666ab) and [Sourcify](https://atlas.optimism.io/project/0x51cda5996ef1a2ccd8fcf4ee5792337695599454c83eb1218c3ad4388dcb5bf5).

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/) 
* Solidity [2025 roadmap update](https://www.argot.org/blog/2025-roadmap-update#solidity).
* IEEE [2025 top programming languages](https://spectrum.ieee.org/top-programming-languages-2025) includes Solidity.

#### [Vyper](https://vyperlang.org/)
* [Vyper team completed all milestones](https://x.com/vyperlang/status/1968142163008794961) for their Arbitrum $50k grant.  Funding went towards raw_return decorator & raw_create builtin for low level control of proxy patterns and a non-reentrancy pragma. 

### Client Libraries
#### [alloy](https://alloy.rs/)
* alloy [v1.0.28](https://github.com/alloy-rs/alloy/releases/tag/v1.0.28) - [v1.0.36](https://github.com/alloy-rs/alloy/releases/tag/v1.0.36).

#### [viem](https://viem.sh/)
* viem [2.36.1](https://github.com/wevm/viem/releases/tag/viem%402.36.1) - [2.37.9](https://github.com/wevm/viem/releases/tag/viem%402.37.9).

### [Web3j](https://docs.web3j.io/)
* web3j [v5.0.1](https://github.com/LFDT-web3j/web3j/releases/tag/v5.0.1).

### Frameworks and Dev Environments
#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.3.1](https://github.com/foundry-rs/foundry/releases/tag/v1.3.1) - [v1.3.6](https://github.com/foundry-rs/foundry/releases/tag/v1.3.6) 

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Sourcify [2025 roadmap update](https://www.argot.org/blog/2025-roadmap-update#sourcify).
* Sourcify [dataset playground](https://sourcify.dev/#/dataset-playground): AI assisted query generation for use with Sourcify dataset in BigQuery.
* [Foundry updated](https://x.com/kaanuzdogan/status/1963505296505978910) to use Sourcify APIv2.

## Ethereum Layer 1

### [Fusaka upgrade](https://forkcast.org/upgrade/fusaka) (target Q4 2025)

* Headliner: L2 scaling via [EIP7594 PeerDAS](https://forkcast.org/upgrade/fusaka#eip-7594) and [EIP7892 Blob parameter only upgrades](https://forkcast.org/upgrade/fusaka#eip-7892).
* [Fusaka upgrade](https://blog.ethereum.org/2025/09/26/fusaka-testnet-announcement) testnet schedule:
  * Holešky: October 1, 8:48 UTC (Slot: 5,283,840).
  * Sepolia: October 14, 7:36 UTC (Slot: 8,724,480).
  * Hoodi: October 28, 18:53 UTC (Slot: 1,622,016).
  * Blob Parameter Only (BPO) upgrades (increase blobs per block target and maximum parameters):
    * BPO1: 10/15 (target/max blobs per block) (~1 week after Fusaka on testnets).
    * BPO2: 14/21 (target/max blobs per block) (~1 week after BPO1 on testnets).
* [Fusaka audit contest](https://blog.ethereum.org/2025/09/15/fusaka-audit-content) with up to $2M in rewards.
* mainnet upgrade: December (at the earliest, if testing goes well).    

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target 2026)

* Headliners: 
  * Consensus layer: [EIP7732 ePBS](https://forkcast.org/upgrade/glamsterdam#eip-7732).
  * Execution layer: [EIP7928 Block-level Access Lists](https://forkcast.org/upgrade/glamsterdam#eip-7928).
* Non-headliners:
  * EIPs are being [proposed for inclusion](https://forkcast.org/upgrade/glamsterdam#proposed-for-inclusion) (23 so far), with client teams specifying which EIPs they want more info on.
  * [Rank non-headliner EIPs on Forkcast](https://forkcast.org/rank) and share on socials to signal your priorities. 
  * Deadline for proposals is Fusaka mainnet releases (~November). 

### H-star + Bogotá upgrade
* [H-star](https://ethereum-magicians.org/t/h-star-name-for-consensus-layer-upgrade-after-glamsterdam/24298) name needed, signal your favourite in the poll.

### Holešky testnet
* [Holešky will be deprecated](https://blog.ethereum.org/2025/09/01/holesky-shutdown-announcement) after upgrading to Fusaka and BPO1 & BPO2.

### Protocol calls
* Protocol calls (All Core Devs Execution/Consensus/Test) [available on Forkcast](https://forkcast.org/calls/) with recording, transcript, chat log and (experimental) AI generated summary.
* [Ansgar Dietrichs chairing All Core Devs Execution](https://x.com/TimBeiko/status/1965047756386644270) until the end of the year.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate).**  Donations of all sizes are greatly appreciated.  




