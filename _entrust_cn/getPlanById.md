---
title: 根据entrustId查询计划委托
position_number: 5
type: get
description: /v1/entrust/plan-detail
parameters:
    -
        name: entrustId
        type: integer
        mandatory: true
        default: N/A
        description: 委托id
        ranges:
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"closePosition\": false,\n\t\t\"createdTime\": 0,\n\t\t\"entrustId\": 0,\n\t\t\"entrustType\": \"\",\n\t\t\"marketOrderLevel\": 0,\n\t\t\"orderSide\": \"\",\n\t\t\"ordinary\": true,\n\t\t\"origQty\": 0,\n\t\t\"positionSide\": \"\",\n\t\t\"price\": 0,\n\t\t\"state\": \"\",\n\t\t\"stopPrice\": 0,\n\t\t\"symbol\": \"\",\n\t\t\"timeInForce\": \"\",\n\t\t\"triggerPriceType\": \"\"\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---