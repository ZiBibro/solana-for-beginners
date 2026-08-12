# Solana, explained to someone who has never heard of it

**Read it here: <a href="https://zibibro.github.io/solana-for-beginners/" target="_blank" rel="noopener">zibibro.github.io/solana-for-beginners</a>**

A plain-language explanation of Solana for people with zero crypto knowledge. There is also a <a href="https://zibibro.github.io/solana-for-beginners/Solana-explained-for-beginners.pdf?v=760bdd4428" target="_blank" rel="noopener">print-ready version</a> for reading away from a screen.

The page is one self-contained HTML file with no dependencies, no tracking and no build step. Every figure in it is read from a public Solana node in the reader's own browser at the moment they open it, including the interval between blocks, which the page times itself over a live six-second window.

## Where the numbers come from

| Claim | Source |
|---|---|
| Base fee of 5,000 lamports per signature, half burned | <a href="https://solana.com/docs/core/fees/fee-structure" target="_blank" rel="noopener">Solana fee documentation</a> |
| Agreement needs more than two thirds of stake, weighted by deposit | <a href="https://docs.anza.xyz/implemented-proposals/tower-bft" target="_blank" rel="noopener">Tower BFT</a>, <a href="https://solana.com/staking" target="_blank" rel="noopener">Staking</a> |
| Block interval, validator count, deposit concentration, fee distribution | Measured against `api.mainnet-beta.solana.com` on 12 August 2026 over 200 consecutive blocks and the full validator set, then re-read live by the page itself |
| Bitcoin's ten-minute target and 2009 start | `nPowTargetSpacing` and the genesis timestamp in <a href="https://github.com/bitcoin/bitcoin/blob/master/src/kernel/chainparams.cpp" target="_blank" rel="noopener">Bitcoin Core</a> |
| Outage durations | Solana Foundation incident reports, <a href="https://solana.com/news/02-06-24-solana-mainnet-beta-outage-report" target="_blank" rel="noopener">Feb 2024</a> and <a href="https://solana.com/news/04-30-22-solana-mainnet-beta-outage-report-mitigation" target="_blank" rel="noopener">Apr 2022</a> |
| SOL price used for the dollar conversion | Coinbase spot, cross-checked against Kraken on the same day |

## Running it locally

The published page above needs nothing at all. To run this copy instead, download `index.html` and open it in any browser. There is no build step and nothing to install.
