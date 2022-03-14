---
title: 查询历史订单
position_number: 1.1
type: get
description: /v1/order/list-history
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: 交易对
        ranges:
    -
        name: direction
        type: string
        mandatory: false
        default: NEXT
        description: "方向（PREV:上一页；NEXT:下一页）\t"
        ranges: PREV;NEXT
    -
        name: id
        type: integer
        mandatory: false
        default: N/A
        description: id
        ranges:
    -
        name: limit
        type: integer
        mandatory: false
        default: 10
        description: "条数\t"
        ranges:
    -
        name: startTime
        type: integer
        mandatory: false
        default:
        description: 起始时间
        ranges:
    -
        name: endTime
        type: integer
        mandatory: false
        default:
        description: 结束时间
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