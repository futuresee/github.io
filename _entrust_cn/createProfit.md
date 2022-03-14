---
title: 创建止盈止损
position_number: 7
type: post
description: /v1/entrust/create-plan
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: 交易对
        ranges:
    -
        name: origQty
        type:
        mandatory: true
        default:
        description: 数量（张）
        ranges:
    -
        name: triggerProfitPrice
        type:
        mandatory: true
        default:
        description: 止盈触发价
        ranges:
    -
        name: triggerStopPrice
        type:
        mandatory: true
        default:
        description: 止损触发价
        ranges:
    -
        name: expireTime
        type:
        mandatory: true
        default:
        description: 过期时间
        ranges:
    -
        name: positionSide
        type:
        mandatory: true
        default:
        description: 仓位方向：LONG;SHORT
        ranges: LONG;SHORT
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---