---
title: 开通合约
position_number: 2
type: get
description: /v1/account/open
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": true,\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---