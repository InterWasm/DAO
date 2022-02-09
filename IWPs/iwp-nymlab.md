---
iwp: iwp-TBC
title: Vectis - Smart Contract Wallet
description: Vectis is a smart contract wallet project to add functionality for users of DApps to manage their keys by allowing for recovery and account freeze, whilst preserving user control, and enabling relayer capability for gas provisioning.
author: NYMLAB Team, Belsy Yuen (@whalelephant), Arsen Kondratiev (@iorveth), Elena Chachkarova (@EChachGitHub), Egidio Casati (@egidiocasati)
discussions-to: https://github.com/nymlab/vectis
status: Draft
type: Grant
created: 2022-02-09
---

## Summary

Vectis allows user to interact with DAPPs on the blockchain with the same amount of autonomy of a classic non-custodial solution, but with more flexibility by providing functionalities designed to serve the user.

Vectis also provides functions that allow businesses to satisfy regulatory requirements regarding support of users, transparency, separation of control duties and verifiability.

Vectis is an Open Source project under Apache-2.0 License, created by [nymlab](https:/www.nymlab.it)

## Motivation

There are a number of Crypoto wallet dilemmas that we are trying to solve with Vectis:
- Custodial vs non-Custodial:
  security, resilience, trust
- Gas provisioning: on-ramp / off-ramp / token swap continuous hassle.
- User Acceptance: we must build for mass adoption, w/o giving up on security and privacy.

## Specification

We already released the cosmWasm contracts (Factory and Proxy) [here](https://github.com/nymlab/vectis), implementing the three roles:

- user: the address that this wallet serves. The user has full control over the roles assignment and wallet operations.
- guardians: the addresses appointed by the user to protect the user (via key recovery and/or account freezing).
- relayers: the addresses appointed by the user to allow for user's off-chain transaction signatures to be committed on-chain with gas and (optionally) certification of transactions.

We now plan to build:
- a dApp to create the wallet interacting with the facroty contract and to manage the wallet (i.e. set/change guardians address, set/change relayers, check asset balances)
- integration with a browser extension wallet (keplr) in order to set the user account and to use Vectis when interacting with other dApps
- Creating a DAO to manage upgrades of the factory contract

## Team(Optional)

Team behind the proposal.

## Grant

Amount, duration, terms of payment.
