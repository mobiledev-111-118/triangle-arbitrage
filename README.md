# Binance Triangle Arbitrage

<div style="text-align: center;">
    <img src="https://github.com/bmino/binance-triangle-arbitrage/blob/master/src/resources/mainDisplay.png" alt="Main HUD display">
</div>

This app monitors the [Binance](https://www.binance.com) cryptocurrency exchange in search of triangle arbitrage opportunities.

## The HUD
The HUD is the chart displayed above. It is repainted after each calculation cycle to show snapshots of currently detected
arbitrage opportunities. To disable the HUD, set `HUD.ENABLED` to false.


### Reading the HUD
* **Trade** - Three symbols related by exchange rates that are involved in the triangle arbitrage.
* **Profit** - Percent profit or loss from executing the triangle arbitrage. This includes trading fees specified via `EXECUTION.FEE` config.
* **AB Age** - Time in milliseconds since the most recent update of the market ticker relating the first and second symbols in the arbitrage.
* **BC Age** - Time in milliseconds since the most recent update of the market ticker relating the second and third symbols in the arbitrage.
* **CA Age** - Time in milliseconds since the most recent update of the market ticker relating the third and first symbols in the arbitrage.
* **Age** - Time in milliseconds since the least recently updated market ticker involved in the triangle arbitrage.