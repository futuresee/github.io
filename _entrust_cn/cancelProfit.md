---
title: 撤销止盈止损
position_number: 8
type: post
description: /v1/entrust/cancel-profit-stop
parameters:
    -
        name: profitId
        type: integer
        mandatory: true
        default: N/A
        description: 止盈止损id
        ranges:
left_code_blocks:
    -
        code_block: "public void getKLine() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getKLine?market=btc_usdt&type=1min&since=0\");\r\n\tSystem.out.println(text);\r\n}"
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