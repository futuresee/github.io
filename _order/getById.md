---
title: 根据id查询订单
position_number: 3
type: get
description: /v1/order/detail
parameters:
  - name: orderId
    type: string
    mandatory: true
    default: N/A
    description: 订单id
    ranges:
left_code_blocks:
  - code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
    title: Java
    language: java
right_code_blocks:
  - code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"avgPrice\": 0,\n\t\t\"closePosition\": false,\n\t\t\"closeProfit\": 0,\n\t\t\"createdTime\": 0,\n\t\t\"executedQty\": 0,\n\t\t\"forceClose\": false,\n\t\t\"marginFrozen\": 0,\n\t\t\"orderId\": 0,\n\t\t\"orderSide\": \"\",\n\t\t\"orderType\": \"\",\n\t\t\"origQty\": 0,\n\t\t\"positionSide\": \"\",\n\t\t\"price\": 0,\n\t\t\"sourceId\": 0,\n\t\t\"state\": \"\",\n\t\t\"symbol\": \"\",\n\t\t\"timeInForce\": \"\",\n\t\t\"triggerProfitPrice\": 0,\n\t\t\"triggerStopPrice\": 0\n\t},\n\t\"returnCode\": 0\n}"
    title: Response
    language: json
---