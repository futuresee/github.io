---
title: 获取全交易对的聚合行情信息
position_number: 1.7
type: get
description: /v1/public/q/agg-tickers
parameters:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"a\": \"\",\n\t\t\t\"ap\": \"\",\n\t\t\t\"bp\": \"\",\n\t\t\t\"c\": \"\",\n\t\t\t\"h\": \"\",\n\t\t\t\"i\": \"\",\n\t\t\t\"l\": \"\",\n\t\t\t\"m\": \"\",\n\t\t\t\"o\": \"\",\n\t\t\t\"r\": \"\",\n\t\t\t\"s\": \"\",\n\t\t\t\"t\": 0,\n\t\t\t\"v\": \"\"\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---