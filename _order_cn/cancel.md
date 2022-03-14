---
title: 撤销订单
position_number: 5
type: post
description: /v1/order/cancel
parameters:
  - name: orderId
    type: Integer
    mandatory: true
    default: N/A
    description: 订单id
    ranges:
right_code_blocks:
  - code_block: "\t\"error\": {\n\t  \"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [],\n\t\"returnCode\": 0\n}"
    title: Response
    language: json
---