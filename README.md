# Farcaster On-Chain Verification ⛓️

Within the [Decentralized Intelligence Season 2](https://learnweb3.io/hackathons/decentralized-intelligence-season-2/), I have developed a system that ensures secure identity verification for **Farcaster** users participating in decentralized networks, enabling authentic identity to be recognized. The goal is to help build a trusted, Sybil-resistant environment for the community.

## Why?

- Sybil attacks caused over $900M in losses. 💸
- Threats to identity and humanity erode trust, necessitating security overhauls in decentralized systems. 🆔
- From Coinbase to Proof of Humanity, unified interoperable standards are crucial. 🔗

## What?

- Farcaster Frame built using Azle hosted on ICP that let Farcaster users easily use Ethereum Attestation Service on Arbitrum One to attest to their accounts. 🎫
- Gitcoin Passport is the first use case using the attestation as a primitive for Sybil resistance. 🛡️

## How?

- On-Chain Verifications: Use @eas_eth for secure verifications. 🏷️
- Community Trust: Incorporate @farcaster_xyz primitive to @gitcoinpassport. 🛂
- User-Centric Design: Use Farcaster Frames for usability and interactiveness to encourage adoption. 🖼️
- Decentralized: Leverage [Azle](https://github.com/demergent-labs/azle) and @dfinity ICP infrastructure for decentralizing computation. 🌐
- Interoperability and Efficiency: Use @arbitrum for smooth, cost-effective and secure integration. ⚡
 
## How does it work?

![Farcaster On-Chain Verify](https://github.com/Farcaster-On-Chain-Verification/.github/assets/1372744/120ad552-e0ec-4829-8614-1db14e656fda)

## What's next?

- Full decentralization: Eliminate backend dependencies by enabling direct network interactions for attestation creation and dispatch. This will help achieve a fully decentralized solution, building on the groundwork laid during the hackathon.

## Repositories
- **attestation-frame-azle**: Facilitate **Farcaster** account attestation using **Frames** on **ICP** decentralized infraestructure.
- **attestation-server**: Attest Farcaster accounts using **Ethereum's Attestation Service** on **Arbitrum One**.
- **gitcoin-passport**: **Gitcoin Passport** allows users to prove their identity through a secure, decentralized UI.

## Architecture

<img width="1657" alt="Architecture Diagram" src="https://github.com/Farcaster-On-Chain-Verification/.github/assets/1372744/055833fd-7e88-4a97-b240-b808cfbe5c6f">

### Components

- **USER**: Farcaster mobile or web user.
- **ICP**: [Internet Computer](https://internetcomputer.org/) canisters, interoperable compute units that bundle code and state, designed for internet-scale services. Used to host the Farcaster Frames frontend. In the future, it will be used to also store the attest backend serivce.
- **FARCASTER HUB**: [Farcaster](https://www.farcaster.xyz/) is a sufficiently decentralized social network. Farcaster Hubs are a distributed network of servers that store and validate Farcaster data.
- **FARCASTER FRAME**: [Farcaster Frames](https://docs.farcaster.xyz/learn/what-is-farcaster/frames) is used to turn any cast into an interactive app. Within this project, it allows users to verify their account directly on the app.
- **WARPCAST**: [Warpcast](https://warpcast.com/) is a decentralized social media platform built on Farcaster.
- **GITCOIN PASSPORT**: [Gitcoin Passport](https://www.passport.xyz/) deployed on [DigitalOcean](https://digitalocean.com/) with the Farcaster Stamp added. In order to verify an account, it checks the Ethereum Attestation Service GraphQL instance on Arbitrum One.
- **ARBITRUM ONE**: [Arbitrum One](https://arbitrum.io/) most dominant L2 on Ethereum by Volume and TVL used to store and query the EAS attestations through their smart contracts.
- **EAS**: [Ethereum Attestation Service](https://attest.org) is an infrastructure public good for making attestations onchain or offchain about anything.
- **NEYNAR**: [Neynar](https://neynar.com/) provides services to build on Farcaster. Used to validate requests on Frames.
- **VERCEL**: [Vercel](https://vercel.com/) is a centralized hosting provider. Due to some restrictions on building backends on the ICP decentralized infraestructure, it's being used as a backend server hosting.


