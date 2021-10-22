# 获取已有穿透隧道

### 接口描述

接口请求域名：lightart.top

此接口用于获取已经创建的穿透隧道。

### 传入参数

以下请求参数列表仅列出了接口请求参数，完整公共参数列表见 [公共请求参数](../../gong-gong-qing-qiu-can-shu.md)。

无附加参数。

### 输出参数



| 参数名称           | 类型      | 描述               |
| -------------- | ------- | ---------------- |
| id             | Integer | 隧道 ID            |
| name           | String  | 隧道名称             |
| protocol       | String  | 隧道协议             |
| custom\_domain | String  | 隧道域名（HTTP/HTTPS） |
| local\_address | String  | 本地地址             |
| remote\_port   | Integer | 远程端口             |
| client\_token  | String  | 程序 Token         |
| sk             | String  | XTCP 密钥          |
| status         | Integer | 隧道在线状态           |
| server\_id     | Integer | 隧道所属节点 ID        |
| project\_id    | Integer | 隧道所属项目 ID        |
| created\_at    | String  | 隧道创建时间           |
| updated\_at    | String  | 隧道最后更新时间         |
| ping           | String  | 隧道最后 Ping        |

### 示例

#### 输入示例

```
GET https://lightart.top/api/v1/_tunnels/
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
