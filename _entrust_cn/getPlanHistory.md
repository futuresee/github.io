---
title: 查询历史计划委托
position_number: 6
type: get
description: /v1/entrust/plan-list-history
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: "交易对（不传时撤销所有交易对）\t"
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
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"hasNext\": false,\n\t\t\"hasPrev\": false,\n\t\t\"items\": [\n\t\t\t{\n\t\t\t\t\"closePosition\": false,\n\t\t\t\t\"createdTime\": 0,\n\t\t\t\t\"entrustId\": 0,\n\t\t\t\t\"entrustType\": \"\",\n\t\t\t\t\"marketOrderLevel\": 0,\n\t\t\t\t\"orderSide\": \"\",\n\t\t\t\t\"ordinary\": true,\n\t\t\t\t\"origQty\": 0,\n\t\t\t\t\"positionSide\": \"\",\n\t\t\t\t\"price\": 0,\n\t\t\t\t\"state\": \"\",\n\t\t\t\t\"stopPrice\": 0,\n\t\t\t\t\"symbol\": \"\",\n\t\t\t\t\"timeInForce\": \"\",\n\t\t\t\t\"triggerPriceType\": \"\"\n\t\t\t}\n\t\t]\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---