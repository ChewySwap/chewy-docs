# 🧑🌾 Yield Farming

Yield Farms allow users to earn CHEWY while supporting ChewySwap by staking LP Tokens.

Check out our [How to Use Farms Guide](how-to-use-farms.md) to get started with farming.



{% hint style="danger" %}
Yield farming can give better rewards than Single Token Staking Pools, but it comes with a risk of **Impermanent Loss**. It’s not as scary as it sounds, but it is worth learning about the concept before you get started.

Check out this great [article about Impermanent Loss ](https://academy.binance.com/en/articles/impermanent-loss-explained)from Binance Academy to learn more.
{% endhint %}

## Reward calculations

Yield Farm APR calculations include both:

* **LP rewards APR** earned through providing liquidity and;
* **Farm base rewards APR** earned staking LP Tokens in the Farm.

Why? Because when you stake your LP tokens in a farm to earn CHEWY, you're still providing liquidity to the liquidity pool, so you earn LP rewards as well!



### Calculating Farm Base Reward APR

The **Farm Base APR** is calculated according to the farm multiplier and the total amount of liquidity in the farm -- this is the amount of CHEWY distributed to the farm.



Let's use the SHIB/BONE pair as an example with these made up values:

**Liquidity:** $387.42M\
**Volume 24H:** $96.97M\
**Volume 7D:** 709.73M

* Calculate yearly fees
  * Use the 24H volume to calculate the **fee share** of liquidity providers in the pool (based on the 0.17% trading fee structure):\
    $96,970,000\*0.17/100 = **$164,849**
  * Next, use that **fee share** to estimate the projected **yearly fees** earned by the pool (based on the current 24h volume):\
    $164,849\*365 = **$60,169,885**
* We can now use the yearly fees to calculate the **LP rewards APR:** That's **yearly fees** divided by **liquidity:**\
  ($60,169,885/$387,420,000)\*100 = **15.53% LP reward APR**
