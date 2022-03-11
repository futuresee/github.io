---
title: 获取所有交易对的配置信息
position_number: 1.3
type: get
description: /v1/public/symbol/list
parameters:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"baseCoin\": \"\",\n\t\t\t\"baseCoinDisplayPrecision\": 0,\n\t\t\t\"baseCoinPrecision\": 0,\n\t\t\t\"contractSize\": 0,\n\t\t\t\"contractType\": \"\",\n\t\t\t\"depthPrecisionMerge\": 0,\n\t\t\t\"initLeverage\": 0,\n\t\t\t\"labels\": [],\n\t\t\t\"liquidationFee\": 0,\n\t\t\t\"makerFee\": 0,\n\t\t\t\"maxEntrusts\": 0,\n\t\t\t\"maxOpenOrders\": 0,\n\t\t\t\"minNotional\": 0,\n\t\t\t\"minPrice\": 0,\n\t\t\t\"minQty\": 0,\n\t\t\t\"multiplierDown\": 0,\n\t\t\t\"multiplierUp\": 0,\n\t\t\t\"onboardDate\": 0,\n\t\t\t\"pricePrecision\": 0,\n\t\t\t\"quantityPrecision\": 0,\n\t\t\t\"quoteCoin\": \"\",\n\t\t\t\"quoteCoinDisplayPrecision\": 0,\n\t\t\t\"quoteCoinPrecision\": 0,\n\t\t\t\"state\": 0,\n\t\t\t\"supportEntrustType\": \"\",\n\t\t\t\"supportOrderType\": \"\",\n\t\t\t\"supportTimeInForce\": \"\",\n\t\t\t\"symbol\": \"\",\n\t\t\t\"takerFee\": 0,\n\t\t\t\"tradeSwitch\": false,\n\t\t\t\"underlyingType\": \"\"\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---