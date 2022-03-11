---
title: 交易对配置
position_number: 1.3
type: get
description: v1/public/symbol/coins
parameters:
  name: market
  type: string
  mandatory: true
  default: N/A
  description: 交易市场
  ranges: btc_usdt, eth_usdt...
content_markdown: 注：**此方法不需要签名**
right_code_blocks:
  - code_block: "\n	\"error\": {\n		\"code\": \"\",\n		\"msg\": \"\"\n	},\n	\"msgInfo\": \"\",\n	\"result\": [],\n	\"returnCode\": 0\n}"
    title: Response
    language: json
---
