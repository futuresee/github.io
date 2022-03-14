---
title: 撤销所有订单
position_number: 6
type: post
description: /v1/order/cancel-all
parameters:
  - name: symbol
    type: String
    mandatory: true
    default: N/A
    description: 交易对（不传时撤销所有交易对订单）
    ranges:
right_code_blocks:
  - code_block: "\t\"error\": {\n\t  \"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [],\n\t\"returnCode\": 0\n}"
    title: Response
    language: json
---