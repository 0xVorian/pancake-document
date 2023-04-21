# Perpetuals V2 Glossary

**Here you will find defined all the terms inherent in futures trading**

Perpetuals, perpetual swaps, or perps are a special type of futures contract without an expiration date.

Leverage is a trading mechanism. Traders can use it to increase their exposure to the market by allowing them to pay less than the full amount of the investment. In simple words, you borrow money to leverage your investment.

**Long:** Open a Long order. In this order, you purchase an asset and wait to sell when the price increases. "Buy" and "long" are used interchangeably.

**Short:** Open a Short order. In this order, you borrow an asset, sell it, and hope to repurchase it when the price drops. "Sell" and "short" are used interchangeably.

**Limit Order:** A limit order is buying or selling at a specific price or better. Limit orders are not guaranteed to execute.

**Market Order:** A market order is an order to buy or sell at the best available current price.

Users can check the details of their opened positions, such as the opening price, by clicking on "Position" located at the bottom of the trading page. They can view details such as opening price, number of positions, latest price and forced liquidation price.

![](https://1397868517-files.gitbook.io/\~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MHREX7DHcljbY5IkjgJ-1972196547%2Fuploads%2FGvHa3Qp2sxjIorIkJ1TX%2FPerp5.png?alt=media\&token=86d5d591-446f-4e57-b6af-5210f4f7b6d9)

PancakeSwap will use an isolated leverage mode for each v2 trading pair. Pairs operate independently:

* Each trading pair is an isolated position, Users can open multiple isolated positions
* Every position (trading pair) runs independently. If users need to top up their margin, they will need to do so manually even if they have available assets in other separate positions (ApolloX will support auto top-up in the future)
* Every isolated trading position will have its own risk rate and liquidation price and will be settled individually.
* Liquidation risk is isolated for each trading pair. If a position is liquidated, it does not affect other positions.

Users can close their positions by clicking on "Close Position".
