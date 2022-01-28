---
iwp: iwp-5
title: SecurityDAO
description: incentivized CosmWasm audits, security tooling and education for Cosmos / IBC
authors: Barton Rhodes (@bmorphism), Paul Wagner (@devcubed)
status: Review
type: Grant
created: 2022-01-26
---
## Summary
SecurityDAO was formed on December 17th, 2021 at the RadicalXChange Unconference in Denver, Colorado. 🏔

We are a group of developers, security engineers, and fellow travelers united by:

- our critical examination of the distributed systems for "rough consensus"
- our dismay at the inconsistent application of well-established security practices in "web3"
- our knowledge / skills and feeling compelled to make a difference

Most of all, we do not wish to see the transformative aims of the radical movements that place their trust into on-chain governance and value exchange be thwarted because security came as an afterthought.

## Motivation
The focal point for the initial members in our DAO is the choice of Cosmos / IBC - sovereign chains with interoperable smart contracts as the backbone for the Pluriverse, one that can _actually_ scale with growing adoption. In it, the additional memory safety guarantees that come with Rust / `CosmWasm` and the Actor model for contract interactions eliminate entire classes of bugs plaguing other chains and [rekt.news leaderboard](https://rekt.news/leaderboard/); still, being able to compile your CosmWasm smart contract in itself is not a guarantee that the logic it implements is correct. Most projects built with CosmWasm do still require review, the space of threats around IBC is still being explored and explicit incentives for operating and securing relayer infrastructure for IBC are yet to be defined. It is still early days and there is no shortage of security work to be done, however, there are relatively few contributors who are qualified, available, or brave enough to do it.

The immediate priority for the DAO will be to improve the security posture of the projects headed for Junø mainnet, and InterWasm funding will help SecurityDAO incentivize contributors, begin development of open-source Cosmos ecosystem security tooling, as well as cover any expenses associated with carrying out of the initial audits and other administrative costs.

Security innovation is a key differentiator for Cosmos / IBC and the goal for SecurityDAO is to be the first contributor-governed alternative to the traditionally structured audit shops operating in the ecosystem.

## Upcoming audits

Initial set of targets:

- [DAO DAO](https://daodao.zone)
- [WasmSwap](https://github.com/Wasmswap)
- [cw-vest](https://github.com/ben2x4/cw-vest)

## CosmWasm security tooling
The InterWasm funds will be used by SecurityDAO to germinate, develop, and open-source the following:

### CosmWasm fuzzer
Fuzz-testing smart contracts allows for discovery of issues outside of the test cases thought up and implemented by the developer. In practice, it will mean fulfilling several sub-bounties that implement AFL fuzzing for smart contract intercations for `CosmWasm` specifically.

https://github.com/rust-fuzz/afl.rs

The characteristics of different contracts as far as their time to run fuzz tests, termination, and failure modes of the testing procedure. It is our goal to make available the fuzz testing tooling that will allow CosmWasm developers discover issues, e.g. missing integrity checks, through encountering of pseudorandom inputs outside of the ordinary tests.

### Cross-chain audit protocol with skin in the game
In many ways, the predominant smart contract audit today is the same old SaaS / web2 model we've seen before.
When it comes to the terms of engagement, final deliverable format, or how the parties think about responsibility stemming from audit services, there is no fundamental difference between a canonical vendor like Trail of Bits auditing [a k8s component](https://github.com/etcd-io/etcd/blob/main/security/SECURITY_AUDIT.pdf) or a [self-sovereign identity protocol](https://github.com/mykeylab/keyid-eth-contracts/blob/master/reports/Trail%20of%20Bits%20Verification%20Report%20for%20MYKEY(2020-09-14).pdf).

A typical smart contract auditor today is paid per engagement at a rate significantly less than the value of the targets being audited. The liability for the audit is limited and in case of their client being hacked, the damage to the auditor is predominantly reputational.

At SecurityDAO, we are fundamentally uninspired by the way web3 / DeFi audits are done today. We build what we build because we share in the values of the protocols, DAOs, L-1s, and individuals that we help, we want to help bring the outcomes in the world that they seek (and yes, sometimes our prospects' values won't align with ours and we will vote to say "no"). If our contributors make mistakes, we will hurt also.

This shared ownership over the outcomes, good or bad, is the fundamental principle of web3 and needs to be emulated, especially wherever the stakes are high. To that end, we want to build a protocol for on-chain audits with automated incentives to get it right! Our goal for the protocol is to allow any "pod" of security frens anywhere to have a structured way of joining forces for an audit. The scope of our ambition is to engineer incentives to capture the entire addressable market for audits and make the corporate transactional audits a relic from 2021.

CosmWasm operating across chains and even ecosystems (Evmos, Gravity Bridge) offers unique flexibility in developing a protocol that could allow for automated settlement to take place, even if the original chain is pwned / forked, in a variety of tokens as long as the chain is in IBC / using AMMs to ensure the token is liquid.

### Other activities and tooling
In the course of carrying out the CosmWasm work, we expect to develop or improve the following.

- IBC labnets - configuration-driven simulations of cross-chain scenarios enncountered by Cosmos / IBC
- responsible disclosure - work out solutions and processes by which to incentivize discovery and disclosure of issues discovered at all layers of proof-of-stake chains


### Art and Education
In order to allow for continuous fundraising and the recording of impactful security events in Cosmos / IBC history, the DAO will begin minting ([when it becomes available](https://mirror.xyz/stargazezone.eth/Ozp8kRUsnGyN46lV3-5I57tB_LxRtlyTN176yL_T0f8)) a weekly `SG-721` NFTs that point at specific transactions of significance from any of the L-1 chains in Cosmos or otherwise, protocols, DAOs being audited, and any adjacent artifacts. In cases where the significant event is a fork or other artifacts that are no longer on-chain for the current height, the NFT will point to an index / sketch of the incident in `Arweave`.

## Governance

- private `junod` chain + gov contract w/ DAO DAO UI for tactical / sensitive SecurityDAO decisions
- public liquid DAO to for security education - meetups, conferences, blogposts, CTFs, and engagement with the community through the DAO's [Pluriverse space](https://invasive.dao.surgery)

## Grant

Amount: `9999 $JUNO`

Wallet: `juno1j37vjp9pcsyvk2ssklx3l7jhqwvfmm7p3frfd6`
