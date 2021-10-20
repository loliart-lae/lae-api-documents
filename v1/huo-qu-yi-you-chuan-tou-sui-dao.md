# 获取已有穿透隧道

### 接口描述

接口请求域名：lightart.top

此接口用于获取已经创建的穿透隧道。

### 传入参数

以下请求参数列表仅列出了接口请求参数，完整公共参数列表见 [公共请求参数](../gong-gong-qing-qiu-can-shu.md)。

无附加参数。

### 输出参数

<table><thead><tr><th>参数名称</th><th data-type="select">类型</th><th>描述</th></tr></thead><tbody><tr><td>id</td><td></td><td>隧道 ID</td></tr><tr><td>name</td><td></td><td>隧道名称</td></tr><tr><td>protocol</td><td></td><td>隧道协议</td></tr><tr><td>custom_domain</td><td></td><td>隧道域名（HTTP/HTTPS）</td></tr><tr><td>local_address</td><td></td><td>本地地址</td></tr><tr><td>remote_port</td><td></td><td>远程端口</td></tr><tr><td>client_token</td><td></td><td>程序 Token</td></tr><tr><td>sk</td><td></td><td>XTCP 密钥</td></tr><tr><td>status</td><td></td><td>隧道在线状态</td></tr><tr><td>server_id</td><td></td><td>隧道所属节点 ID</td></tr><tr><td>project_id</td><td></td><td>隧道所属项目 ID</td></tr><tr><td>created_at</td><td></td><td>隧道创建时间</td></tr><tr><td>updated_at</td><td></td><td>隧道最后更新时间</td></tr><tr><td>ping</td><td></td><td>隧道最后 Ping</td></tr></tbody></table>

### 示例

#### 输入示例

```
GET https://lightappengine.test/api/v1/_tunnels/
```

#### 输出示例

```json
{
    "status":1,
    "data":[
        {
            "id":5,
            "name":"Go",
            "protocol":"xtcp",
            "custom_domain":null,
            "local_address":"127.0.0.1:80",
            "remote_port":null,
            "client_token":"1ec15111-d621-6994-b550-65b284bbf32a",
            "sk":"123456",
            "status":0,
            "server_id":3,
            "project_id":1,
            "created_at":"2021-09-14T04:06:19.000000Z",
            "updated_at":"2021-10-18T13:32:15.000000Z",
            "ping":"2021-10-18 21:32:15"
        },
        {
            "id":77,
            "name":"Static",
            "protocol":"tcp",
            "custom_domain":null,
            "local_address":
            "127.0.0.1:80",
            "remote_port":41002,
            "client_token":"1ec3016f-5a36-6f4a-95a6-02423ff14302",
            "sk":null,
            "status":0,
            "server_id":3,
            "project_id":1,
            "created_at":"2021-10-18T13:26:11.000000Z",
            "updated_at":"2021-10-18T13:31:36.000000Z",
            "ping":"2021-10-18 21:31:36"
        },
        {
            "id":46,
            "name":"Test",
            "protocol":"https",
            "custom_domain":"www.yistars.net",
            "local_address":"127.0.0.1:443",
            "remote_port":0,
            "client_token":"1ec29183-9b5c-6ca6-8b33-02423ff14202",
            "sk":null,
            "status":0,
            "server_id":3,
            "project_id":8,
            "created_at":"2021-10-09T15:47:36.000000Z",
            "updated_at":"2021-10-09T15:47:36.000000Z",
            "ping":null
        }
    ]
}
```
