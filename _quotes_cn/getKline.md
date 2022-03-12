---
title: 获取交易对的k线信息
position_number: 14
type: get
description: /v1/public/q/kline
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: 交易对
        ranges:
    -
        name: interval
        type:
        mandatory: true
        default:
        description: 时间间隔
        ranges: 1m;5m;15m;30m;1h;4h;1d;1w
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
    -
        name: limit
        type:
        mandatory: false
        default:
        description: 限制条数
        ranges:
content_markdown: 注：**此方法不需要签名**
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"a\": 0,\n\t\t\t\"c\": 0,\n\t\t\t\"h\": 0,\n\t\t\t\"l\": 0,\n\t\t\t\"o\": 0,\n\t\t\t\"s\": \"\",\n\t\t\t\"t\": 0,\n\t\t\t\"v\": 0\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---