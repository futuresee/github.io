## 获取单个交易对的配置信息


**接口地址**:`/v1/public/symbol/detail`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|symbol|symbol|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|CommonResponse«SymbolCacheDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|error||ErrorMessage|ErrorMessage|
|&emsp;&emsp;code||string||
|&emsp;&emsp;msg||string||
|msgInfo||string||
|result||SymbolCacheDTO|SymbolCacheDTO|
|&emsp;&emsp;baseCoin|标的资产|string||
|&emsp;&emsp;baseCoinDisplayPrecision|标的币种显示精度|integer(int32)||
|&emsp;&emsp;baseCoinPrecision|标的币种精度|integer(int32)||
|&emsp;&emsp;contractSize|合约乘数（面值）|number(bigdecimal)||
|&emsp;&emsp;contractType|合约类型，永续，交割|string||
|&emsp;&emsp;depthPrecisionMerge|盘口精度合并|integer(int32)||
|&emsp;&emsp;initLeverage|初始杠杆倍数|integer(int32)||
|&emsp;&emsp;labels|标签|array|string|
|&emsp;&emsp;liquidationFee|强平手续费|number(bigdecimal)||
|&emsp;&emsp;makerFee|maker手续费|number(bigdecimal)||
|&emsp;&emsp;maxEntrusts|最多open条件单|integer(int32)||
|&emsp;&emsp;maxOpenOrders|最多open订单|integer(int32)||
|&emsp;&emsp;minNotional|最小名义价值|number(bigdecimal)||
|&emsp;&emsp;minPrice|最小价格|number(bigdecimal)||
|&emsp;&emsp;minQty|最小数量|number(bigdecimal)||
|&emsp;&emsp;multiplierDown|限价卖单下限百分比|number(bigdecimal)||
|&emsp;&emsp;multiplierUp|限价买单价格上限百分比|number(bigdecimal)||
|&emsp;&emsp;onboardDate|上线时间|integer(int64)||
|&emsp;&emsp;pricePrecision|价格精度|integer(int32)||
|&emsp;&emsp;quantityPrecision|数量精度|integer(int32)||
|&emsp;&emsp;quoteCoin|报价资产|string||
|&emsp;&emsp;quoteCoinDisplayPrecision|报价币种显示精度|integer(int32)||
|&emsp;&emsp;quoteCoinPrecision|报价币种精度|integer(int32)||
|&emsp;&emsp;state|状态|integer(int32)||
|&emsp;&emsp;supportEntrustType|支持计划委托类型|string||
|&emsp;&emsp;supportOrderType|支持订单类型|string||
|&emsp;&emsp;supportTimeInForce|支持有效方式|string||
|&emsp;&emsp;symbol|交易对|string||
|&emsp;&emsp;takerFee|taker手续费|number(bigdecimal)||
|&emsp;&emsp;tradeSwitch|交易对开关|boolean||
|&emsp;&emsp;underlyingType|标的类型，币本位，u本位|string||
|returnCode||integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"error": {
		"code": "",
		"msg": ""
	},
	"msgInfo": "",
	"result": {
		"baseCoin": "",
		"baseCoinDisplayPrecision": 0,
		"baseCoinPrecision": 0,
		"contractSize": 0,
		"contractType": "",
		"depthPrecisionMerge": 0,
		"initLeverage": 0,
		"labels": [],
		"liquidationFee": 0,
		"makerFee": 0,
		"maxEntrusts": 0,
		"maxOpenOrders": 0,
		"minNotional": 0,
		"minPrice": 0,
		"minQty": 0,
		"multiplierDown": 0,
		"multiplierUp": 0,
		"onboardDate": 0,
		"pricePrecision": 0,
		"quantityPrecision": 0,
		"quoteCoin": "",
		"quoteCoinDisplayPrecision": 0,
		"quoteCoinPrecision": 0,
		"state": 0,
		"supportEntrustType": "",
		"supportOrderType": "",
		"supportTimeInForce": "",
		"symbol": "",
		"takerFee": 0,
		"tradeSwitch": false,
		"underlyingType": ""
	},
	"returnCode": 0
}
```