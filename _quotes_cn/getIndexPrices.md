---
title: 获取所有交易对的指数价格
position_number: 2.5
type: get
description: /v1/public/q/index-price
parameters:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"p\": 0,\n\t\t\t\"s\": \"\",\n\t\t\t\"t\": 0\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---