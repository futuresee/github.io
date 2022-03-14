---
title: 下单
position_number: 1
type: post
description: /v1/order/create
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default: N/A
        description: 交易对
        ranges:
    -
        name: orderSide
        type:
        mandatory: true
        default:
        description: 买卖方向：BUY;SELL
        ranges: BUY;SELL
    -
        name: orderType
        type:
        mandatory: true
        default:
        description: 订单类型：LIMIT；MARKET
        ranges: LIMIT；MARKET
    -
        name: origQty
        type:
        mandatory: true
        default:
        description: 数量（张）
        ranges:
    -
        name: marketOrderLevel
        type:
        mandatory: true
        default:
        description: 市价最优档：1：对手价；5，10，15挡
        ranges: 1;5;10;15
    -
        name: price
        type:
        mandatory: true
        default:
        description: 价格
        ranges:
    -
        name: reduceOnly
        type:
        mandatory: true
        default:
        description: 只减仓
        ranges:
    -
        name: timeInForce
        type:
        mandatory: true
        default:
        description: 有效方式：GTC;IOC;FOK;GTX
        ranges: GTC;IOC;FOK;GTX
    -
        name: triggerProfitPrice
        type:
        mandatory: true
        default:
        description: 止盈价
        ranges:
    -
        name: triggerStopPrice
        type:
        mandatory: true
        default:
        description: 止损价
        ranges:
    -
        name: positionSide
        type:
        mandatory: true
        default:
        description: 仓位方向：LONG;SHORT
        ranges: LONG;SHORT
content_markdown: 注：**此方法不需要签名**
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