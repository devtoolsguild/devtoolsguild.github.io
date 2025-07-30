---
slug: devtoolsguild-july-update
title: Dev Tools Guild July update
authors: [abcoathup]
tags: [update]
draft: true
---

# Dev Tools Guild July update

_**TL;DR**: Ethereum and Solidity turn ten.  Ethereum Foundation, Octant and Optimism's Retro Funding support member projects.  Gas limit to 45M. Partial history expiry.  Fusaka upgrade: targeting Q4.  Glamsterdam upgrade: feedback wanted on proposed headliners_

<!-- truncate -->

## Dev Tools Guild members

* [Argot Collective](https://argot.org/) (includes Solidity & Sourcify) secured [three years of operational funding](https://argot.org/blog/ef-grant-announcement) from the Ethereum Foundation.
* Golem Foundation's [Octant Epoch 8](https://x.com/OctantApp/status/1948437029555220557) supported [Solidity](https://octant.app/project/8/0xe2F7cF9C2b12c0BfcdAB571F9E50418fC08F4AD1), [Vyper](https://octant.app/project/8/0x0b450A3688a55d4221329D31e2F103bCe9adAc40), [ethers.js](https://octant.app/project/8/0x8ba1f109551bD432803012645Ac136ddd64DBA72) and Scaffold-ETH (via [BuidlGuidl](https://octant.app/project/8/0x6A4E5ed62d3827128Dbd70c5bDe25C0e6c6aA537)).
* Optimism's [Retro Funding: Dev Tooling](https://atlas.optimism.io/missions/retro-funding-dev-tooling) continues to support [Solidity](https://atlas.optimism.io/project/0xcc8d03e014e121d10602eeff729b755d5dc6a317df0d6302c8a9d3b5424aaba8), [Vyper](https://atlas.optimism.io/project/0x9ca1f7b0e0d10d3bd2619e51a54f2e4175e029c87a2944cf1ebc89164ba77ea0), [alloy](https://atlas.optimism.io/project/0x56ce7cbc27852a8d8ef5869dc9033a215c8893f799468f61527dacb9f92be790), [ethers.js](https://atlas.optimism.io/project/0xa3d07f453f70d844196d89d79848aa2e70a0bd8b38bf0f493cba1547bb3bca5e), [Nethereum](https://atlas.optimism.io/project/0x4a5e771af86cf1938056b43cddbf0018dca1376d578f631f7449fe10ac4958ed), [viem](https://atlas.optimism.io/project/0x6bd057da522918a4675396313ae33a2f2788a1ceeb3bd7ae228015e3eb317a7d), [web3.py](https://atlas.optimism.io/project/0xebe03c3d6d33cad60124b9b05ef6e2ff056293a1de3c5fa51dfbb90c86c14bf7), [Ape Framework](https://atlas.optimism.io/project/0xa0b16714baef75d97ec07fd48eaf42e79df92fe2a3c2d725d2388ede587ea54c), [Foundry](https://atlas.optimism.io/project/0x4562c0630907577f433cad78c7e2cc03349d918b6c14ef982f11a2678f5999ad), [Scaffold-ETH](https://atlas.optimism.io/project/0x154a42e5ca88d7c2732fda74d6eb611057fc88dbe6f0ff3aae7b89c2cd1666ab) and [Sourcify](https://atlas.optimism.io/project/0x51cda5996ef1a2ccd8fcf4ee5792337695599454c83eb1218c3ad4388dcb5bf5).

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/) 
* Celebrating [10 years of Solidity](https://x.com/solidity_lang/status/1942905422467551248).
* Join the [Language Design calls](https://meet.solidity.org) (Wednesdays 13:00 UTC) to learn about current priorities and upcoming changes.

#### [Vyper](https://vyperlang.org/)
* [Vyper EthCC workshop](https://github.com/vyperlang/vyper-workshop#readme): basic - deploy a token with Snekmate or advanced - Venom IR optimization.

### Client Libraries
#### [alloy](https://alloy.rs/)
* alloy [v1.0.17](https://github.com/alloy-rs/alloy/releases/tag/v1.0.17) - [v1.0.23](https://github.com/alloy-rs/alloy/releases/tag/v1.0.23).

#### [viem](https://viem.sh/)
* viem [2.31.7](https://github.com/wevm/viem/releases/tag/viem%402.31.7) - [2.33.1](https://github.com/wevm/viem/releases/tag/viem%402.33.1): includes [initial support for Flashblocks](https://x.com/_jxom/status/1946961084125954476) (up to 200ms transaction preconfirmations).

#### [web3.py](https://web3py.readthedocs.io/)
* web3.py [v7.12.1](https://web3py.readthedocs.io/en/latest/release_notes.html#web3-py-v7-12-1-2025-07-14).

#### [Web3j](https://docs.web3j.io/)
* [Two mentorships have started](https://blog.web3labs.com/web3j-mentorship-2025-meet-the-mentees/) and are currently ongoing.

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* Uniswap SDK [v0.3.0](https://github.com/ApeWorX/uniswap-sdk/releases/tag/v0.3.0): includes new solver implementation and `uni` CLI.

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.3.0-rc1](https://github.com/foundry-rs/foundry/releases/tag/v1.3.0-rc1) - [v1.3.0-rc4](https://github.com/foundry-rs/foundry/releases/tag/v1.3.0-rc4): includes `forge lint` support, time-based campaigns and coverage-guided fuzzing for invariant tests, table tests, fork test improvements for Reth clients and new EIP-712 features.

#### [Scaffold-ETH](https://scaffoldeth.io/)
* [create-eth v1](https://github.com/scaffold-eth/create-eth/releases) CLI launched.  (currently [v1.0.2](https://github.com/scaffold-eth/create-eth/releases/tag/v1.0.2)): more flexible/customisable, allowing extension developers to build more powerful extensions on top of Scaffold-ETH.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* New [Verification UI](https://verify.sourcify.dev): uses Sourcify APIv2 for clear error messages, onchain vs recompiled diffs and one-click GitHub issue reporting for failures.
* [Otterscan](https://x.com/otterscan/status/1944891894192070812) integrated Sourcify APIv2 to link revert traces to verified contract code.
* [8.5 million contracts verified](https://sourcify.dev/), includes 1.2 million on mainnet.

## Ethereum Layer 1

Ethereum [turns ten](https://etherscan.io/block/0). :cake:

### Gas limit increase
* Gas limit on mainnet can [safely be raised to 45M](https://ethpandaops.io/posts/gaslimit-scaling/), ~48% of validators are [signaling for 45M](https://gaslimit.pics/).

### History expiry
* [Partial history expiry](https://blog.ethereum.org/2025/07/08/partial-history-exp): nodes can run without pre-Merge data, saving 300-500GB in disk space.

### [Fusaka upgrade](https://forkcast.org/upgrade/fusaka) (target Q4 2025)

* Ideally upgrade mainnet before [Devconnect](https://devconnect.org/) (17-22 November) but timeline is tight.  
* Headliner is L2 scaling via [EIP7594 PeerDAS](https://forkcast.org/upgrade/fusaka#eip-7594) and [EIP7892 Blob parameter only upgrades](https://forkcast.org/upgrade/fusaka#eip-7892).
* [EIP7907](https://eips.ethereum.org/EIPS/eip-7907) to increase the contract code size cap was unfortunately removed, due to [unresolved complexity & timeline risks](https://ethereum-magicians.org/t/allcoredevs-execution-acde-216-july-17-2025/24770/4#p-60423-eip-7907-6).
* Current devnet: [Fusaka-devnet-3](https://fusaka-devnet-3.ethpandaops.io/) ([specs](https://notes.ethereum.org/@ethpandaops/fusaka-devnet-3)).

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target 2026)

* Glamsterdam [proposed headliners](https://forkcast.org/upgrade/glamsterdam#headliner-options) & [client team perspectives](https://forkcast.org/upgrade/glamsterdam#client-team-perspectives): 
  * [Stakeholder feedback](https://ethereum-magicians.org/t/soliciting-stakeholder-feedback-on-glamsterdam-headliners/24885) wanted on proposed headliners.
  * Execution layer client teams favor [EIP-7928 block level access lists](https://forkcast.org/upgrade/glamsterdam#eip-7928) (BALs) + repricing.
  * Consensus layer headliner short list: [EIP7732 ePBS](https://forkcast.org/upgrade/glamsterdam#eip-7732), [EIP7782 6-second slots](https://forkcast.org/upgrade/glamsterdam#eip-7782) and [EIP7805 FOCIL](https://forkcast.org/upgrade/glamsterdam#eip-7805).
* EIPs (non-headliners) can be proposed for inclusion via PRs to the [upgrade meta EIP](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-7773.md#proposed-for-inclusion).

---


Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate).**  Donations of all sizes are greatly appreciated.  




