# FAQ

## Swap

### What’s new in v3 Exchange?

* Concentrated liquidity - liquidity will be concentrated on the most actively traded price range, which means:
  * Lower trading slippage for traders
  * Potentially more LP fee rewards for liquidity providers
* A flexible trading fee structure - Liquidity providers can choose between multiple trading fee tiers when creating liquidity pairs or providing liquidity
* Customisable price range - Liquidity providers can also choose what price ranges they want to provide liquidity to
* Non-fungible liquidity positions - Each liquidity position will have its own unique ID corresponding to its configurations (such as price range). Therefore, you will be able to create and maintain multiple positions with the same trading pair but with different configurations and liquidity amount
* Backwards compatible - v3 Exchange will also utilise the legacy v2 and stable swap liquidity pairs to always provide the best trading route
* Built-in limit order - Pro users can utilise the new customisable price range in liquidity provisioning to effectively create a limit order which will convert all the tokens to the desired one when the price hits the target

### **How come my transaction won't go through?**

PancakeSwap is a DeFi application such that it interacts with the wallet to complete on-chain transactions for swapping, creating LPs, staking in farms and pools, etc.

**Gas Fees**

As such, the first thing is to **make sure you have enough BNB to pay for the gas fee** of the on-chain transactions. Typically, gas fee fluctuates depending on the number of transactions in the queue, if there are more transactions, a higher gas fee may be required to push through the transaction. On BNB Smart Chain, the gas fee typically ranges from cents to a dollar USD in BNB. Learn more about [gas fee here](https://academy.binance.com/en/glossary/gas).

**Transaction Fees**

If your swapping action still doesn't go through and it is displaying an error for you to revise the slippage -- you may want to check if the tokens you are trying to swap has **any fees and restrictions on transactions**.

It is not uncommon for tokens on BNB Smart Chain to include a **transaction fee** in their contracts, usually these fees could be used for burning, funding a treasury of a fair launch project -- for example, this [APX token has an 1% tax on every transaction](https://apollox-finance.gitbook.io/apollox-finance/apx-token/tax) for sending to a burn address, such that more transactions would mean more burning, accruing value to APX token holders.

With the transaction fee, whether it is inclusive (a portion of the swap amount is sent elsewhere than your address so the output is less than expected for the estimated input) or exclusive (requiring an additional transfer from your address to send extra tokens so the input is more than expected for the estimated output), it affects the input and output amount that you agree for signing the transaction. In many cases, the transaction cannot meet the input and output requirements because of the tax.

**Swapping with Transaction Fees**

Before you swap any tokens, make sure you have visited their website to understand if they have a transaction fee mechanism (or _tax_ as many projects put it). If there is, make sure you set a slippage that is sufficient to accommodate the transaction fee -- e.g. if there is a transaction fee of 5%, your slippage will have to be set at at least 5% plus the normal trading slippage depending on your trading amount and the token's liquidity, say 5.5%-6%.

In some extreme cases including some scams, some tokens even have a block on most or all transfers on chain, or only allowing certain addresses to sell, in such case it is impossible to swap the token successfully. Do learn about the token you are trying to swap and be aware of any fees and restrictions!



### Does the new Swap interface use v2 or stable swap liquidity?

Yes. The new Swap v3 uses liquidity from PancakeSwap v3, v2 and stable swap to get the best trading route.



### What is split routing?

In Swap v3, your trade might be broken into multiple routes to execute your trade with the best rate.

To view more detail of how your trade is routed, tap the “v” button on the “Route” section to expand and view the details.



### How to customise or disable certain liquidity sources?

The new Swap v3 uses liquidity from PancakeSwap v3, v2 and stable swap to get the best trading route. However, you can customize or disable certain liquidity sources if you do not want your trade to route through them.

When viewing a trading route, click the “Customize Routing” button. Or click the cog ⚙️ button on the top right hand corner of the Swap interface and choose “Customize Routing”.

Within the “Customize Routing” pop up, you are able to choose which liquidity source you want to utilise. Or disable multihops completely.

Note: disabling multihops could lead to increased slippage or worse trading rate on specific trading pairs. Proceed with caution.

## Liquidity

### What are fee tiers and how to pick the correct one?

In Exchange v3, when you are providing liquidity, you can choose between several different trading fees (0.01%, 0.05%, 0.25%, and 0.1%) for the same token pair.

For example, for CAKE-BNB, there might be a 0.25% pair, which means a 0.25% trading fee is in place for every trade. However, some liquidity providers might choose to provide liquidity to a CAKE-BNB trading pair with a 0.05% fee rate, offers a better quote and attract more trading volume.

There is no “correct” answer for which trading fee configuration to choose. It depends on the tokens within the trading pair. Usually, volatile tokens should have a higher trading fee to better compensate for the impermanent loss brought by the volatility. On the other hand, tokens like stable coins have smaller price movements and lower impermanent losses, therefore their trading fee should be lower.

When selecting a token pair, the “Add Liquidity” interface will automatically choose the most popular fee tier for you.



### What happens if my liquidity position goes out of range?

You will not earn any trading fee rewards if the current price goes out of the price range defined in your position.

We recommend removing liquidity and reconfiguring an active position to continue earning trading fee rewards.

On top of that, all tokens will be converted to one single asset depending on the direction of the price condition.

For example, if a position of CAKE/BUSD is configured with a price range of 3 BUSD per CAKE to 5 BUSD per CAKE. And all assets in the position will be converted to BUSD if the CAKE price is higher or equal to 5 BUSD per CAKE, and vice versa.



### Is it better to always provide liquidity with a smaller range?

Providing liquidity to a smaller price range will help concentrate your liquidity to a spesific price range, boosting your relative shares again the total liquidity within the price range, potentially earning more trading fee rewards.

However, please bear in mind that only active liquidity positions will earn trading fee rewards from trades. This means you will only earn rewards when the current trading price is within the price range defined in the liquidity position.



### Are there any ways to automatically adjust my position so it is always in range and earning fee rewards?

Automatic position managing feature is coming soon to PancakeSwap v3 with one-click liquidity depositing (Zap!). Stay tuned for more detail.



### What will be the trading fee breakdown for v3 Exchange?

|                    | 0.01% | 0.05% | 0.25% | 1%  |
| ------------------ | ----- | ----- | ----- | --- |
| Liquidity Provider | 67%   | 66%   | 68%   | 68% |
| CAKE Burn          | 10%   | 10%   | 23%   | 23% |
| Treasury           | 23%   | 24%   | 9%    | 9%  |



### Are LP fee rewards automatically compounded like Exchange v2?

No.

In Exchange v3 you will need to claim trading fee rewards manually. You may do that on the position detail page. You may find all your v3 liquidity positions on the liquidity page.



### What affects LP APR and how to calculate it?

In Exchange v3, LP fee reward APR could vary between liquidity positions. It is based on the following factors:

* Trading volume\
  \- more volume generates more fee rewards
* Liquidity pair fee tier\
  \- higher fee tier generates more fee rewards from individual trades
* The number of tokens deposited\
  \- more token in the position translates to a larger relative share against the total active liquidity, which gets more trading fee rewards from trades
* The selected price range\
  \- smaller price range allows a higher concentration for the same amount of token deposited, which translates to a larger relative share against the total active liquidity, and gets more trading fee rewards from trades
* The amount of liquidity currently active\
  \- if there are more users who deposit and concentrate their liquidity with the same range as you, you will earn less trading fee due to a smaller relative share against the total
* Whether the liquidity position is active\
  \- only active liquidity positions will earn trading fee rewards

Since the manual calculation is complex and time-consuming. We are offering:

Automatic APR calculation for every PancakeSwap v3 liquidity position which calculates based on the live data of liquidity distributions/concentrations, historical volume data, and the configurations from the position.

* You may find the APR display on the top right-hand corner of the position detail page or in the list of v3 liquidity positions.
* Plus, when creating a new liquidity position, the APR value is calculated live, reacting with the configuration changes you just made.

On top of that, we are also offering an easy-to-use ROI calculator for all PancakeSwap liquidity providers.

* You may find the calculator button on every APR display. Simply click and open the ROI calculator panel.



### Can I provide v2 liquidity?

Providing v2 liquidity is no longer advisable. We recommend using v3 liquidity to take advantage of the new features to improve efficiency.

If you want to proceed with adding v2 liquidity:

* If the token pair does not have a v3 pool, or it has more liquidity in v2 than the largest pool in v3. A “Add V2 Liquidity” will appear. Simply click to switch to adding v2 liquidity
* Alternatively, use `/v2` in the URL to always use v2 liquidity provisioning



### How to manage stable LP, and legacy v2 LP?

You can manage them as usual by going to the [Liquidity](https://pancakeswap.finance/liquidity) page.
