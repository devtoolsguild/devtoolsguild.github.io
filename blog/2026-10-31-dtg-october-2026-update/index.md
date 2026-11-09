---
slug: devtoolsguild-october-2026-update
title: Dev Tools Guild October 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild October 2026 update

_**TL;DR**: Glamsterdam upgrade on Hoodi testnet postponed. Nethereum 7 full Ethereum SDK & node toolkit for .NET. Sourcify introduces Onay signing companion._

<!-- truncate -->

## Dev Tools Guild members

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* Solidity [0.8.38](https://www.soliditylang.org/blog/2026/10/22/solidity-0.8.38-release-announcement/): fixes low severity [Yul optimizer knowledge base stale bookkeeping bug](https://www.soliditylang.org/blog/2026/10/22/yul-optimizer-knowledge-base-stale-bookkeeping-bug/) (affects 0.8.19 - 0.8.37).  Faster Yul optimizer.  Warns when `swapn`, `dupn` or `exchange` are used as identifiers in Yul or inline assembly, as they are new opcodes in the Amsterdam EVM version ([EIP-8024](https://forkcast.org/eips/8024)).  
* [Core Solidity status update](https://www.soliditylang.org/blog/2026/10/14/the-state-of-core-solidity/): Core Solidity is a new solc frontend.  It adds a new type system with algebraic data types, pattern matching, generics, traits and compile-time evaluation.  Much of what is built into the compiler today gets moved into a standard library written in the language itself.  Syntax reworked to be closer to Classic Solidity and uses composition instead of inheritance.  Still a prototype and not ready for mainnet deployment.  Try the [playground](https://playground.solcore.soliditylang.org/).
* Argot: [ethdebug status update](https://www.argot.org/blog/2026-10-ethdebug), open format for compilers to describe their output to debuggers, with experimental ethdebug output in solc.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* [evm2](https://github.com/alloy-rs/evm2) is up to 2x faster than revm, built for custom EVMs and with clean extension boundaries.  [Reth v2.9.0](https://github.com/paradigmxyz/reth/releases/tag/v2.9.0) (execution layer client) replaced revm with evm2.

#### [Nethereum](https://nethereum.com/) (.NET)
* Nethereum [7.0.0](https://github.com/Nethereum/Nethereum/releases/tag/7.0.0): evolved into a full Ethereum SDK & node toolkit for .NET.  Interact through JSON-RPC, embed the EVM, execute and simulate transactions and blocks, connect to Ethereum over DevP2P, verify through a beacon light client and follow mainnet.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.57.2](https://github.com/wevm/viem/releases/tag/viem%402.57.2) - [v2.57.13](https://github.com/wevm/viem/releases/tag/viem%402.57.13).
* viem reached [1M daily downloads](https://x.com/_jxom/status/2106857746129936789).
* wagmi [v3.7.8](https://github.com/wevm/wagmi/releases/tag/wagmi%403.7.8) - [v3.7.9](https://github.com/wevm/wagmi/releases/tag/wagmi%403.7.9).

#### [Web3j](https://docs.web3j.io/) (Java)
* Web3j [v6.1.0](https://github.com/LFDT-web3j/web3j/releases/tag/v6.1.0): adds `CappedDynamicEIP1559GasProvider` with a max fee cap, fixes nested dynamic arrays (`string[][]`) and `maxPriorityFeePerGas` exceeding `maxFeePerGas`, plus ABI decoding performance improvements.

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* Ape [v0.8.53](https://github.com/ApeWorX/ape/releases/tag/v0.8.53): fixes custom error revert decoding, adds opt-in autosign for raw message hashes and `inject_poa_middleware` option for custom networks.

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.8.4](https://github.com/foundry-rs/foundry/releases/tag/v1.8.4): durable script recovery, native Base execution, external compiler adapters, integrated editor clients, expanded block-access-list tooling, substantial correctness and performance improvements.
* Foundry [v1.8.5](https://github.com/foundry-rs/foundry/releases/tag/v1.8.5) - [v1.8.7](https://github.com/foundry-rs/foundry/releases/tag/v1.8.7): patch releases, fixes Anvil mining for ready transactions left in the pool after a full block, dependency security fixes and compile cache regressions.

#### [Scaffold-ETH](https://scaffoldeth.io/)
* BuidlGuidl [Learning Lab](https://lab.buidlguidl.com) live: learn Ethereum basics, write Solidity and deploy contracts in your browser with an AI tutor.  First labs: Ethereum 101, Wallets & Crowdfunding.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Sourcify server [v4.1.2](https://github.com/argotorg/sourcify/releases/tag/sourcify-server%404.1.2) - [v4.2.0](https://github.com/argotorg/sourcify/releases/tag/sourcify-server%404.2.0): serves the OpenAPI spec, uses the Blockscout PRO API for creation transaction fetching and verification.
* [Onay](https://docs.sourcify.dev/blog/onay-local-signing-companion/) (prototype): second factor when signing transactions.  View only (holds no keys), independently fetches & verifies transaction details using a local light client, Sourcify verified source, ERC-7730 clear signing and local simulation.
* [Sourcify new look](https://x.com/SourcifyEth/status/2113569726936871252): one lookup box for verified contracts, 4byte selectors and ERC-7730 clear signing.
* Mainnet DAI [now an exact match](https://x.com/kaanuzdogan/status/2108282705406263807) on Sourcify, after recovering the 2019 build paths.

## Ethereum Layer 1

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* Sepolia testnet upgraded to Glamsterdam October 6, with a [200M gas limit](https://terencechain.com/writing/glamsterdam-scaling-results-ten-days-in/).
* [Glamsterdam on Hoodi testnet postponed](https://blog.ethereum.org/2026/10/22/glamsterdam-hoodi-delay) to further investigate interactions of [EIP-8037](https://forkcast.org/eips/8037) with mainnet contracts.  New schedule to be announced; [mainnet likely delayed until 2027](https://forkcast.org/calls/acde/248/).
  * ChainSecurity: [gas repricing changes assumptions](https://www.chainsecurity.com/blog/glamsterdam-gas/), gas based failure handling can change behavior after the upgrade, including post-call gas checks, revert based protection and fixed gas budgets.
  * ChainSecurity & Dedaub [due to report on the gas repricing investigation](https://forkcast.org/calls/acdt/102/) in November.
* Glamsterdam security vulnerabilities in scope for the [Ethereum bug bounty program](https://ethereum.org/en/bug-bounty).

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target 2027)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
  * Execution layer: [EIP-8141 Frame transaction](https://forkcast.org/eips/8141).
* Devnets renamed to layer names Heze (consensus) & Bogotá (execution):
  * [heze-devnet-3](https://forkcast.org/networks/heze-devnet-3/) adds [EIP-8198](https://forkcast.org/eips/8198) quick slots, set to 9 seconds.
  * [bogota-devnet-2](https://forkcast.org/networks/bogota-devnet-2/) adds [EIP-8298](https://forkcast.org/eips/8298) SETCODEFROM, [EIP-8151](https://forkcast.org/eips/8151) account code restricted ecRecover, [EIP-4758](https://forkcast.org/eips/4758) deactivate SELFDESTRUCT & [EIP-8253](https://forkcast.org/eips/8253) bump nonce of zero nonce storage accounts.

### Ethereum Foundation

* Cambridge research workshops:
  * [Post-Quantum Research Workshop](https://pq.ethereum.org/cambridge/) (2nd annual), October 10-12.
  * [Fast Finality Workshop](https://consensus.ethereum.foundation/cambridge/), October 13-15.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.