---
title: 获取listenKey
position_number: 1.1
type: post
description: /v1/user/listen-key
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
          "result": {},
          "returnCode": 0
        }
      title: Response
      language: json
---