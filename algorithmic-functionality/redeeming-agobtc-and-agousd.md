---
description: Redeeming explanation
---

# Redeeming AGOBTC & AGOUSD

The process of redeeming implies returning the collateralized tokens AGOUSD / AGOBTC back to the protocol and, in return, receiving back the user's collateral assets and the required amount of share tokens CNBTC / CNUSD, which are required to reach desired equality. This in turn means that with every $1 value, users will receive part of the collateral together with the part of share tokens.

The redeeming formula works based on the Effective Collateral Ratio \(`ECR`\) and applies for both algorithmic tokens:

$$
Collateral(WBTC/USDT) _{Amount}= \cfrac{AGOBTC/AGOUSD_{Amount}×ECR}{Collateral(WBTC/USDT) _{Price}}
$$

$$
Share (CNBTC/CNUSD)_{Amount}= \cfrac{AGOBTC/AGOUSD_{Amount}×(1-ECR)}{Share (CNBTC/CNUSD)_{Price}}
$$

Now, let's take a look at the following situations, using different input data.

### Set - up №1:

* ECR - 100%
* USDT price - $1.00

$$
USDT_{Amount}= \cfrac{100_{AGOUSD}}{$1} = 100_{USDT}
$$

### Set - up №2:

* ECR  is equal to 80%
* WBTC price - $59,000.00
* CNBTC - $18,000.00
* The user wants to redeem 1 AGOBTC

$$
WBTC_{Amount}= \cfrac{1_{AGOBTC}×\overbrace{80\%}^{\text{ECR}}}{\underbrace{59000}_{\text{WBTC price}}} = 0.00001356_{WBTC}
$$

$$
CNBTC_{Amount}= \cfrac{1_{AGOBTC}×(1-\overbrace{80\%}^{\text{ECR}})}{\underbrace{18000}_{\text{CNBTC price}}} = 0.00001111_{CNBTC}
$$

Summarizing all the above, when the user redeems 1 AGOBTC, he receives 0.00001356 WBTC and 0.00001111 at the WBTC price - $59,000.00 and ECR level of 80%.

$$
\text{Total Value} =(0.00001356_{WBTC}×59000) +(0.00001111_{CNBTC}×18000)= 0.80004+0.19998=1.00002
$$



