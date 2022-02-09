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

Vectis allows user to interact with DApps on the blockchain with the same amount of autonomy of a classic non-custodial solution, but with more flexibility by providing functionalities designed to serve the user.

Vectis also provides functions that allow businesses to satisfy regulatory requirements regarding support of users, transparency, separation of control duties and verifiability.

Vectis is an Open Source project under Apache-2.0 License, created by [nymlab](https:/www.nymlab.it)

## Motivation

We believe that the core values in designing Vectis will significantly improve user experience in the CosmWasm ecosystem.

- Custodial vs non-Custodial: Users should be provided with usability (recoverability, account freezing), security (key rotation) as well as the same level of autonomy as self custodial wallets.
- Gas provisioning: Service providers should be able to provide seemless experience (on-ramp / off-ramp / tx relaying) for users without users worrying about network gas costs.
- User acceptance: Regardless of the users proficiency of web3 or the DApps they choose to use, they should be provided with the same intuitive wallet experience.

Futhermore, being a part of the interWASM DAO community,
Vectis aims to provide a fully decentralised solution governed by a DAO where contract upgrades / feature development can reflect the needs of the community.

## Specification

### Work Completed

We already released the first version of the CosmWasm contracts (Factory and Proxy) [here](https://github.com/nymlab/vectis), implementing the three roles:

- User: the address that this wallet serves. The user has full control over the roles assignment and wallet operations.
- Guardians: the addresses appointed by the user to protect the user (via key recovery and/or account freezing and/or relayers rotation).
- Relayers: the addresses appointed by the user to allow for user's off-chain transaction signatures to be committed on-chain with gas and (optionally) certification of transactions.

### Proposed New Features

1. Ensure Vectis codebase is compatible with the Juno network cosmwasm version
1. Creating a DAO and integrate with Vectis for managing migration of contracts via [DAODAO](https://daodao.zone/)
1. Integration of the DApp frontend with Junotools to create the wallet interacting with the facroty contract and to manage the wallets (i.e. set/change guardians address, set/change relayers, check asset balances)
1. Provide an additional feature for a browser extension self custodial wallet (e.g. keplr) for users to use Vectis when interacting with other DApps on Juno
1. Deployment of Vectis to Juno
1. Deliver research and execution plan for deploying and managing Vectis DAO and wallets in candidate chains in the greater InterWasm ecosystem

## Team

NYMLAB Team, Belsy Yuen (@whalelephant), Arsen Kondratiev (@iorveth), Elena Chachkarova (@EChachGitHub), Egidio Casati (@egidiocasati)

## Grant

For the existing published work, we had invested in 10 weeks FTE[^1].

| New Features | Est. Time (in week FTE) |
| -----------: | ----------------------: |
|           1. |                     1.5 |
|           2. |                     1.5 |
|           3. |                     2.5 |
|           4. |                       3 |
|           5. |                       1 |
|           6. |                       2 |

Grant total: 21.5 weeks FTE for 5375Juno

[^1]: Full Time Equivalent
