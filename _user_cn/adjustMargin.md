---
title: 修改保证金
position_number: 9
type: post
description: /v1/position/margin
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: 交易对（不传时查询所有交易对的持仓信息）
        ranges:
    -
        name: margin
        type: number
        mandatory: false
        default: N/A
        description: 数量
        ranges:
    -
        name: positionSide
        type: string
        mandatory: false
        default: N/A
        description: 持仓方向：LONG;SHORT
        ranges:
    -
        name: type
        type: string
        mandatory: false
        default: N/A
        description: 调整方向（ADD：增加逐仓保证金；SUB：减少逐仓保证金）
        ranges: ADD;SUB
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    - code_block: |-
      {
        "error": {
          "code": "",
          "msg": ""
        },
        "msgInfo": "",
        "result": {},
        "returnCode": 0
      }
    title: Response
    language: json
---