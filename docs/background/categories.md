---
sidebar_position: 2
---

# Project Categories

The DevTools Guild comprises of a number of open-source, projects that are common goods for Ethereum. These projects are free software in the [GNU parlance](https://www.gnu.org/philosophy/free-sw.en.html) that can be utilised by developers building on Ethereum, without the requirement of any third-party commercial products or services to use them to their full potential.

They are common goods for developers on Ethereum in the truest sense of the word.

The Guild consists of four categories of developer tooling projects.

- [Client integration libraries](#client-integration-libraries)
- [Smart contract languages](#smart-contract-languages)
- [Development frameworks](#development-frameworks)
- [Standardisation public goods](#standardisation-public-goods)

These are outlined below.

## Client Integration Libraries

Client integration libraries provide developers using popular programming languages the ability to interact with the Ethereum blockchain. The types of interactions typically encompass querying the blockchain via Ethereum clients (nodes), the deployment of and transacting with smart contracts, and transacting with the Ether cryptocurrency. 

Programming languages in scope include those listed in [IEEE’s Spectrum Top Programming Languages Report](https://spectrum.ieee.org/top-programming-languages-2024) JavaScript/Typescript, Python, Java/Android, C#/.NET framework and Rust (Go is the one notable exception from the list, which lacks a dedicated RPC integration library. The geth codebase is typically used for this purpose). 

Ensuring that a diversity of different programming languages is available for developers working with Ethereum, isn’t just important for reducing friction for onboarding new developers, but also mitigating risk away from single points of failure for the network. If all developers were using the same programming language or development stack on Ethereum, identification of a critical vulnerability could have severe implications for the entire ecosystem, a scenario we are keen to avoid.

## Smart Contract Languages

Smart contract languages that are designed for developing smart contracts on Ethereum and smart contract development tools. 

As the universe of smart contract languages on Ethereum is small, it encompasses the most popular and actively maintained languages Solidity and Vyper, but also emerging smart contracts including Fe. 

This is due to the significant R&D overhead that is required to develop new smart contract languages.

The Ethereum Foundation recently span out a number of teams including Solidity, Fe and Sourcify, into the [Argot Collective](https://argot.org/blog/hello-world). As such, whilst a number of teams in Argot are supportive of the DevTools Guild, their short-term focus is on getting this new organisation off the group hence some members decided to hold off joining at this stage.

## Development Frameworks

Development frameworks encompass those specifically targeting developers developing smart contracts and DApps for Ethereum (this is unlike integration libraries which cater primarily for integrating with Ethereum clients using specific programming languages). 

They provide functionality for developers to create, test, deploy and interact with smart contracts and DApps on Ethereum. 

These development frameworks typically utilise client integration libraries to provide a simplified developer experience to develop DApps for Ethereum. However, a number of client integration libraries could also be considered development frameworks based on their full feature set.

## Standardisation Public Goods

These are common good services that provide standardised data for developers on Ethereum.

This includes smart contract verification service [Sourcify](https://sourcify.dev/) and the Ethereum metadata service [ethereum-lists](https://github.com/ethereum-lists).

## Future Categories

In addition to the above, the future categories for inclusion include:
- Smart Contract Libraries
- Further Standardisation Public Goods

## Smart Contract Libraries

Smart contract libraries provide reference and optimised implementations of smart contracts. These are public goods that are widely used by application developers and often integrated into developer frameworks to simplify the application development process.

Examples include [Open Zepplin’s Contracts](https://www.openzeppelin.com/solidity-contracts)  and [Snekmate](https://github.com/pcaversaccio/snekmate).

## Further Standardisation Public Goods

Further standardisation public goods that could be included within the Guild, include the [Ethereum Request for Comments (ERCs)](https://github.com/ethereum/ERCs) editors.

At the time of writing, the ERC repository had only just separated from the EIP repository with the group of editors responsible for the two repositories remaining the same. As a number of the active EIP editors are already members of the Protocol Guild, it would make sense to revisit this when there is a separation of duties between those editing EIPs versus ERCs.
