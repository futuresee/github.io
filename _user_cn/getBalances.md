---
title: 获取用户资金
position_number: 4
type: get
description: /v1/balance/list
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"availableBalance\": 0,\n\t\t\t\"coin\": \"\",\n\t\t\t\"isolatedMargin\": 0,\n\t\t\t\"openOrderMarginFrozen\": 0,\n\t\t\t\"walletBalance\": 0\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---