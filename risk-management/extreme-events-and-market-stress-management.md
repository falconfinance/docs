# Extreme Events & Market-Stress Management

Cryptocurrencies are among the most volatile assets which may demonstrate incredible\
price movements such as 500% growth within a day and 90% price drop within an hour.\
Bitcoin demonstrated such behavior earlier but with time it demonstrates less extreme\
behaviour while most altcoins still are known for this. For example, MANTA has collapsed by\
more than 90% within just an hour recently which triggered massive liquidations and losses.

### How Falcon Finance Manages Extreme Events&#x20;

Falcon Finance treats extreme events as a first-order risk and employs disciplined, multi-layered controls to minimize losses in both stressed and normal market conditions.

Falcon Finance employs delta neutral strategies to minimize directional exposure while capturing basis and funding opportunities. The approach is straightforward and follows clear execution rules:

* With stablecoins: Falcon purchases spot exposure in the target altcoin and stake it where appropriate, then open an offsetting short position in the corresponding perpetual sized to the marked spot exposure.
* With altcoins: Falcon sells the spot position to neutralize risk and open an offsetting long position in the corresponding perpetual when basis or funding conditions make the trade attractive. This often leads to large profits in case of large price differences between spot and perps\
  or/and in case of negative funding rates.

### Risk Controls for Extreme Market Conditions&#x20;

During extreme events involving rapid price increases, the risk of liquidation increases\
drastically. In order to avoid such scenarios, Falcon Finance performs the following:

1. Connect all strategies that trade spot and perpetuals into a single monitoring system that enforces near-zero net delta across the total position.
2. As soon as price exceeds a given threshold, the systems automatically sell spot and closes perpetuals positions.
3. Even when staking yields are highly profitable, we maintain at least 20% of spot holdings on exchanges and available for immediate sale, allowing us to liquidate a significant portion of the position without delay.
4. If an extreme event happens, Falcon removes spot coins from staking immediately or\
   when it’s possible. Falcon aim to negotiate zero lockup period for staking or any\
   other DeFi activities.
5. Falcon employs machine learning models that continuously analyze market data and flag potential extreme events ahead of broader market recognition, allowing for rapid intervention.
6. Falcon sets maximum altcoin position sizes so that the majority of any position can be unwound within a day.



During sharp declines in spot prices, Falcon prioritizes management of perpetual positions to ensure they can be closed or resized quickly and to prevent adverse funding from accumulating. Execution algorithms derived from high frequency trading practices enable rapid order placement and cancellation, allowing efficient exits even under stressed conditions.

In addition, depegging of other stablecoins is treated as a distinct scenario. Falcon’s risk monitoring system surfaces abnormal peg deviations early, ahead of broader market recognition. Depending on the configured risk posture, Falcon either exits exposure to the affected stablecoin with minimal realized loss, typically under a few basis points, before a full depeg develops, or maintains a hedged stance and waits for the peg to restore.
