# 添加穿透隧道

### 接口描述

接口请求域名：lightart.top

此接口用于添加穿透隧道。

### 传入参数

<table><thead><tr><th>参数名称</th><th data-type="checkbox">必选</th><th data-type="select">类型</th><th>描述</th></tr></thead><tbody><tr><td>name</td><td>true</td><td></td><td>隧道名称</td></tr><tr><td>protocol</td><td>true</td><td></td><td>隧道协议</td></tr><tr><td>local_address</td><td>true</td><td></td><td>本地地址，包含端口</td></tr><tr><td>project_id</td><td>true</td><td></td><td>项目 ID</td></tr><tr><td>server_id</td><td>true</td><td></td><td>服务器 ID</td></tr><tr><td>custom_domain</td><td>true</td><td></td><td>域名，仅限 Http 协议</td></tr></tbody></table>

### 输出参数

<table><thead><tr><th>参数名称</th><th data-type="select">类型</th><th>描述</th></tr></thead><tbody><tr><td></td><td></td><td></td></tr><tr><td></td><td></td><td></td></tr></tbody></table>

### 示例

#### 输入示例

```
https://lightappengine.test/api/v1/tunnels?name=test_api
&protocol=http
&local_address=localhost:80
&project_id=1
&server_id=3
&custom_domain=helloworld.com
```

#### 输出示例

