# Staking Credentials: Mitigating Decentralized Network Denial-of-Service with Proof-of-Stake Challenges

Systematic abuse of un-metered relay resources (subscriptions, notes storage) is one of the main robustness
concern of Nostr, a decentralized network protocol aiming to build a global censorship-resistant social community.

Additionally, systematic abuse is a source of concern for decentralized financial network such as the Lightning
Network, where local and network-level channels jamming have been extensively studied.

Staking Credentials aims to propose a framework to mitigate both class of denial-of-service with trust-minimized
and anonymous proof-of-stake challenges, satisfying the level of scarce resources consumed. The framework is inspired
by the IETF's Privacy Pass effort on new anonymopus internet challenges to protect web content delivery.

## Table of Contents

* [Design](#design)
* [Frequently Asked Questions](#frequently asked questions)
* [Resources](#resources)

## Design

Staking Credentials rely on two phases:
- credentials issuance
- credentials redemption

Credentials issuance happens between two roles: requester and issuer.

Credentials redemption happens between two roles: client and provider.

## Frequently Asked Questions

### What use cases could be covered by Staking Credentials ?

- nostr notes archiving
- LSP API services payment
- lightning routing hops liquidity locks up

## Resources

* [Staking Credentials Specification](https://github.com/civkit/staking-credentials-spec)
* [Unjamming Lightning: A Systematic Approach](https://eprint.iacr.org/2022/1454.pdf)
* [Privacy Pass: Bypassing Internet Challenges Anonymously](https://www.petsymposium.org/2018/files/papers/issue3/popets-2018-0026.pdf)
* [Privacy Pass IETF Working Group](https://datatracker.ietf.org/wg/privacypass/about/)
* [Mitigating Channel Jamming with Reputation Credentials: a Protocol Sketch](https://lists.linuxfoundation.org/pipermail/lightning-dev/2022-November/003754.html)
* [Solving channel jamming issue of the lightning network](https://jamming-dev.github.io/book/about.html)
