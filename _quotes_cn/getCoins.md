---
title: 获取交易对币种
position_number: 1.1
type: get
description: /data/api/v1/getMarketConfig
parameters:
  - name:
    content:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
  - code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
    title: Java
    language: java
right_code_blocks:
  - code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [],\n\t\"returnCode\": 0\n}"
    title: Response
    language: json
---