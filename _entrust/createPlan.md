---
title: 创建计划委托
position_number: 1
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
        name: orderSide
        type:
        mandatory: true
        default:
        description: 买卖方向：BUY;SELL
        ranges: BUY;SELL
    -
        name: entrustType
        type:
        mandatory: true
        default:
        description: >-
            委托类型：TAKE_PROFIT(止盈限价单)；STOP(止损限价单)；TAKE_PROFIT_MARKET（止盈市价单）；STOP_MARKET（止损市价单）；TRAILING_STOP_MARKET（跟踪止损单）
        ranges: TAKE_PROFIT;STOP;TAKE_PROFIT_MARKET;STOP_MARKET;TRAILING_STOP_MARKET
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
        name: stopPrice
        type:
        mandatory: true
        default:
        description: 触发价
        ranges:
    -
        name: timeInForce
        type:
        mandatory: true
        default:
        description: 有效方式：GTC;IOC;FOK;GTX
        ranges: GTC;IOC;FOK;GTX
    -
        name: triggerPriceType
        type:
        mandatory: true
        default:
        description: 触发价格类型：INDEX_PRICE(指数价格)；MARK_PRICE(标记价格)；LATEST_PRICE(最新价格)
        ranges: INDEX_PRICE;MARK_PRICE;LATEST_PRICE
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