---
title: 根据profitId查询止盈止损
position_number: 11
type: get
description: /v1/entrust/profit-detail
parameters:
    -
        name: profitId
        type: integer
        mandatory: true
        default: N/A
        description: 止盈止损id
        ranges:
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"createdTime\": 0,\n\t\t\"entryPrice\": 0,\n\t\t\"executedQty\": 0,\n\t\t\"isolatedMargin\": 0,\n\t\t\"origQty\": 0,\n\t\t\"positionSide\": \"\",\n\t\t\"positionSize\": 0,\n\t\t\"profitId\": 0,\n\t\t\"state\": \"\",\n\t\t\"symbol\": \"\",\n\t\t\"triggerProfitPrice\": 0,\n\t\t\"triggerStopPrice\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---