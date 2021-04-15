---
description: Creating new tokens
---

# Minting AGOBTC & AGOUSD

The process of creating new algorithmic tokens is based on the current _Target Collateral Ratio_, which uses in the token minting formula. This formula shows the required amount of both collateral and share tokens needed for the minting in different examples.

{% hint style="info" %}
The token minting formula is the same for both AGOUSD / AGOBTC tokens. The main difference will be applied only for the mechanism of the price stability, as our main goal to reach $1 peg in the case of AGOUSD and to repeat all the price movements of Bitcoin, using our native AGOBTC.
{% endhint %}

Let's take a look at the following basic formula:

$$
AGOUSD / AGOBTC Ammount=(Ca*Cp) +(Sa*Sp)
$$

{% hint style="warning" %}
Where:

* Ca - the amount of the collateral
* Cp - the current price of the collateral
* Sa - CNUSD / CNBTC token amount
* Sp - the current price of both share CNUSD / CNBTC tokens
{% endhint %}

Now, let's take a look at the following situations, using different input data.

### Set - up №1:

* TCR - 100%
* USDT price - $1

In the beginning, when the level of the collateralization will be absolute, for minting 1 AGOUSD token, there is no need to use the CNUSD share token:

$$
1 USDT * 1 = $1 =1AGOUSD
$$

### Set - up №2:

* TCR - 76.25%
* WBTC price - $62,350
* CNBTC price - $21,500
* We are going to mint 1 AGOBTC





