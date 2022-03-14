---
title: 获取ADL信息
position_number: 12
type: get
description: /v1/position/adl
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"longQuantile\": 0,\n\t\t\t\"shortQuantile\": 0,\n\t\t\t\"symbol\": \"\"\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---