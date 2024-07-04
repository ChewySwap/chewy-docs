---
description: How to migrate project Liquidity from Marswap to ChewySwap
---

# 🌎 Migrate from Marswap

On July 1st it was announced that former competitor Marswap DEX on Shibarium would be "closing its doors" and projects had 24 hours to remove their liquidity and migrate before they took down the frontend.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

This was understandably met with a lot of panic by projects owners and was soon extended afterwards, but still it is a good idea to always have a plan in case the unexpected happens. Their reasoning was that volume couldn't sustain the cost of running their website.&#x20;

Lets be real for a minute here: it's not easy building on new Layer 2 blockchains as it can take time for adoption to take off and for developer services to start supporting it. Never count your eggs before they've hatched! If you expect to launch a project and for it to be instantly successful then you are setting yourself up for bitter disappointment. Everything takes time to build and expect to be in it for the long run or not at all! Always have a backup to your backup to your backup plans!&#x20;

ChewySwap has been building on Dogechain for over 2 years (starting as Dogeshrek DEX) and has been launched on Shibarium since day 1! Uptime, reliability and trust are always at the top of our priorities and in the forefront of our minds. We have backups to our backups and there will NEVER be a case where you are unable to access your tokens and liquidity. We have backups on IPFS and if that fails you can even download and host a version of our frontend yourself!

## Help is Here with ChewySwap ❤️

If you run a project and need assistance in the migration process [do not hesitate to reach out](https://t.me/m/vQs2JNEBNzkx). For those of us who are more technically inclined here are some pointers to help you if you're having trouble removing liquidity from Marswap (as you're unlikely to get any help from them).



### Try first if you have trouble Removing from Marswap:

The first step you can try if getting an error on removing liquidity is to switch to receive WBONE. On Marswap this option isn't very obvious and is easy to miss. This is done by clicking where it says "Receive WNative" as pointed out in this screenshot:

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="357"><figcaption><p>Click Receive WNative to remove as WBONE</p></figcaption></figure>

Then you will just have to unwrap the resulting WBONE back to BONE. (The process to remove is to first click "Enable", confirm transaction and wait for confirmation. Then click "Remove" to finish process)



### If removing as WBONE doesnt work...

If your token smart contract has a tax or any limits on max wallet, max transaction etc it is recommended that you first go to your smart contract's write page and:

* [ ] Turn off SwapBack (setSwapTokensAtAmount function set to 0) - This is a function that sets how many tokens the contract needs to fill with before swapping for rewards, marketing, etc. If liquidity is removed then this function won't work so your transaction will revert. This setting must be turned all the way down to 0 or off if possible
* [ ] Set max wallet / max TX to total supply of token (don't forget to add 18 0's at the end of the number to account for decimal amount. for example for 1 token the # would be 1000000000000000000)
* [ ] Make sure wallet that is removing LP is exempt from taxes, max wallet, max tx, etc
* [ ] If none of these work contact us for more help





## Migrating the Liquidity to ChewySwap

[You can find our guide on adding liquidity on ChewySwap here](../products/exchange/liquidity-pools.md). But to ensure your project has a smooth migration and the starting price is the same as was on Marswap make sure you add the tokens in the same exact ratio of TOKEN/BONE as was originally removed. If you're adding LP to both ChewySwap and ShibaSwap still keep the same ratio to ensure the same price. It can be figured out by a simple ratio:

$$
tokenAmount/oldBONE = X/newBONE
$$

So tokenAmount/oldBONE is the amount of token and BONE you removed from Marswap. Cross multiply and divide to figure out new token amount for new bone amount and vice versa.
