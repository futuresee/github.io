---
title: 查询成交明细
position_number: 1.1
type: get
description: /v1/order/trade-list
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
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"items\": [\n\t\t\t{\n\t\t\t\t\"fee\": 0,\n\t\t\t\t\"feeCoin\": \"\",\n\t\t\t\t\"orderId\": 0,\n\t\t\t\t\"price\": 0,\n\t\t\t\t\"quantity\": 0,\n\t\t\t\t\"symbol\": \"\",\n\t\t\t\t\"timestamp\": 0\n\t\t\t}\n\t\t],\n\t\t\"page\": 0,\n\t\t\"ps\": 0,\n\t\t\"total\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---