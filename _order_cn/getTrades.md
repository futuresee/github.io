---
title: 查询成交明细
position_number: 1.1
type: get
description: /v1/order/trade-list
parameters:
    -
        name: orderId
        type: integer
        mandatory: true
        default: N/A
        description: 订单id
        ranges:
    -
        name: page
        type: integer
        mandatory: true
        default: 1
        description: "页码\t"
        ranges:
    -
        name: size
        type: integer
        mandatory: false
        default: 10
        description: "单页数\t"
        ranges:
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"items\": [\n\t\t\t{\n\t\t\t\t\"fee\": 0,\n\t\t\t\t\"feeCoin\": \"\",\n\t\t\t\t\"orderId\": 0,\n\t\t\t\t\"price\": 0,\n\t\t\t\t\"quantity\": 0,\n\t\t\t\t\"symbol\": \"\",\n\t\t\t\t\"timestamp\": 0\n\t\t\t}\n\t\t],\n\t\t\"page\": 0,\n\t\t\"ps\": 0,\n\t\t\"total\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---