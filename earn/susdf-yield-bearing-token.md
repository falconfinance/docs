---
description: >-
  Read how sUSDf works: yield-bearing token, minted when USDf is deposited &
  staked into Falcon’s ERC-4626 vaults, based on the sUSDf-to-USDf value.
---

# sUSDf (Yield-Bearing Token)

sUSDf is the yield-bearing version of USDf, and the other half of Falcon's dual token system. Minted when USDf is deposited and staked into Falcon's ERC-4626 vaults, the amount of sUSDf received by users is calculated based on the prevailing sUSDf-to-USDf value.

$$
\text{Current sUSDf-to-USDf Value} = \frac{\text{Total USDf Staked} + \text{Total Rewards}}{\text{Total sUSDf Supply}}
$$

$$
\text{sUSDf Minted} = \frac{\text{USDf Staked}}{\text{Current sUSDf-to-USDf Value}}
$$

Following the above formulas, the sUSDf-to-USDf value at any point of time reflects the total supply of sUSDf relative to the total USDf staked and accumulated yield in USDf, and is a gauge for cumulative yield performance. As such, the value of sUSDf increases over time as Falcon accrues yield through strategies such as positive & negative funding rate spreads, and altcoin staking.&#x20;

### ERC-4626

[ERC-4626](https://ethereum.org/en/developers/docs/standards/tokens/erc-4626/) is a standard for tokenized vaults on EVM-compatible blockchains, designed to enhance interoperability and composability within DeFi. By providing a standardized API, this standard also ensures the unification and optimized management of yield-bearing assets.

Falcon's sUSDf utilizes the ERC-4626 vault standard for its yield distribution mechanism. The standard is crucial in ensuring a transparent and efficient mechanism for distributing yield to users who stake their USDf, while streamlining the process. This also supports integration of sUSDf into various DeFi applications in the future, enhancing overall user experience and security.

Refer to the [Classic Yield](../resources/quick-app-guide/navigating-the-earn-tab/classic-yield/) section for details on the USDf staking process.
