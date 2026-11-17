# X-RAY open register samples

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24300931.svg)](https://doi.org/10.5281/zenodo.24300931)

Sample files of the register lists [X-RAY](https://x-ray.me) keeps on Web3's players: who is licensed, who is sanctioned, who holds the keys. Each file is the first 50 rows of one list, exactly as [x-ray.me/registers](https://x-ray.me/registers) serves it, with the list's date and its source's credit line in the head.

X-RAY is a map of Web3's organisations: who controls each one, where its capital sits and where it stands with regulators, every fact with its source.

## The lists

| File | List | Source |
|---|---|---|
| [`data/mica-casps.csv`](data/mica-casps.csv) | [MiCA-authorised crypto-asset service providers (CASPs)](https://x-ray.me/registers/mica-casps) | ESMA, interim MiCA register |
| [`data/mica-token-issuers.csv`](data/mica-token-issuers.csv) | [MiCA stablecoin issuers: e-money and asset-referenced tokens](https://x-ray.me/registers/mica-token-issuers) | ESMA, interim MiCA register |
| [`data/mica-white-papers.csv`](data/mica-white-papers.csv) | [Crypto-asset white papers notified under MiCA](https://x-ray.me/registers/mica-white-papers) | ESMA, interim MiCA register |
| [`data/mica-non-compliant.csv`](data/mica-non-compliant.csv) | [Entities EU regulators list as non-compliant with MiCA](https://x-ray.me/registers/mica-non-compliant) | ESMA, interim MiCA register |
| [`data/japan-crypto-exchanges.csv`](data/japan-crypto-exchanges.csv) | [Japan's registered crypto-asset exchange service providers](https://x-ray.me/registers/japan-crypto-exchanges) | Financial Services Agency of Japan |
| [`data/korea-vasps.csv`](data/korea-vasps.csv) | [Korea's reported virtual asset service providers (VASPs)](https://x-ray.me/registers/korea-vasps) | 금융정보분석원 (KoFIU) |
| [`data/ofac-crypto-sanctions.csv`](data/ofac-crypto-sanctions.csv) | [OFAC-sanctioned entities with listed crypto addresses](https://x-ray.me/registers/ofac-crypto-sanctions) | OFAC, SDN list (US Treasury) |
| [`data/us-crypto-bills.csv`](data/us-crypto-bills.csv) | [Crypto bills in the US Congress](https://x-ray.me/registers/us-crypto-bills) | Congress.gov (Library of Congress) |
| [`data/sec-filers.csv`](data/sec-filers.csv) | [Crypto companies that file with the SEC](https://x-ray.me/registers/sec-filers) | SEC EDGAR and Wikidata |
| [`data/l2-upgrade-keys.csv`](data/l2-upgrade-keys.csv) | [Who can upgrade each Ethereum L2: upgrade keys by rollup](https://x-ray.me/registers/l2-upgrade-keys) | L2BEAT |
| [`data/l2-stages.csv`](data/l2-stages.csv) | [Ethereum layer 2s by stage and value secured](https://x-ray.me/registers/l2-stages) | L2BEAT |
| [`data/superchain-chains.csv`](data/superchain-chains.csv) | [Superchain chains: the OP Stack networks in Optimism's registry](https://x-ray.me/registers/superchain-chains) | Superchain Registry |
| [`data/token-upgrade-keys.csv`](data/token-upgrade-keys.csv) | [Who can upgrade a token: upgrade and owner keys of token contracts](https://x-ray.me/registers/token-upgrade-keys) | Token contracts on chain |
| [`data/dao-governors.csv`](data/dao-governors.csv) | [DAO governance rules: quorum, proposal threshold, voting period and timelock](https://x-ray.me/registers/dao-governors) | Governor and timelock contracts on chain |
| [`data/lido-node-operators.csv`](data/lido-node-operators.csv) | [Lido node operators by stake](https://x-ray.me/registers/lido-node-operators) | Lido contracts on Ethereum |
| [`data/safe-harbor.csv`](data/safe-harbor.csv) | [Protocols that adopted the SEAL Safe Harbor agreement](https://x-ray.me/registers/safe-harbor) | SEAL Safe Harbor registry (on chain) |
| [`data/defi-exploits.csv`](data/defi-exploits.csv) | [DeFi exploits of the last 12 months](https://x-ray.me/registers/defi-exploits) | DeFiHackLabs |

## How to read a file

- The lines that start with `#` are the head: the list's title, its date and size, the source's credit line and the address of the whole list.
- Then one header row and up to 50 rows, comma-separated, UTF-8.
- A dash means the source states nothing there. It is never a zero.
- A row says no more than its source's file does. A list that a row left says nothing of why.
- Where a row names a player, the tie of that row to an organisation is X-RAY's, not the source's. The credit line says so.

## The whole list

Every list has its page, linked in the table above, with all of its rows and its cuts (by country, chain, stage and so on). An AI agent reads a list in full, and everything else X-RAY holds on a player, over the MCP server: [x-ray.me/docs/connect](https://x-ray.me/docs/connect).

## Updates

A workflow reads the sample files from x-ray.me every Monday and commits what changed. The date in a file's head is the day its source was last read.

## Sources and licence

The facts belong to their sources and stay under each source's own terms. Each file's head carries the credit line the source asks for:

- ESMA, interim MiCA register. Reproduction is authorised provided the source is acknowledged.
- Financial Services Agency of Japan, the registers of exchange service providers, under the Public Data License 1.0: "Source: Financial Services Agency website (https://www.fsa.go.jp/en/regulated/licensed/index.html)". The files here are edited from that content by X-RAY.
- Korea Financial Intelligence Unit: 출처: 금융정보분석원(KoFIU), kofiu.go.kr.
- OFAC's SDN list, SEC EDGAR and Congress.gov: works of the United States government, in the public domain.
- Wikidata: CC0.
- L2BEAT: MIT. Superchain Registry: MIT © 2023 Optimism. DeFiHackLabs (SunWeb3Sec): Apache-2.0.
- Token, governor, Lido and SEAL Safe Harbor contracts: read on chain over public RPC.

What X-RAY adds, which is the selection, the wording of the rows and the ties to players, is under [CC BY 4.0](LICENSE). Credit: **X-RAY, https://x-ray.me**.

No source listed here endorses X-RAY or these files. The files are information, not legal advice, and come without warranty: for a decision that depends on a register, read the register.

## Cite

X-RAY. *X-RAY open register samples*. Zenodo. https://doi.org/10.5281/zenodo.24300931

The DOI names every version; each release is a dated snapshot with a DOI of its own.

## Contact

[x-ray.me/contact](https://x-ray.me/contact)
