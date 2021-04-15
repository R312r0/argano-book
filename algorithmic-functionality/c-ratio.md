---
description: How does collateralization work
---

# C - Ratio

Since Argano offers 2 algorithmic, dollar and bitcoin pegged tokens - **AGOUSD & AGOBTC** respectively, our team is going to use _Target Collateral Ratio_ and _Effective Collateral Ratio_ in order to stabilize the asset price and regulate their circulation according to the market supply and demand:

_Target Collateral Ratio_ `TCR` represents the C - Ratio to reach the desired asset price.

* The `TCR` is used in the asset **minting** calculation formula, both for AGOUSD & AGOBTC tokens.
* The `TCR` will be automatically calculated and established one time per hour, with the possible step of 0.25%. The maximum ratio couldn't be reached more than 6% per 24 hours.

{% hint style="info" %}
In the general sense, if the algorithmic token price is higher than the price of the stablecoin \(in the case of AGOUSD\) or the real bitcoin price \(in the case of AGOBTC\), the protocol will apply the lower collateral ratio to create new tokens. And vice versa, when the algorithmic token price is lower than it's needed, the protocol will increase the ratio automatically.
{% endhint %}

_Effective Collateral Ratio_ `ECR` is equal to the ratio between the total value of collateral assets and the total value of algorithmic tokens in circulation.

* The `ECR` is used in the asset **redeeming** calculation formula, both for AGOUSD & AGOBTC tokens.
* When the user wants to redeem his AGOUSD or AGOBTC tokens, he can be sure that for every number of both algorithmic tokens, he will receive the required number of collateral tokens and Share tokens to achieve an equivalent value in dollar terms.

$$
ECR =
$$
