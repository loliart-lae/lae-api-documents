# 获取用户的项目

### 接口描述

接口请求域名：lightart.top

此接口用于获取用户拥有权限的项目。

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

### 示例

#### 输入示例

```
GET https://lightart.top/api/v1/_projects
```

#### 输出示例

```json
{
    "status":0,
    "data":[
        {
            "id":8,
            "user_id":2,
            "project_id":8,
            "joined":1,
            "created_at":"2021-09-09T14:42:11.000000Z",
            "updated_at":"2021-09-09T14:42:11.000000Z",
            "project":
            {
                "id":8,
                "name":"\u51b0\u781a\u70bd",
                "description":"\u6d4b\u8bd5\u9879\u76ee",
                "user_id":2,
                "created_at":"2021-09-09T14:42:11.000000Z",
                "updated_at":"2021-10-23T04:59:04.000000Z",
                "balance":446640.4868
            }
        },{
            "id":18,
            "user_id":2,
            "project_id":1,
            "joined":1,
            "created_at":"2021-09-11T16:23:09.000000Z",
            "updated_at":"2021-09-11T16:23:09.000000Z",
            "project":
            {
                "id":1,
                "name":"LoliArt",
                "description":"\u6d1b\u4e3d\u827a\u7f8e \u5728 \u897f\u5b89\u9ad8\u9632\u670d\u52a1\u5668",
                "user_id":1,
                "created_at":"2021-09-09T12:27:41.000000Z",
                "updated_at":"2021-10-23T04:59:04.000000Z",
                "balance":1504.3499
            }
        }
    ]
}
```
