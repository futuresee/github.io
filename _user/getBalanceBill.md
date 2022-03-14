---
title: 获取用户账务流水
position_number: 5
type: get
description: /v1/balance/bills
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: 交易对
        ranges:
    -
        name: direction
        type:
        mandatory: true
        default: NEXT
        description: "方向（PREV:上一页；NEXT:下一页）\t"
        ranges: PREV;NEXT
    -
        name: id
        type:
        mandatory: false
        default:
        description: id
        ranges:
    -
        name: limit
        type:
        mandatory: false
        default:
        description: "条数\t"
        ranges:
    -
        name: startTime
        type:
        mandatory: false
        default:
        description: 起始时间
        ranges:
    -
        name: endTime
        type:
        mandatory: false
        default:
        description: 结束时间
        ranges:
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"hasNext\": false,\n\t\t\"hasPrev\": false,\n\t\t\"items\": [\n\t\t\t{\n\t\t\t\t\"afterAmount\": 0,\n\t\t\t\t\"amount\": 0,\n\t\t\t\t\"coin\": \"\",\n\t\t\t\t\"createdTime\": 0,\n\t\t\t\t\"id\": 0,\n\t\t\t\t\"side\": \"\",\n\t\t\t\t\"symbol\": \"\",\n\t\t\t\t\"type\": \"\"\n\t\t\t}\n\t\t]\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---