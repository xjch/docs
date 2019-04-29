# docs

# 何把jar发布到中央仓库 
#参考 
https://blog.csdn.net/huangjinjin520/article/details/78915789
https://oss.sonatype.org/
https://issues.sonatype.org/login.jsp
注册邮箱：xjch7703@163.com
用户名：xjch
密码：X&1**5**&j**

*  规划的响应字段说明

| 名称  | 类型  | 说明 |Description|
|---|---|---|---|
| success | boolean | 请求成功与否。true:请求成功；false请求失败 |request result|
| errorCode | string | 错误编码。 00000000表示success，非00000000表示失败错误 |error code. 00000000 represent success, >00000000 represent failure code |
| errorMsg | string | 请求失败返回的错误信息 |error message from failed request|
| result | object| 请求返回的数据 |return data|
