# General config properties. Properties with `NULL` should be replaced with your own exchange account information.

##TRIBECA_MODE options = dev, prod
TRIBECA_MODE=dev

##EXCHANGE options = coinbase, hitbtc, okcoin, bitfinex, null
EXCHANGE=null

## See the README for more info on supported pairs.
TradedPair=BTC/USD

##Username and password is not necessary but highly recommended, especially if running in a cloud server
WebClientUsername=NULL
WebClientPassword=NULL

WebClientListenPort=3000
MongoDbUrl=mongodb://tribeca-mongo:27017/tribeca

##Set ShowAllOrders to false to save on memory
ShowAllOrders=true

NullGatewayTick=100

# DEV
## HitBtc
HitBtcPullUrl=http://demo-api.hitbtc.com
HitBtcOrderEntryUrl=ws://demo-api.hitbtc.com:8080
HitBtcMarketDataUrl=ws://demo-api.hitbtc.com:80
HitBtcSocketIoUrl=https://demo-api.hitbtc.com:8081
HitBtcApiKey=NULL
HitBtcSecret=NULL
HitBtcOrderDestination=HitBtc

## Coinbase / GDAX (Use GDAX API keys)
### Note: If you're using the sandbox URLs, you will need to create a separate API key, secret and passphrase. Live GDAX API credentials will NOT work with the GDAX Sandbox URLs and vice versa.
CoinbaseRestUrl=https://api-public.sandbox.gdax.com
CoinbaseWebsocketUrl=wss://ws-feed-public.sandbox.gdax.com
CoinbasePassphrase=NULL
CoinbaseApiKey=NULL
CoinbaseSecret=NULL
CoinbaseOrderDestination=Coinbase

## OkCoin
OkCoinWsUrl=wss://real.okcoin.com:10440/websocket/okcoinapi
OkCoinHttpUrl=https://www.okcoin.com/api/v1/
OkCoinApiKey=NULL
OkCoinSecretKey=NULL
OkCoinOrderDestination=OkCoin

## Bitfinex
BitfinexHttpUrl=https://api.bitfinex.com/v1
BitfinexKey=NULL
BitfinexSecret=NULL
BitfinexOrderDestination=Bitfinex

# PROD - values provided for reference.
## HitBtc
#HitBtcPullUrl=http://api.hitbtc.com
#HitBtcOrderEntryUrl=wss://api.hitbtc.com:8080
#HitBtcMarketDataUrl=ws://api.hitbtc.com:80
#HitBtcSocketIoUrl=https://api.hitbtc.com:8081
## Coinbase / GDAX
#CoinbaseRestUrl=https://api.gdax.com
#CoinbaseWebsocketUrl=wss://ws-feed.gdax.com
