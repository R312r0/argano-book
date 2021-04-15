---
description: Creating new tokens
---

# Minting AGOBTC & AGOUSD

The process of creating new algorithmic tokens is based on the current _Target Collateral Ratio_, which uses in the token minting formula. This formula shows the required amount of both collateral and share tokens needed for the minting in defferent examples.

{% hint style="info" %}
The token minting formula is the same for both AGOUSD / AGOBTC tokens. The main difference will be applied only for the mechanism of the price stability, as our main goal to reach $1 peg in the case of AGOUSD and to repeat all the price movements of Bitcoin, using our native AGOBTC.
{% endhint %}

Let's take a look at the following formula:

$$
AGOUSD / AGOBTC Ammount=(Ca*Cp) +(Sa*Sp)
$$

{% hint style="warning" %}
Where:

* Ca - ammount of the collateral
* Cp - current price of the collateral
* Sa - CNUSD / CNBTC token ammount
* Sp - current price of the both share CNUSD / CNBTC tokens
{% endhint %}

