---
description: FAQ about ChewySwap
---

# ❔ Frequently Asked Questions

## Swaps

<details>

<summary>Q: What is Unknown error: "Chewy: K"?</summary>

A: If you get this error it means you are swapping a token which has a tax on it with your output set at a certain BONE or DOGE amount. To fix this error first make sure your slippage is set high enough to account for the token's tax, then modify the input side of your trade and try again. For example:&#x20;

* Remove decimals from token amount
* Add .000 to end of whole number token amount

</details>

<details>

<summary>Q: How to fix transaction error "Cannot convert string to buffer. toBuffer only supports 0x-prefixed hex strings and this string was given: 109"?</summary>

A: This is an error related to MetaMask wallet which can usually be fixed by closing out of ChewySwap tab and closing MetaMask then trying again. If the problem persists we recommend importing your MetaMask wallets into a better wallet app such as [Rabby walle](https://rabby.io/)t as MetaMask has been having many problems recently.

</details>
