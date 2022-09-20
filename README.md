# TradingView Charting Library UDF Data Source

Sample implementation of server-side UDF-compatible data source for [Binance exchange](https://www.binance.com/) for [TradingView](https://www.tradingview.com/) [Charting Library](https://www.tradingview.com/HTML5-stock-forex-bitcoin-charting-library/).

## Run

```
$ npm install
$ npm start
```

Default port is 80.

### Docker

```
$ docker build . -t udf
$ docker run -p 8080:80 udf
```

### Test

In browser open:

http://localhost/symbols?symbol=ETHBTC

or

http://localhost:8080/symbols?symbol=ETHBTC

if you start from docker with port 8080.

### Test with Chart Library

Take library from TradingView repo.

Open `index.html` and find `new TradingView.widget({})` and setup config:

- set `symbol` to `BTCUSDT`
- set `datafeed` to `new Datafeeds.UDFCompatibleDatafeed('http://localhost')` or `new Datafeeds.UDFCompatibleDatafeed('http://localhost:8080')` if you use port 8080.

For example you can use [http-server](https://www.npmjs.com/package/http-server) to serve library. In library directory write commands in terminal:

```
$ npm install -g http-server
$ http-server -p 3000
```

Check in browser:
# run live server-plugin port that make system  random choice
or
http://localhost:3000/index.html

## Links

* [Binance REST API](https://github.com/binance-exchange/binance-official-api-docs)
* [TradingView Charting Library](https://www.tradingview.com/HTML5-stock-forex-bitcoin-charting-library/)
* [TradingView Charting Library Demo](https://charting-library.tradingview.com/)
* [TradingView GitHub](https://github.com/tradingview)




## Installation
- ** 설치 docker 를 권장<br>
- 사용한 Docker image는 Docker Hub에 첨부합니다. <br>
    - https: ~~ <br>

```
git clone https://github.com/d10000usd/Tradingview.git
cd TRADINGVIEW
pip install -r requirements.txt
pip install .
```


