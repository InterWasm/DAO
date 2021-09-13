---
iwp: iwp-1
title: CosmWasm IDE powered by Oraichain
description: An open-source project to simplify the development of WASM smart contracts on Cosmos-based networks: writing code, editing, testing, simulation, and deployment.
author: Tu Pham, Duc Pham, Diep Nguyen, Chung Dao, Thao Nguyen.
discussions-to: InterWasm DAO
status: Draft
type: Grant
created: 2021-08-25
---

## Summary

This proposal describes the motivation and goal of our "CosmWasm IDE powered by Oraichain" project in order to ask for a grant from InterWasm DAO. *The CosmWasm IDE powered by Oraichain is a hub for developers to write code, edit, build, simulate, test, and deploy WASM smart contracts on CosmosSDK-based blockchains through CosmWasm*. 

## Motivation

Oraichain is currently using the WASMD module to create different decentralized services such as price feed or VRF, and several AI Oracle services which utilize 100+ AI APIs for the community through the wasm smart contracts. We understand the variety of problems that a developer can have to deal with when developing such services: (1) time consumed in preparing working environments including building a test network; (2) lack of support libraries for deployment; (3) lack of simulation tools for monitoring interaction between multiple contracts and their states; (4) too simple unit tests which cannot cover in-production cases; (5) unfriendly hand-coding interface through CLI commands.

All of those obstacles have motivated us to build a hub for developers, called CosmWasm IDE. The IDE will provide developers with *a set of quick, convenient, and specific tools to fill the gap between ideas and development, and reduce the time consumption.* With readily available testing and developing environments and a high compatibility level to existing CosmosSDK-based blockchains, developers can easily write code, build, simulate, and deploy their smart contracts.

## Specification

- Use Gitpod template for server-side-development environment. Each user can have access to their workspace with fully customized VS Code extensions, terminals and other tools suitable to build and deploy wasm smart contracts.

- Integrate Keplr wallet extension to deploy the contracts onto different Cosmos-based networks.

- Build a Simulate VS Code extension and install it into the Gitpod template so users can simulate running the contracts as if they have deployed them onto the network.

- Simulate features:

    - Fast load & deploy & hot-reload contract without run WASMD
    
    - Fast call contract interface via command & switch contract, account
    
    - Fast Dapp development via Restful API & already integrated with Oraichain Studio
    
    - Print some debug information on screen
    
    - Do some bytecode check during wasm instanced
    
    - Watching storage db change on realtime
    
    - Dynamic calcuate and printing gas used during contract execute
    
    - Easy to test smart contract without input a json string

## Team(Optional)

Tu Pham, Duc Pham, Diep Nguyen, Chung Dao, Thao Nguyen.

## Grant

Expected amount: $35k

Duration: 2 months

Form of payment: $ATOM tokens