---
title: 获取账户相关信息
position_number: 1
type: get
description: /v1/account/info
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"accountId\": 0,\n\t\t\"allowOpenPosition\": false,\n\t\t\"allowTrade\": false,\n\t\t\"allowTransfer\": false,\n\t\t\"openTime\": \"\",\n\t\t\"state\": 0,\n\t\t\"userId\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---