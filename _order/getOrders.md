---
title: 查询订单
position_number: 4
type: get
description: /v1/order/list
parameters:
  - name: page
    type:
    mandatory: true
    default: N/A
    description: 页码
    ranges:
  - name: size
    type:
    mandatory: true
    default:
    description: 单页数
    ranges:
  - name: startTime
    type:
    mandatory: true
    default:
    description: 开始时间
    ranges:
  - name: endTime
    type:
    mandatory: true
    default:
    description: 结束时间
    ranges:
  - name: state
    type:
    mandatory: true
    default:
    description: >-
      订单状态
      NEW：新建订单（未成交）；PARTIALLY_FILLED：部分成交；FILLED：全部成交；CANCELED：用户撤销；REJECTED：下单失败；EXPIRED：已过期；UNFINISHED：未完成；HISTORY：（历史）
    ranges:
  - name: symbol
    type:
    mandatory: false
    default:
    description: 交易对
    ranges:
left_code_blocks:
  - code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
    title: Java
    language: java
right_code_blocks:
  - code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"items\": [\n\t\t\t{\n\t\t\t\t\"avgPrice\": 0,\n\t\t\t\t\"closePosition\": false,\n\t\t\t\t\"closeProfit\": 0,\n\t\t\t\t\"createdTime\": 0,\n\t\t\t\t\"executedQty\": 0,\n\t\t\t\t\"forceClose\": false,\n\t\t\t\t\"marginFrozen\": 0,\n\t\t\t\t\"orderId\": 0,\n\t\t\t\t\"orderSide\": \"\",\n\t\t\t\t\"orderType\": \"\",\n\t\t\t\t\"origQty\": 0,\n\t\t\t\t\"positionSide\": \"\",\n\t\t\t\t\"price\": 0,\n\t\t\t\t\"sourceId\": 0,\n\t\t\t\t\"state\": \"\",\n\t\t\t\t\"symbol\": \"\",\n\t\t\t\t\"timeInForce\": \"\",\n\t\t\t\t\"triggerProfitPrice\": 0,\n\t\t\t\t\"triggerStopPrice\": 0\n\t\t\t}\n\t\t],\n\t\t\"page\": 0,\n\t\t\"ps\": 0,\n\t\t\"total\": 0\n\t},\n\t\"returnCode\": 0\n}"
    title: Response
    language: json
---