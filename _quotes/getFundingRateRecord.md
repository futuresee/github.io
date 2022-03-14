---
title: 获取资金费率记录
position_number: 18
type: get
description: /v1/public/q/funding-rate-record
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
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"fundingRate\": 0,\n\t\t\"nextCollectionTime\": 0,\n\t\t\"symbol\": \"\"\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---