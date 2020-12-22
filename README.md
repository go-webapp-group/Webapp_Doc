# Report
- [18342102 伍浩源报告](https://blog.csdn.net/weixin_44113352/article/details/111493937)
- [18342137 赵文序报告](https://blog.csdn.net/weixin_43504086/article/details/111490492)
- [18342139 周京有报告](https://blog.csdn.net/weixin_45960131/article/details/111414428)
- [18342140 周景伟报告](https://blog.csdn.net/weixin_43977005/article/details/111472413)
- [18342106 谢正雄报告]()

# Webapp-APIdocs

## API简单编写流程
   1. 通过浏览器访问swagger在线文档编辑器[https://editor.swagger.io/](https://editor.swagger.io/)（或使用本地swagger文档编辑器打开）。
   2. 按照`yaml`编辑格式对API文档进行编写或修改。
   3. 确认文档无误后，可以以多种方式导出这份文档（这里导出了源文件`swagger.yaml`和html2形式的`index.html`文件）。

## API overview
- `存放API的yaml文件`: swagger.yaml
- `生成API的html形式`: index.html
- 该API时按照`REST API v3`风格编写的关于一个简单购物车的实现。包括获取用户信息，上传商品信息、更新商品信息等API。

## API实例说明

#### 获取所有用户信息
``` bash
GET /users
```
##### Parameters

|Null|
|---|

##### Responses

|HTTP Code|Description|
|---|---|
|**200**|OK|


#### Produces

- `application/json`

#### 上传一个商品信息
``` bash
POST /commodities
```
##### Parameters

|Type|Name|Description|
|---|---|---|
|**string**|**name**  <br>*required*|The name of new commodity|
|**string**|**introduction**  <br>*required*|The introduction of new commodity|
|**string**|**picture**  <br>*required*|The picture of new commodity|
|**string**|**price**  <br>*required*|The price of new commodity|

##### Responses

|HTTP Code|Description|
|---|---|
|**200**|OK|

#### Produces

- `application/json`

## APIRoot
- 通过`GET /`可获取该API列表信息
- 不支持分页

