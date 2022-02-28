---
iwp: iwp-6
title: CW-Griptape
description: Bring GriptapeJS to Entire Cosmos Ecosystem as CW-Griptape
author: Stake or Die, (Luis Espinoza, David Rodriguez, Sandy Corsillo)
status: 
type: Grant
created: 2022-02-18
---

# Summary

GriptapeJS is a front-end development framework for applications that interact with smart contracts. Originally built for Secret Network on top of SecretJS (a Secret Network early fork of CosmJS), we propose to update and generalize the framework to be built on top CosmJS and rebranded as CW-Griptape.

In its current form, GriptapeJS is the framework of choice to build apps on Secret Network. The reason for this is that it handles all the common requirements that any developer needs to be immediately productive. Seeing the success on Secret Network we are eager and excited to bring the same framework to the entire Cosmos Ecosystem with CW-Griptape.

## Motivation

We have three main motivation for this project:

First: Our motivation is to unify front-end development practices across all of Cosmos with CosmWasm enabled. By doing this, developers will be able to choose the best chain for their use-case without worrying about compatibility.

Second: Through conversations with the InterWasm DAO, we realized that by acting as a layer between CosmJS and popular UI frameworks like React, Griptape insures applications using it don't have to worry about the development lifecycle of CosmJS. This creates a better experience for developers but also for CosmJS devs who can be freed to focus on building the best library possible. Breaking changes and new features can be added to CW-Griptape ahead of release therefore minimizing any disruption.

Third: We truly believe that Griptape is the best way to develop web3 applications. Thus, we want as many people as possible to use it and building CW-Griptape is the way to accomplish that.

## Specification

- CW-Griptape has the following objectives:
	- To abstract and provide a cohesive set of APIs to rapidly start building applications that connect to a CosmWasm enabled chains
	- To provide an entrypoint for CosmJS that centralizes the various APIs into one single package
	- To provide front-end specific utilities to help 3rd party integrations like Keplr
- Therefore, the CW-Griptape will include the following APIs:
	- Bootstrap API
		- An API that initializes and connects a front-end application to a CosmWasm enabled chain
	- Contracts API
		- An API that enables the creation of clients that can send messages and queries to smart contracts, by providing:
			- A contract blueprint interface
			- A set of built-in contract blueprints for CW specs 
			- A contract client creator
	- General utilities APIs
		- Error Handling Utilities
		- Re-export common CosmJS utilities (like @cosmjs/math)
	- APIs for extending and integrating 3rd party libraries through plugins
		- i.e. Keplr Integration
- Due to the mission critical nature of this framework, the libraries must be rock solid and built to evolve over time. Therefore we will build it using the following:
	- TypeScript
	- Jest (Full Test Coverage)
	- Circle CI (CI/CD Pipeline)
- Finally the developer experience with CW-Griptape must be world class, therefore we will make documentation and education a top priority through:
	- Continous (Release by Release), High Quality Docs
	- Tutorials

## Team

- Website: [https://griptapejs.com](https://griptapejs.com), [https://github.com/stakeordie](https://github.com/stakeordie)
- Luis Espinoza [https://github.com/luis-stakeordie](https://github.com/luis-stakeordie), [@luiseel_](https://twitter.com/luiseel_)
- David Rodriguez [https://github.com/David-Sod](https://github.com/David-Sod), [@lealdavid20](https://twitter.com/lealdavid20)
- Sandy Corsillo [https://github.com/the-dusky](https://github.com/the-dusky), [@the_dusky](https://twitter.com/the_dusky)

## Grant

6K **JUNO**

JUNO address: juno1zs0ag2mu95434uk3kped60za0naae3jl69ecc7

DA0 DA0 proposal: https://daodao.zone/multisig/juno1kkvct82dl0afp7lv2v6wv6emgltwqywxw2xu7p0l0vvl8rquv94s7e6xss/proposals/1
