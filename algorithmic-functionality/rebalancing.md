---
description: Over-collateralization / under-collateralization
---

# Rebalancing

If we are talking about algorithmic and partially collateralized tokens, we need to understand in which separate cases the system requires to update the current C - Ratio, based on the market condition and demand on the share tokens: CNUSD and CNBTC. The Argano protocol will automatically react to those conditions and implement the following actions:

## Condition №1: "Over-collateralization"

{% hint style="info" %}
Being in this state means that the system requires to lower Target Collateral Ratio and increase the value of share tokens: CNUSD / CNBTC
{% endhint %}

* Invoking the `rebalance` function will buy back CNUSD / CNBTC tokens from the market and lock them in the Treasury smart contract.

## Condition №2: "Under-collateralization"

{% hint style="info" %}
Being in this state means that the system requires to higher Target Collateral Ratio and increase the usage of the collateral assets in order to better support the price of algorithmic tokens: AGOUSD / AGOBTC
{% endhint %}

* Invoking the `rebalance` function will lead to the sale of share tokens CNUSD / CNBTC from the Treasury smart contract to reach the necessary amount of collateral assets.

