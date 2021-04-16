---
description: Creating new tokens
---

# Minting AGOBTC & AGOUSD

The whole process of minting new tokens into circulation works in the same way for both algorithmic AGOBTC and AGOUSD tokens. It is based on the current _Target Collateral Ratio._ Argano protocol uses a formula, which shows the required amount of both collateral and share tokens needed for the minting in different examples.

{% hint style="info" %}
The main difference will be applied only for the mechanism of the price stability, as our main goal to reach $1 peg in the case of AGOUSD and to repeat all the price movements of Bitcoin for our native AGOBTC.
{% endhint %}

Let's take a look at the following basic formula:

$$
AGOUSD / AGOBTC Amount=(Ca*Cp) +(Sa*Sp)
$$

{% hint style="warning" %}
Where:

* Ca - the amount of the collateral
* Cp - the current price of the collateral
* Sa - CNUSD / CNBTC token amount
* Sp - the current price of both share CNUSD / CNBTC tokens
{% endhint %}

Now, let's take a look at the following situations, using different input data.

In the case of AGOUSD minting, the amount of CNUSD and collateral \(USDT\) is required to reach a $1 price. The required amount of both share and collateral tokens will be calculated according to the present **`TCR`** level.

### Set - up №1:

* TCR is equal to 100%
* USDT price - $1.00

In the beginning, when the level of the collateralization will be absolute, for minting 1 AGOUSD token, there is no need to use the CNUSD share token:

$$
1 USDT * 1 = $1 =1AGOUSD
$$

### Set - up №2:

* TCR  is equal to 70%
* WBTC price - $62,000.00
* CNBTC - $24,000.00
* The user wants to mint 1 AGOBTC using his 0.7 WBTC

Let's find the amount of CNBTC, needed to perform the minting, using 0.7 WBTC:

$$
CNBTC Amount= (0.7*62,000.00)*(1-0.7)/24,000.00*0.7=13020/16800=0.775
$$

Using 0.7 WBTC and 0.775 CNBTC the total amount of AGOBTC will be minted.

$$
(0.7WBTC*62000)+(0.775*24000)=43400+18600=$62000 = 1AGBTC
$$

The same calculation applies to the AGOUSD minting.

