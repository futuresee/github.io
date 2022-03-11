---
title: 聚合行情
position_number: 1.3
type: get
description: /data/api/v1/getTicker
parameters:
    -
        name: market
        type: string
        mandatory: true
        default: N/A
        description: 交易市场
        ranges: btc_usdt, eth_usdt...
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getTicker() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getTicker?market=btc_usdt\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block:
            ```javascript
                {
                    "error": {
                        "code": "",
                        "msg": ""
                    },
                    "msgInfo": "",
                    "result": {
                        "baseCoin": "",
                        "baseCoinDisplayPrecision": 0,
                        "baseCoinPrecision": 0,
                        "contractSize": 0,
                        "contractType": "",
                        "depthPrecisionMerge": 0,
                        "initLeverage": 0,
                        "labels": [],
                        "liquidationFee": 0,
                        "makerFee": 0,
                        "maxEntrusts": 0,
                        "maxOpenOrders": 0,
                        "minNotional": 0,
                        "minPrice": 0,
                        "minQty": 0,
                        "multiplierDown": 0,
                        "multiplierUp": 0,
                        "onboardDate": 0,
                        "pricePrecision": 0,
                        "quantityPrecision": 0,
                        "quoteCoin": "",
                        "quoteCoinDisplayPrecision": 0,
                        "quoteCoinPrecision": 0,
                        "state": 0,
                        "supportEntrustType": "",
                        "supportOrderType": "",
                        "supportTimeInForce": "",
                        "symbol": "",
                        "takerFee": 0,
                        "tradeSwitch": false,
                        "underlyingType": ""
                    },
                    "returnCode": 0
                }
            ```
        title: Response
        language: json
---
