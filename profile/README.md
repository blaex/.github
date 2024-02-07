# Abstract
Blaex is a perpetual decentralized exchange (Perps Dex) protocol built on Blast, an ethereum layer two with native yield for ETH and stablecoins. The liquidity pool is formed by ETH and USDB, supplied by liquidity providers and locked in the vault contract. The liquidity is represented by Blaex Liquidity Index tokens (BLI) and simultaneously receives native yield from Blast. The providers are a counterparty to traders: if traders make profits, then providers make losses and viceversa. Transaction fees are shared among liquidity providers and BAEX investors, with a small portion allocated to the referral program.
# How it works
![image](https://github.com/blaex/.github/assets/102639451/097085fb-e83e-485d-91f8-00b0b9f31f57)


# Liquidity Provider
## Blaex Liquidity Index (BLI)
BLI is minted when liquidity providers deposit assets and burned when they withdraw. The value of BLI is calculated by dividing the total value of the Liquidity Vault by the number of BLI supplied. After minting, BLI will be automatically staked to receive real yield rewards from the protocol.
## Liquidity Assets (BTC, ETH, USDB)
The ideal ratio of the liquidity vault is 25% BTC, 25% ETH, and 50% USDB. In the event of any deviation from this ratio, minority swap mechanisms as well as profit distribution to traders in the form of tokens will be employed to stabilize the vault.
This ratio helps ensure that regardless of whether the market is bull or bear, the vault will maintain a relatively stable value.
## Blast Native Yield
In addition to the real yield received from the protocol, liquidity providers also receive Blast native yield through the appreciation of ETH and USDB in the pool.
# Perpetual Trading
## USDB collateralized & bUSDB
To open an interest, traders will use USDB as collateral. An intermediate token, bUSDB, will be minted and kept in Vault to represent the collateralized assets. After the distribution of Blast native yield to the Perps Vault, USDB will be evenly shared according to the bUSDB ownership ratio among traders.
## Profit & Loss
If a close position is profitable, the assets will be transferred from the Liquidity Vault to the Perps Vault to pay the trader. If the USDB ratio in the Liquidity Vault is below half, this portion will be paid in ETH or BTC.
Conversely, if trading results in a loss, the loss amount will be transferred from the Perps Vault to the Liquidity Vault.
## Fees
Transaction fees: 0.05% of trade size
Keeper fees: The fees for order execution and liquidation will fluctuate within the range of $1 - $2, depending on the gas fees of Blast.
# Swap
## Minority swap mechanism
The swap mechanism will be utilized to assist in balancing the Liquidity Vault. Tokens with distribution ratios below the threshold will incur higher fees, while tokens exceeding the distribution threshold will benefit from discounted fees, encouraging the return of the Vault to a balanced ratio.
## Fees
Swap fees: 
- 0.1% fee if input token has a higher ratio than default
- 0.5% fee if input token has a lower ratio than default 
# BAEX Token
Blaex Protocol’s ERC-20 native token
## Vesting
BAEX holders can lock up, or 'vest,' their BAEX tokens in the Vesting Pool to receive veBAEX, as well as yield from trader transaction fees. The longer the vesting period, the more veBAEX is minted, and the yield APR also increases.
In the initial years following the launch of the BAEX token, a portion of BAEX will be allocated to incentivize holders participating in vesting BAEX.
## Governance
Holders can use veBAEX to vote on proposals presented to the Blaex DAO, such as revenue distribution or decisions related to product development and ecosystem.
# Transaction Mining
We have designed a transaction mining program to attract more traders to the system and kickstart a positive feedback loop for traders and stakers.
## Leaderboard
Weekly and monthly, there will be a reward in BAEX tokens for traders with trading volume and for stakers involved in transactions.
## Transaction Fee Rebates
Traders reaching specific trading volumes will receive discounts on their trading fees.
## Referral Commission
Participants can receive fee discounts and earn rebates through the BAEX referral program, with a 5% discount for traders and up to 10% rebates for the referrer.
