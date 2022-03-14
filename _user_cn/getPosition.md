---
title: 获取持仓信息
position_number: 7
type: post
description: /v1/position/list
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: 交易对（不传时查询所有交易对的持仓信息）
        ranges:
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"autoMargin\": false,\n\t\t\t\"availableCloseSize\": 0,\n\t\t\t\"closeOrderSize\": 0,\n\t\t\t\"entryPrice\": 0,\n\t\t\t\"isolatedMargin\": 0,\n\t\t\t\"leverage\": 0,\n\t\t\t\"openOrderMarginFrozen\": 0,\n\t\t\t\"positionSide\": \"\",\n\t\t\t\"positionSize\": 0,\n\t\t\t\"positionType\": \"\",\n\t\t\t\"realizedProfit\": 0,\n\t\t\t\"symbol\": \"\"\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---