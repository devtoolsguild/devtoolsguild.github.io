---
slug: devtoolsguild-september-2026-update
title: Dev Tools Guild September 2026 update
authors: [abcoathup]
tags: [update]
---

# Dev Tools Guild September 2026 update

_**TL;DR**: Glamsterdam upgrade on Sepolia testnet October 6. Sourcify passes 50M verified contracts. Frame transactions Hegotá upgrade headliner._

<!-- truncate -->

## Dev Tools Guild members

### Smart Contract Languages
#### [Solidity](https://soliditylang.org/)
* Solidity [v0.8.37](https://www.soliditylang.org/blog/2026/09/10/solidity-0.8.37-release-announcement/): three important bugfixes (two low/medium: memory `bytes` element `delete` zeroing a whole word & via-IR memory slot collision with mutually recursive functions; one very low: misordered named custom error parameters in `require`), adds `block.slotnum` ([EIP-7843](https://forkcast.org/eips/7843)) to Amsterdam EVM version, planning stack shuffler for experimental SSA CFG pipeline, compiler performance and Yul optimizer improvements.  Removes experimental LSP mode & Generic Solidity prototype, deprecates Constantinople to Berlin EVM versions and the SMTChecker BMC engine.

#### [Vyper](https://vyperlang.org/)
* Vyper [v0.5.0b1](https://github.com/vyperlang/vyper/releases/tag/v0.5.0b1) (beta prerelease): adds access to immutables through `self`, conversions from flag to `bytes32` and a bottom type; Venom gains a `noinline` function annotation, reduced spilling for deep dups, redundant memory copy forwarding and range analysis for comparison folding.
* [End-to-end formally verified Vyper compiler grant](https://initiatives.thedao.fund/initiative/vyper-verified-compilation-and-secure-language-upgrades) live in TheDAO ETHSecurity Fund second round. Ethereum Foundation pledged $100K.  The grant funds a machine-checked proof that Vyper compilation preserves source semantics, with the goal of a public `--verified` compilation mode in the official compiler.

### Client Libraries
#### [alloy](https://alloy.rs/) (Rust)
* alloy [v2.4.2](https://github.com/alloy-rs/alloy/releases/tag/v2.4.2): adds Hegotá engine API methods, CCIP Read support, migrates ENS resolution to the Universal Resolver, chunked event query streams and Glamsterdam payload errors.
* alloy [v2.5.0](https://github.com/alloy-rs/alloy/releases/tag/v2.5.0): adds [EIP-8141](https://forkcast.org/eips/8141) Frame transactions, REST-SSZ Engine API wire types and execution witness encoding.

#### [viem](https://viem.sh/) (TypeScript)
* viem [v2.56.2](https://github.com/wevm/viem/releases/tag/viem%402.56.2) - [v2.57.1](https://github.com/wevm/viem/releases/tag/viem%402.57.1): v2.57.0 adds `createClientResolver` to lazily resolve and cache typed clients across configured chains; v2.57.1 adds [Open USD (OUSD) support](https://x.com/wevm_dev/status/2105356877077045319).
* Ox [v1.8.0](https://github.com/wevm/ox/releases/tag/ox%401.8.0): adds [EIP-8141](https://forkcast.org/eips/8141) Frame transactions.

#### [web3.py](https://web3py.readthedocs.io/) (Python)
* web3.py [v8.0.0](https://github.com/ApeWorX/web3.py/releases/tag/v8.0.0): migrates ENS resolution to the Universal Resolver, adds Python 3.14 support & CCIP-Read configuration, removes `LegacyWebSocketProvider` and drops Python 3.8 & 3.9.
  * [Major revisions of all snekcharmer libraries](https://x.com/ApeFramework/status/2094936296774861057) (Python packages stewarded by the ApeWorX Collective, including `eth-account`, `hexbytes` & `py-geth`): upgraded to a modern devtools stack (uv/ruff) and supporting all active versions of Python (3.10-3.14).  [Policy change](https://x.com/ApeFramework/status/2094936298842706009): libraries will only support active versions of Python.  Previously dropping a Python version required a major release.

### Frameworks and Dev Environments
#### [Ape Framework](https://docs.apeworx.io/ape)
* Ape [v0.8.52](https://github.com/ApeWorX/ape/releases/tag/v0.8.52): filter logs by multiple addresses.

#### [Foundry](https://getfoundry.sh/)
* Foundry [v1.8.3](https://github.com/foundry-rs/foundry/releases/tag/v1.8.3): expanded Glamsterdam support, including EIP-8037 state gas reporting (`Vm.Gas.gasStateUsed`) and `vm.getSlotNumber()`/`vm.rollSlot()` cheatcodes, `forge reinit`, Safe & token commands in cast, expanded invariant fuzzing & symbolic follow-up.  Default lints now high, medium & low severities.  (v1.8.2 was not published due to a rustls advisory.)
* forge-std [v1.17.0](https://github.com/foundry-rs/forge-std/releases/tag/v1.17.0): new `StdSecp256k1` library, state gas reporting and more reliable `stdStorage`.  `Vm.Gas` gains a field, use Foundry v1.8.3 or newer.

#### [Scaffold-ETH](https://scaffoldeth.io/)
* BuidlGuidl [Agents Arena](https://x.com/buidlguidl/status/2094842639350940102): 10 AI agents competed on 12 Solidity CTF challenges (the same CTF BuidlGuidl ran at Devcon).
* BuidlGuidl [Learning Lab Ethereum 101](https://lab.buidlguidl.com/labs/ethereum-101) (alpha): browser-based introduction to Ethereum.

### Standardisation Tooling
#### [Sourcify](https://sourcify.dev/)
* Sourcify server [v4.1.0](https://github.com/argotorg/sourcify/releases/tag/sourcify-server%404.1.0) - [v4.1.1](https://github.com/argotorg/sourcify/releases/tag/sourcify-server%404.1.1): stores metadata once per compilation and removes the block explorer creation transaction fetcher.
* [50M verified contracts](https://x.com/SourcifyEth/status/2100203098786402613) milestone, with the Parquet export 40GB smaller thanks to metadata.json deduplication.  The database [passed 1TB](https://x.com/SourcifyEth/status/2095100116105417170) earlier in the month.
* [Onay](https://x.com/argotorg/status/2104929593782309055) (local signing companion) by Sourcify is live in TheDAO ETHSecurity Fund second round.

## Ethereum Layer 1

### [Glamsterdam upgrade](https://forkcast.org/upgrade/glamsterdam) (target H2 2026)

* Headliners:
  * Consensus layer: [EIP-7732 ePBS](https://forkcast.org/eips/7732).
  * Execution layer: [EIP-7928 Block-level Access Lists](https://forkcast.org/eips/7928).
* [Glamsterdam activates on Sepolia testnet](https://blog.ethereum.org/2026/09/17/glamsterdam-testnet-announcement) October 6 (13:53:36 UTC).  Hoodi and mainnet dates to be decided.
* Reminder: [gas repricing impact](https://blog.ethereum.org/2026/08/24/glamsterdam-repricing-testing), check whether contracts are in the [affected mainnet contracts](https://ethereum.github.io/repricing-impact/affected-contracts.html) and test fixes on Sepolia (once upgraded to Glamsterdam).  Applications relying on fixed gas stipends, hardcoded gas limits or assumptions about remaining gas may need changes.

### [Hegotá upgrade](https://forkcast.org/upgrade/hegota) (target 2027)

* Headliners:
  * Consensus layer: [EIP-7805 FOCIL](https://forkcast.org/eips/7805) (Fork-choice enforced Inclusion Lists).
  * Execution layer: [EIP-8141 Frame transaction](https://forkcast.org/eips/8141).
* [frames-devnet-0](https://forkcast.org/networks/frames-devnet-0/) live.
* [Scoping of non-headliner EIPs](https://forkcast.org/upgrade/hegota/client-priority/?group=category) for Hegotá is ongoing.

### Ethereum Foundation

* [EF Protocol priorities](https://blog.ethereum.org/2026/09/07/protocol-priorities): north star is quantum resistant by December 2029.
* Will Corcoran [EF Protocol September update](https://x.com/corcoranwill/status/2104283555018731995).
* [EF Protocol cluster Reddit AMA](https://www.reddit.com/r/ethereum/comments/1wf48x3/ama_we_are_ef_protocol_pt_15_16_september_2026/) was held September 16.

---

Support Dev Tools Guild members by donating to **[donate.devtoolsguild.eth](https://devtoolsguild.xyz/donate)** on mainnet, Arbitrum, Base and Optimism.  Donations of all sizes are greatly appreciated.
