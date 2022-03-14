---
title: 修改止盈止损
position_number: 12
type: post
description: /v1/entrust/update-profit-stop
parameters:
  - name: profitId
    type:
    mandatory: true
    default:
    description: 止盈止损id
    ranges:
  - name: triggerProfitPrice
    type:
    mandatory: false
    default:
    description: 止盈触发价
    ranges:
  - name: triggerStopPrice
    type:
    mandatory: false
    default:
    description: 止损触发价
    ranges:
right_code_blocks:
  - code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {},\n\t\"returnCode\": 0\n}"
    title: Response
    language: json
---