---
description: >-
  Redemptions in Falcon Finance: how it works & differs from unstaking. Classic
  redemptions for stablecoin collateral & claims for non-stablecoins.
---

# Redemptions

Besides selling USDf on external markets, users looking to exit their USDf positions have the option of initiating redemptions on Falcon. Redemptions are split into two types - a classic redemption and a claim. This is based on the type of asset a user is receiving for his USDf, with both forms of redemptions being subject to a 7-day cooldown period. Users will only receive their assets after this period, in which their redemption requests are processed.

The cooldown period is implemented to ensure the health of Falcon and its reserves, providing a sufficient window of time for Falcon to withdraw users' assets from its active yield generation strategies.\
&#xNAN;_**This is not to be confused with unstaking, where users can unstake their sUSDf and receive USDf in return immediately.**_

### Classic Redemptions (Stablecoins)

Classic redemptions involve users exchanging their existing USDf for one of Falcon's supported stablecoin options (e.g., USDC, USDT).&#x20;

Refer to the [Redeem](../resources/quick-app-guide/navigating-the-swap-tab/redeem.md) section for further details on redeeming USDf for stablecoins.

### Claims (Non-Stablecoins)

Claims, on the other hand, involve users exchanging their existing USDf for non-stablecoin positions that they previously locked to mint USDf.&#x20;

For users of [Classic Mint](../resources/quick-app-guide/navigating-the-swap-tab/classic-mint/), this process enables users to recover the [overcollateralization buffer](usdf-synthetic-dollar/overcollateralization-ratio.md) applied during the initial minting. Upon claiming, users may choose to receive their assets in one of three formats: the original collateral asset, USDT, or a combination of both.

For users of [Innovative Mint](usdf-synthetic-dollar/usdf-minting-mechanisms/innovative-mint.md), claims can be made only after the tenure of collateral has matured.&#x20;

Once the tenure has matured, to reclaim the original non-stablecoin collateral, users must repay the amount of USDf initially minted. Full recovery of the collateral is possible only if the position was not liquidated or exited due to the asset price reaching the predefined strike level during the term. Users will have a 72 hour window to recover the full collateral from the tenure maturity date.

Refer to the [Claim](../resources/quick-app-guide/navigating-the-swap-tab/claim.md) section for further details on redeeming USDf for non-stablecoin assets.

