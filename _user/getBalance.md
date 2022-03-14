---
title: 获取用户单币种资金
position_number: 3
type: get
description: /v1/balance/detail
parameters:
    -
        name: coin
        type: string
        mandatory: true
        default: N/A
        description: 币种
        ranges:
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"availableBalance\": 0,\n\t\t\"coin\": \"\",\n\t\t\"isolatedMargin\": 0,\n\t\t\"openOrderMarginFrozen\": 0,\n\t\t\"walletBalance\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---