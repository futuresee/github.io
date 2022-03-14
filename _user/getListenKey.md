---
title: 获取listenKey
position_number: 16
type: get
description: /v1/user/listen-key
parameters:
    -
        name: symbol
        type: string
        mandatory: true
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
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---