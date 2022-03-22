---
title: WEBSOCKET API
position_number: 1
type:
description:
parameters:
    -
        name:
        type:
        mandatory: false
        default:
        description:
        ranges:
content_markdown: |-
    正式:

    wss://xtsocket.xt.com/websocket
    
    行情ws订阅地址:  https://xxx.xxx.xxx/ws/market
    
    用户ws订阅地址:  https://xxx.xxx.xxx/ws/user
    
     客户端订阅行情的时候，创建俩个链接，一个链接只订阅交易对信息和K线信息
     
     ({"req":"sub_symbol","symbol":"btc_usdt"}
     
     {"req":"sub_kline","symbol":"btc_usdt","type":"1m"})
     
     另一个订阅其他的行情
     
     {"req":"sub_ticker","symbol":"btc_usdt,eth_usdt"}
     
     {"req":"sub_mark_price","symbol":"btc_usdt,eth_usdt"})

left_code_blocks:
-
    code_block:
    title:
    language:
right_code_blocks:
-
    code_block:
    title:
    language:
---
