---
title: 获取交易对的深度信息
position_number: 9
type: get
description: /v1/public/q/depth
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: 交易对
        ranges:
    -
        name: level
        type: integer
        mandatory: true
        default: N/A
        description: "档位（min:1,max:50）\t"
        ranges:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"a\": [],\n\t\t\"b\": [],\n\t\t\"s\": \"\",\n\t\t\"t\": 0,\n\t\t\"u\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---