# docs

# 何把jar发布到中央仓库 
#参考 
https://www.jdon.com/idea/publish-to-center-maven.html
https://blog.csdn.net/huangjinjin520/article/details/78915789

https://oss.sonatype.org/
https://issues.sonatype.org/login.jsp
注册邮箱：xjch7703@163.com
(real name)用户名：xjch
密码：X&1**5**&j**
#创建新问题
https://issues.sonatype.org/browse/OSSRH-48196
#申请结果
com.github.xjch has been prepared, now user(s) xjch can:
Deploy snapshot artifacts into repository 
https://oss.sonatype.org/content/repositories/snapshots

Deploy release artifacts into the staging repository 
https://oss.sonatype.org/service/local/staging/deploy/maven2

Promote staged artifacts into repository 'Releases'
Download snapshot and release artifacts from group 
https://oss.sonatype.org/content/groups/public

Download snapshot, release and staged artifacts from staging group 
https://oss.sonatype.org/content/groups/staging

please comment on this ticket when you promoted your first release, thanks


mvn dependency:get -DrepoUrl=http://repo.maven.apache.org/maven2/ -Dartifact=org.apache.maven.plugins:maven-gpg-plugin:1.6
mvn dependency:get -DrepoUrl=http://repo.maven.apache.org/maven2/ -Dartifact=org.apache.maven.plugins:maven-source-plugin:3.0.1
mvn dependency:get -DrepoUrl=http://repo.maven.apache.org/maven2/ -Dartifact=org.sonatype.plugins:nexus-staging-maven-plugin:1.6.7


*  规划的响应字段说明

| 名称  | 类型  | 说明 |Description|
|---|---|---|---|
| reqResult | boolean | 请求成功与否。true:请求成功；false请求失败 |request result|
| respErrorCode | string | 请求返回的错误编码。 00000000表示success，非00000000表示失败错误 |error code. 00000000 represent success, >00000000 represent failure code |
| respErrorMsg | string | 请求失败返回的错误信息 |error message from failed request|
| repsResult | object| 请求返回的数据 |return data|
