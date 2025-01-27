---
sidebar_position: 2
---

# Project Categories

The DevTools Guild comprises of a number of open-source, projects that are public goods for Ethereum. These projects are free software in the [GNU parlance](https://www.gnu.org/philosophy/free-sw.en.html) that can be utilised by developers building on Ethereum, without the requirement of any third-party commercial products or services to use them to their full potential.

They are public goods for developers on Ethereum in the truest sense of the word.

The Guild consists of four categories of developer tooling projects.

- [Client integration libraries](#client-integration-libraries)
- [Smart contract languages](#smart-contract-languages)
- [Development frameworks](#development-frameworks)
- [Standardisation public goods](#standardisation-public-goods)

These are outlined below.

## Client Integration Libraries

Client integration libraries provide developers using popular programming languages the ability to interact with the Ethereum blockchain. The types of interactions typically encompass querying the blockchain via Ethereum clients (nodes), the deployment of and transacting with smart contracts, and transacting with the Ether cryptocurrency. 

Programming languages in scope include those listed in [IEEE’s Spectrum Top Programming Languages Report](https://spectrum.ieee.org/top-programming-languages-2024) JavaScript/Typescript, Python, Java/Android, C#/.NET framework and Rust (Go is the one notable exception from the list, which lacks a dedicated RPC integration library. The [geth codebase](https://geth.ethereum.org/) is typically used for this purpose). 

Ensuring that a diversity of programming languages are available for developers working with Ethereum, isn’t just important for reducing friction for onboarding new developers, but also mitigating risk away from single points of failure for the network. If all developers were using the same programming language or development stack on Ethereum, identification of a critical vulnerability could have severe implications for the entire ecosystem - a scenario we are keen to avoid.

## Smart Contract Languages

Smart contract languages and compilers are specialized for creating arbitrarily complex smart contracts on Ethereum. 

The ecosystem primarily includes Solidity and Vyper, but also includes emerging smart contract languages such as Fe.

## Development Frameworks

Development frameworks encompass those specifically targeting developers developing smart contracts and DApps for Ethereum (this is unlike integration libraries which cater primarily for integrating with Ethereum clients using specific programming languages). 

They provide functionality for developers to create, test, deploy and interact with smart contracts and DApps on Ethereum. 

These development frameworks typically utilise client integration libraries to provide a simplified developer experience to develop DApps for Ethereum. However, a number of client integration libraries could also be considered development frameworks based on their full feature set.

## Standardisation Public Goods

These are public good services that provide standardised data for other developer tools, as well as app developers on Ethereum.

This category includes smart contract verification [Sourcify](https://sourcify.dev/) and the Ethereum metadata service [ethereum-lists](https://github.com/ethereum-lists).

# Future Categories

The current scope of the guild is limited to the above categories, but is up for discussion during the pilot phase. Examples of potential future categories may include smart contract libraries, ERC editors, and any other public good that meets the criteria of the guild.