# crypto-exchange

An easy way to check the most up-to-date exchange rates between popular cryptocurrencies and real-world currency. Built using the CoinBase API. crypo-exchange also shows historical exchange rate data for cryptocurrencies, going back up to a year. Below are some screenshots of the app in action.

<p align="center">
<img src="https://github.com/jyoo980/crypto-exchange/blob/master/CryptoExchange/Assets.xcassets/v1.1-p1.imageset/v1.1-p1.png" width="327" height="561" style="float: left; width: 30%; margin-right: 1%; margin-bottom: 0.5em;">
<img src="https://github.com/jyoo980/crypto-exchange/blob/master/CryptoExchange/Assets.xcassets/v1.1-p2.imageset/v1.1-p2.png" width="327" height="561" style="float: left; width: 30%; margin-right: 1%; margin-bottom: 0.5em;">
</p>

## Development Requirements
* To use Charts for iOS, you need to install `Cocoapods` via `Ruby`. Luckily, macOS ships with Ruby in the base installation,  so all you need to do after cloning this repo is to `cd` into `crypto-exchange` and run `sudo gem install cocoapods`, then run `pod install`.

## Technologies
* CryptoCompare API (for most up-to-date exchange rates)
* Coinbin API (for historical exchange rates)
* Charts for iOS
* Custom Cache - `ExchangeRateCache.swift` 

## Current facts
* Request URL: https://rest.coinapi.io/v1/exchangerate/{CRPTO}/{REAL}?apikey={KEY}
* Looking to add more support for other crytocurrencies 

## Todos
* Refactor into MVC architecture - <strong>Tentatively Complete</strong>
* Introduce caching for API calls (workaround for 100 requests/24hr limit) - <strong>IN PROGRESS</strong>
* Refactor to use with API which has unlimited calls - <strong>Complete</strong>
* Introduce caching for historical data graphs (on app startup?)
