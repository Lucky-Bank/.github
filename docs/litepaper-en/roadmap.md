---
icon: road-circle-check
---

# Roadmap

{% stepper %}
{% step %}
### 03 2025

* Mint $BANK
* Preparation of Litepaper
* Start of Public Sale
{% endstep %}
{% step %}
### 04-06 2025

* Backend Launch
* Peer-to-peer NFT Lending
* AMM Telegram Gifts Lending
{% endstep %}

{% step %}
### 07-09 2025

* Automated Peer-to-peer NFT Lending
* Peer-to-peer Jetton Lending
* Automated Peer-to-peer Jetton Lending
* Start of Marketing Campaigns
{% endstep %}

{% step %}
### 10-12 2025

* Development of an Indexer
* Integration of Lending into Lucky Market
{% endstep %}
{% endstepper %}

### Description

#### 1. Backend Launch
Currently, the application consists only of a dApp and a smart contract system, with interaction handled by tonconsole/tonapi. To speed up the application and add new features (such as user notifications, publishing new applications, and auctions), the launch of a backend with Telegram bot integration is planned.

#### 2. Peer-to-peer NFT Lending
This technology has already successfully existed in the TON network, but the niche is currently vacant. Loans will be issued in TON and USDT. The process consists of the following steps:
- The borrower sends an NFT for evaluation by bankers.
- Bankers send the borrower their offers regarding the loan amount, term, and interest rate.
- The borrower selects the best offer and receives the loan.

#### 3. AMM Telegram Gifts Lending
With the emergence of Telegram Gifts collections, which have an active market and a sufficiently large supply of NFTs, there is an opportunity to create AMM lending pools:
- The borrower tokenizes their floral gift by sending the NFT to a special contract, which in return issues 1 token corresponding to that gift collection.
- The borrower exchanges the received token in the AMM pool for TON (or USDT) at the current exchange rate.
- When the borrower needs to repay the loan, they perform the reverse actions: exchange TON for the token of the required collection and "redeem" their gift or any other available gift from the smart contract.
- The smart contract limits the available time for the borrower to exchange their token specifically for their NFT, thus achieving a certain "anonymity" of the gifts, with the main parameter being their floral value.
- In the dApp interface, all these processes may not be visible. The borrower simply sends the NFT, receives TON in return, and vice versa when repaying the loan on time.
- For investors, the AMM lending pool is practically no different from standard DEX liquidity pools, except that these pools have significantly higher exchange fees, and to replenish liquidity, it is necessary to deposit NFTs from the corresponding collections along with TON/USDT.
- If this type of lending proves sufficiently popular, it will be possible to spin it off into a separate service, and thus a new protocol — AMM NFT Marketplace — may emerge in the TON ecosystem.

#### 4. Automated Peer-to-peer NFT Lending
Thanks to our accumulated experience in developing pool-to-peer smart contracts, we have the opportunity to expand standard peer-to-peer lending, thereby simplifying and speeding up the loan process for borrowers:
- A banker creates their own liquidity pool and configures lending parameters for the NFT collections they are interested in.
- The borrower selects the best offer from pre-created ones and receives the loan.

#### 5. Peer-to-peer Jetton Lending
Similar to **2. Peer-to-peer NFT Lending**, lending against Jettons will be launched.

#### 6. Automated Peer-to-peer Jetton Lending
Similar to **4. Automated Peer-to-peer NFT Lending**, lending against Jettons will be launched.

#### 7. Start of Marketing Campaigns
Working with influencers, searching for project ambassadors, and using applications for task completion (planned launch of Lucky Promo).

#### 8. Development of an Indexer
The capabilities of third-party indexers (currently using tonconsole/tonapi) do not fully meet the needs of further development and implementation of new features, so it will be necessary to create our own indexer.

#### 9. Integration of Lending into Lucky Market
This feature will allow purchasing NFTs on credit, as well as listing pledged NFTs for sale.