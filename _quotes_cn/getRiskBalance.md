---
title: 获取交易对风险基金余额
position_number: 19
type: get
description: /v1/public/contract/risk-balance
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: 交易对
        ranges:
    -
        name: direction
        type:
        mandatory: false
        default: NEXT
        description: 方向（PREV:上一页；NEXT:下一页）
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
        description: 条数
        ranges:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"hasNext\": false,\n\t\t\"hasPrev\": false,\n\t\t\"items\": [\n\t\t\t{\n\t\t\t\t\"amount\": 0,\n\t\t\t\t\"coin\": \"\",\n\t\t\t\t\"createdTime\": 0,\n\t\t\t\t\"id\": 0\n\t\t\t}\n\t\t]\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---