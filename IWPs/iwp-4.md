---
iwp: iwp-4
title: Starrybot - Token Gating Communities in the Cosmos Ecosystem
description: A bot that detects Cosmos ecosystem tokens and NFTs, then promotes users with those tokens or NFTs in their wallets to different roles in Discord. 
author: Amber Case (@caseorganic), Amber Case <caseorganic@gmail.com>, Caseorganic (@caseorganic) Mike Purvis (@mikedotexe), Mike Purvis <mikedotexe@gmail.com>, Mikedotexe (@mikedotexe), Anselm Hook <anselm@hook.org>, Anselm Hook (@anselm) Anselm Hook (@anselm) and anselm (@anselm)
discussions-to: <https://starrybot.xyz/>
status: Draft
type: Grant
created: <date created on, in ISO 8601 (2021-12-15) format>
---

## Summary

StarryBot is set to build a flexible system that allows for communities to emerge and provide special access based on cw721 and cw20 tokens. 

This type of token gated system doesn't exist for Cosmos yet. We believe there is room for improvement in the web3 Discord bot space.

We're especially interested in supporting new projects like DAO DAO and making their work easier. 

## Motivation

The Cosmos ecosystem is a thriving community waiting for helpful token gated communities, and we'd like to help usher in the availability of niches in a community. Some niche groups may form around native tokens in the interchain world, or through fungible tokens, NFTs, or even particular aspects of NFTs.

With these new communities comes necessary gating to avoid spam, and the value-add of having subsets of folks given special permission to certain conversations.

There's a small handful of similar bots that don't serve the Cosmos ecosystem. Some of them suffer from poor user experience or — more concerningly — adopt patterns that may have security implications. We'd love to make a bot that improves on what's out there, as well as improving on security. 


We feel that important aspects of the ecosystem that have lower priority could get a jump start in progress. For instance, the ADR36 standard for signing offline messages might shake off some star dust and move forward from its current status in draft. 

The Keplr Wallet might also include some features related to offline signing if such a bot were to really utilize the zero-gas offline signing method designated in ADR36.

In short, we think the ecosystem would love it, use it, and it could have collateral improvements across other products and initiatives.

## Specification

We have four parts to StarryBot:

1. Static welcome website, inviting folks to add StarryBot to their Discord server.

2. Static verification subdomain website, where folks use Keplr to sign a message that goes to a backend. (https://github.com/starryzone/cosmos-webapp)

3. Discord bot + ExpressJS backend. The backend receives the offline signature, verifies it, and uses its access to the Discord token to add roles where needed. (https://github.com/starryzone/starrybot-discord)

4. Database — postgresql database with two tables tracking the conditions to add roles to users and members who need to sign custom Carl Sagan jibberish, matching them to their unique session token during verification.

Libraries used from the Cosmos ecosystem:

@cosmjs/amino
@cosmjs/crypto
@cosmjs/encoding
@cosmjs/stargate

As mentioned, we're using ADR36 to the best of our ability and the Keplr Wallet to sign offline messages. The messages are unique to each user, and are generated Carl Sagan ipsum.

## Team (Optional)

The authors of this proposal are the team:

- Amber Case
- Mike Purvis
- Anselm Hook

## Grant

2500 Juno tokens upon receipt of the grant. Delivered to Amber Case's Juno Grant Token Wallet.   

December: 

- Better configuration for the admin - a user clicks the emoji, or types in the one they want [each option is an emoji vote]
- Setup of additional tokens and roles
- Bot can tell you what version it is - “what version are you” in channel 
- Improved Website 
- Improved visual Design, logo, name 
- User flow: type !starry and the bot will respond telling you to go to your dms

January:

- Working bot, ready to test with DAO/DAO and future DAO/DAO projects 
- Improvements, code cleanup
- Documentation 
- Announcement and social media 

February:  

- Test with larger channels, with a specific focus on regenerative DAOs 
- Improve system, remove bugs 

March-Dec: 

- Grow the bot and help it to become a vibrant and friendly piece of the Cosmos ecosystem! 
