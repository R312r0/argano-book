---
description: Redeeming explanation
---

# Redeeming AGOBTC & AGOUSD

The process of redeeming implies returning the collateralized tokens AGOUSD / AGOBTC back to the protocol and, in return, receiving back the user's collateral assets and the required amount of share tokens CNBTC / CNUSD, which are required to reach desired equality. This in turn means that with every $1 value, users will receive part of collateral together with the part of share tokens.

Redeeming formula works based on the Effective Collateral Ratio \(`ECR`\) and applies for both algorithmic tokens:

$$
Collateral(WBTC/USDT) _{Amount}= \cfrac{AGOBTC/AGOUSD_{Amount}×ECR}{Collateral(WBTC/USDT) _{Price}}
$$

$$
Share (CNBTC/CNUSD)_{Amount}= \cfrac{AGOBTC/AGOUSD_{Amount}×(1-ECR)}{Share (CNBTC/CNUSD)_{Price}}
$$

