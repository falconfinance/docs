---
description: >-
  Maintaing USDf’s peg through delta-neutral hedging, overcollateralization, and
  cross-market arbitrage.
---

# Peg Stability

Falcon employs delta-neutral hedging to balance the protocol's exposure to the collateral assets held. Falcon dynamically rebalances and neutralizes directional risk from the underlying assets, strengthening USDf's peg stability.&#x20;

In parallel, overcollateralization serves as a critical risk buffer. By requiring users to deposit more value than the amount of USDf minted, the protocol safeguards against price volatility in non-stablecoin assets. This ensures that every USDf remains fully backed by assets of equal or greater value, reinforcing the strength of the peg stability.

Together, these mechanisms allow Falcon to maintain synthetic dollar stability without relying on traditional banking infrastructure, even during periods of significant market fluctuations.

### Cross-market Arbitrage

Falcon also utilizes arbitrage of USDf across both centralized and decentralized spot markets to maintain the peg of USDf. This opportunity is also available to users, who are able to mint or redeem to profit from the price differences of USDf.

* If USDf is above peg (> $1.00):
  * KYC-ed Users can mint USDf at peg via Falcon, and sell them on external markets where USDf is trading above peg value.
* If USDf is below peg (< $1.00):
  * KYC-ed Users can purchase USDf below peg on external markets and redeem them for $1.00 worth of collateral per token via Falcon.

This incentivizes all parties to actively take part in stablizing USDf at its rightful peg value across various markets.
