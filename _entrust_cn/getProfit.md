---
title: 查询止盈止损
position_number: 10
type: get
description: /v1/entrust/profit-list
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default: N/A
        description: "交易对（不传时撤销所有交易对）\t"
        ranges:
    -
        name: page
        type: integer
        mandatory: false
        default: 1
        description: 页码
        ranges:
    -
        name: size
        type: integer
        mandatory: false
        default: 10
        description: 单页数
        ranges:
    -
        name: startTime
        type: integer
        mandatory: false
        default: N/A
        description: 开始时间
        ranges:
    -
        name: endTime
        type: integer
        mandatory: false
        default: N/A
        description: 结束时间
        ranges:
    -
        name: state
        type:
        mandatory: true
        default:
        description: >-
            委托状态
            NOT_TRIGGERED：新建委托（未触发）；TRIGGERING：触发中；TRIGGERED：已触发；USER_REVOCATION：用户撤销；PLATFORM_REVOCATION：平台撤销（拒绝）；EXPIRED：已过期；UNFINISHED：未完成；HISTORY：（历史）
        ranges: >-
            NOT_TRIGGERED;TRIGGERING;TRIGGERED;USER_REVOCATION;PLATFORM_REVOCATION;EXPIRED;UNFINISHED;HISTORY
    
left_code_blocks:
    -
        code_block: "public void getMarketConfig() {\r\n\tString text = HttpUtil.get(URL + \"/data/api/v1/getMarketConfig\");\r\n\tSystem.out.println(text);\r\n}"
        title: Java
        language: java
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"items\": [\n\t\t\t{\n\t\t\t\t\"createdTime\": 0,\n\t\t\t\t\"entryPrice\": 0,\n\t\t\t\t\"executedQty\": 0,\n\t\t\t\t\"isolatedMargin\": 0,\n\t\t\t\t\"origQty\": 0,\n\t\t\t\t\"positionSide\": \"\",\n\t\t\t\t\"positionSize\": 0,\n\t\t\t\t\"profitId\": 0,\n\t\t\t\t\"state\": \"\",\n\t\t\t\t\"symbol\": \"\",\n\t\t\t\t\"triggerProfitPrice\": 0,\n\t\t\t\t\"triggerStopPrice\": 0\n\t\t\t}\n\t\t],\n\t\t\"page\": 0,\n\t\t\"ps\": 0,\n\t\t\"total\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: json
---