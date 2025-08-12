---
description: Minting flow for Innovative Mint
---

# Innovative Mint

_**Disclaimer: The minimum amount required to initiate an Innovative Mint is USD$50,000 worth of eligible non-stablecoin collateral. Users should contact support@falcon.finance for more information or assistance with the process.**_

The Innovative Mint allows users to mint USDf by depositing non-stablecoin assets while maintaining limited exposure to potential price appreciation. Collateral is locked for a fixed term ranging from 3 to 12 months. At the time of minting, the users will have to set the following key parameters: tenure, capital efficiency level, the strike price multiplier. These parameter will determine the initial amount of USDf minted, the liquidation price, and the strike price.

The user's collateral is monitored throughout the lock-up period. Depending on price movements during or at the end of the term, there are three possible outcomes:

**1. If the collateral price drops below the liquidation price at any time during the term:**\
The collateral is liquidated to protect the protocol’s collateral backing. In this case, the user does not retain any claim to the original collateral. However, the user continues to hold the USDf that was minted at the start, which can be redeemed for supported stablecoins such as USDT or USDC.

**2. If the collateral price remains between the liquidation price and the strike price by the end of the term:**\
The user may reclaim the full collateral asset by returning the USDf originally minted. This allows the user to regain their asset while still having accessed to USDf liquidity during the term.

**3. If the collateral price rises and exceeds the strike price during the term or at maturity:**\
The collateral is exited. The user no longer retains any claim to the original asset. Instead, they receive an additional USDf payout, calculated as:&#x20;

$$
(Strike Price × Collateral Amount) − USDf Minted
$$

This additional USDf reflects the value of the collateral based on the agreed strike level, effectively capturing a predefined upside for the user in USDf terms.
