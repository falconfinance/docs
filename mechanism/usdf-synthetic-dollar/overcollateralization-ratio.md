---
description: >-
  Read how Overcollateralization Ratio is implemented for non-stablecoin crypto
  collateral when minting USDf in Falcon Finance.
---

# Overcollateralization Ratio

**Overcollateralization Ratio (OCR)**\
The implementation of an OCR helps to mitigate the impact of market slippage and inefficiencies, ensuring that each USDf minted by all non-stablecoin deposits is fully backed by collateral of equal or greater value. It indicates a user's total value of locked collateral relative to the amount of minted USDf.&#x20;

$$
\text{OCR} = \frac{\text{Initial Mark Price of Collateral} \times \text{Collateral Amount}}{\text{USDf Minted}}
$$

OCRs for each non-stablecoin collateral asset are dynamically calibrated based on the asset’s inherent market volatility, liquidity profile, market slippage and historical price behavior. This risk-adjusted approach ensures the protocol’s resilience against adverse price movements while optimizing capital efficiency for users.

Users should also note that the valuation of their collateral is directly tied to the prevailing market price and conditions at the time of collateral deposit. \
&#xNAN;_&#x46;alcon does not guarantee the stability or value of any assets and accepts no liability for any discrepancies or losses arising from market volatility or external factors influencing asset prices._

**Overcollateralization Ratio (OCR) Buffer**\
An OCR buffer is the portion of collateral retained by Falcon beyond the value of minted USDf. The buffer serves as a risk mitigation mechanism to safeguard the protocol against market fluctuations. The amount of collateral asset held as an OCR buffer is derived by:

$$
\text{OCR Buffer} = (\text{OCR} - 1) \times (\text{Collateral Amount})
$$

Reclaiming of the OCR buffer is based on market conditions at the time of claim.

* If the current market price ≤ initial mark price (of the collateral asset): Users will reclaim the full unit amount of the buffer
* If the current market price ≥ initial mark price: Users will reclaim the USD-equivalent value of the buffer based on the initial mark price
