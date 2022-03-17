---
title: 取消收藏交易对
position_number: 14
type: post
description: /v1/user/collection/cancel
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: 交易对（不传时查询所有交易对的持仓信息）
        ranges:
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
        "result": true,
        "returnCode": 0
      }
    title: Response
    language: json
---