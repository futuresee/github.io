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
        code_block: "{\n	\"error\": {\n		\"code\": \"\",\n		\"msg\": \"\"\n	},\n	\"msgInfo\": \"\",\n	\"result\": [\n		{\n		  \"baseCoin\": \"\",\n			\"baseCoinDisplayPrecision\": 0,\n			\"baseCoinPrecision\": 0,\n			\"contractSize\": 0,\n			\"contractType\": \"\",\n			\"depthPrecisionMerge\": 0,\n			\"initLeverage\": 0,\n			\"labels\": [],\n			\"liquidationFee\": 0,\n			\"makerFee\": 0,\n			\"maxEntrusts\": 0,\n			\"maxOpenOrders\": 0,\n			\"minNotional\": 0,\n			\"minPrice\": 0,\n			\"minQty\": 0,\n			\"multiplierDown\": 0,\n			\"multiplierUp\": 0,\n			\"onboardDate\": 0,\n			\"pricePrecision\": 0,\n			\"quantityPrecision\": 0,\n			\"quoteCoin\": \"\",\n			\"quoteCoinDisplayPrecision\": 0,\n			\"quoteCoinPrecision\": 0,\n			\"state\": 0,\n			\"supportEntrustType\": \"\",\n			\"supportOrderType\": \"\",\n			\"supportTimeInForce\": \"\",\n			\"symbol\": \"\",\n			\"takerFee\": 0,\n			\"tradeSwitch\": false,\n			\"underlyingType\": \"\"\n		}\n	],\n	\"returnCode\": 0\n}"
        title: Response
        language: json
---
