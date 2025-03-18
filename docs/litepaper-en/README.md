---
description: Lucky Bank — NFT Collateral Lending
icon: rocket-launch
---

# Litepaper \[EN]

## **1. Introduction**

**Lucky Bank** is an innovative platform for NFT collateral lending, offering **high-quality service**, **flexible terms**, and **unique opportunities** for NFT owners and investors. The service was launched on December 6, 2024, and currently implements the following features[^1]:

#### 1. Pool-to-peer NFT lending
Automatic perpetual loans in TON with flexible settings for loan amount and repayment terms.

#### 2. Liquidity vault
Passive income for investors who deposit their funds into the automatic lending pool.

#### 3. USDT lending
We are the first in the TON network to implement a smart contract system that allows pool-to-peer lending in USDT against NFT collateral (along with a corresponding USDT liquidity pool).

#### 4. Auctions
Collateral NFTs from overdue loans are automatically sent to auction.

---

## **2. The Problem**

> _Monopolies are very harmful to economic development, if only because they set high prices for not always high-quality products. And of course, in the end, they "cannibalize" themselves, their own technologies._
> Jean Tirole
>
> _Every monopoly... inevitably breeds stagnation and decay._
> V. I. Lenin

Historically, NFT collateral lending in the TON network has been monopolized. With the emergence of Krediton Lending Tool in the lending market (more details in the [Market Analysis](market-analysis.md) section), the market could only respond by undercutting lending rates. The sole player dictates high fees and inflexible terms, and there is no information about risks (closed smart contracts)[^2].

In this situation, no new DeFi tools related to NFT collateral lending are emerging, which, in turn, hinders the development of the TON ecosystem as a whole.

---

## **3. The Solution**

After assessing the volume of the pool-to-peer NFT collateral lending market, we decided not to enter into direct competition with existing players, as this would inevitably lead to "price wars" and ultimately benefit no one. Therefore, as part of Lucky Bank's further development, we plan to occupy free niches and attempt to create new DeFi tools utilizing NFTs. The following main features are planned for implementation in the near future:

#### 1. Peer-to-peer NFT lending
This technology has already successfully existed in the TON network, but this niche is currently vacant. Loans will be implemented in TON and USDT. The process consists of the following steps:
- The borrower sends NFTs for appraisal to bankers.
- Bankers send the borrower their offers regarding loan amount, term, and interest rate.
- The borrower selects the best offer and receives the loan.

#### 2. Automated Peer-to-peer NFT lending
Thanks to our accumulated experience in developing pool-to-peer smart contracts, we have the opportunity to expand standard peer-to-peer lending, thereby simplifying and speeding up the loan process for borrowers:
- A banker creates their own liquidity pool and configures lending parameters for the collections they are interested in.
- The borrower selects the best offer from pre-created ones and receives the loan.

#### 3. AMM NFT lending
With the emergence of Telegram Gifts collections, which have an active market and a sufficiently large supply of NFTs, there is an opportunity to create AMM lending pools:
- The borrower tokenizes their floral gift by sending the NFT to a special contract, which in return will issue 1 token corresponding to that gift collection.
- The borrower exchanges the received token in the AMM pool for TON (or USDT) at the current exchange rate.
- When the borrower needs to repay the loan, they perform the reverse actions: exchange TON for the token of the required collection and "redeem" their gift or any other available gift from the smart contract.
- The smart contract limits the available time for the borrower to exchange their token specifically for their NFT, thus achieving some "anonymity" of the gifts, with the main parameter being their floral type.
- In the dApp interface, all these processes may not be visible. The borrower simply sends the NFT, receives TON in return, and vice versa when repaying the loan on time.
- For investors, the AMM lending pool is practically no different from standard DEX liquidity pools, except that these pools have significantly higher exchange fees, and to provide liquidity, one must deposit NFTs of the corresponding collections along with TON/USDT.
- If this type of lending becomes sufficiently popular, it will be possible to spin it off into a separate service, and thus a new protocol — AMM NFT Marketplace — may emerge in the TON ecosystem.

For more details on the development and roadmap, please refer to the [Roadmap](roadmap.md) section.

---

## **4. Financial Model**

- **Revenue Sources**:
  - Loan issuance fee (competitive rates, no undercutting).
  - Loan interest rate (market conditions).
  - Penalties for late payments.
  - P2P lending fee.
  - AMM lending fee.
- **Expenses**:
  - Platform development and maintenance.
  - Marketing and user acquisition.
  - Reserves for replenishing the automatic lending pool.
  - Reserves for replenishing the AMM lending pool.

---

## **5. Tokenomics**

To implement the planned development of Lucky Bank, additional investments will be required. Investments will be attracted through the issuance of the project's token.

Ticker: _**$BANK**_\
Total supply: **100,000**\
Master contract address: [**EQB1399hPqWDdupmVw43dKBEgYgsEtoliVGsfpchiHC-BANK**](https://tonviewer.com/EQB1399hPqWDdupmVw43dKBEgYgsEtoliVGsfpchiHC-BANK)\
Owner: _**Revoked**_\
ICO format: _**Quadratic curve. Start at 1 USDT. End at 3 USDT.**_

For more details, please refer to the [Tokenomics](tokenomiks.md) section.

---

## **6. Benefits for Token Holders**

- **Staking.** A portion of the service fees will be distributed among token holders through staking.
- **Increased passive income.** Token holders will have access to lending pools with higher utilization rates (and thus higher APY).
- **Access to p2p.** Lending for incoming applications will be available only to token holders. The service fee will also depend on the number of tokens held.
- **Access to the private bankers' chat.** A private chat accessible to people interested in lending against liquid/beautiful NFTs that also interest them. Communication, advice, and insights.

---

## **9. Team**

- **CEO**/**CTO**: Pavel.\
  Telegram: [@x1y1x3](https://t.me/x1y1x3)\
  Full-stack programmer (general programming experience since 1994).\
  Main specialization/work — f2p games for social networks (since 2009).\
  Experience in TON smart contract programming (since 2023).\
  Implemented: NFT collateral lending smart contract system for TON Lombard bot, Lucky Wallet container contract (semi-finalist of TON Open League Hackathon 2024), and Krediton Lending Tool (also made it to the top 100 projects of the hackathon).
- **CM**: Soon.

---

## **10. Conclusion**

**Lucky Bank** offers **an alternative to the monopolist**, providing users with **high-quality service**, **transparency**, and **unique opportunities**. We aim to become **the market leader** by using innovative technologies and offering users more freedom and choice. The $BANK token will play a key role in the ecosystem, providing utilities and incentives for participants.

[^1]: Based on Krediton Lending Tool (KLT) — a decentralized dApp (fully implemented on smart contracts without server-side involvement) B2B service https://t.me/krediton. 
[^2]: KLT loan smart contract is verified, Bugbounty announced https://t.me/krediton_official/18