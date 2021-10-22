# 添加穿透隧道

### 接口描述

接口请求域名：lightart.top

此接口用于添加穿透隧道。

### 传入参数

以下请求参数列表仅列出了接口请求参数，完整公共参数列表见 [公共请求参数](../../gong-gong-qing-qiu-can-shu.md)。

<table><thead><tr><th>参数名称</th><th data-type="checkbox">必选</th><th>类型</th><th>描述</th></tr></thead><tbody><tr><td>name</td><td>true</td><td>String</td><td>隧道名称</td></tr><tr><td>protocol</td><td>true</td><td>String</td><td>隧道协议</td></tr><tr><td>local_address</td><td>true</td><td>String</td><td>本地地址，包含端口</td></tr><tr><td>project_id</td><td>true</td><td>Integer</td><td>项目 ID</td></tr><tr><td>server_id</td><td>true</td><td>Integer</td><td>服务器 ID</td></tr><tr><td>custom_domain</td><td>false</td><td>String</td><td>域名，Http(s) 须填写</td></tr></tbody></table>

### 输出参数

<table><thead><tr><th>参数名称</th><th data-type="select">类型</th><th>描述</th></tr></thead><tbody><tr><td>name</td><td></td><td></td></tr><tr><td>protocol</td><td></td><td></td></tr><tr><td>local_address</td><td></td><td></td></tr><tr><td>remote_port</td><td></td><td></td></tr><tr><td>custom_domain</td><td></td><td></td></tr></tbody></table>

### 示例

#### 输入示例

```
POST https://lightart.top/api/v1/tunnels?name=test_api
&protocol=http
&local_address=localhost:80
&project_id=1
&server_id=3
&custom_domain=helloworld.com
```

#### 输出示例
