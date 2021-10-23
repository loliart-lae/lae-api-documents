# 获取用户的项目

### 接口描述

接口请求域名：lightart.top

此接口用于获取用户拥有权限的项目。

### 传入参数

以下请求参数列表仅列出了接口请求参数，完整公共参数列表见 [公共请求参数](../../gong-gong-qing-qiu-can-shu.md)。

无附加参数。

### 输出参数

| 参数名称                | 类型      | 描述               |
| ------------------- | ------- | ---------------- |
| id                  | Integer | 用户在该项目中的 ID      |
| user\_id            | Integer | 用户 ID            |
| project\_id         | Integer | 项目 ID            |
| created\_at         | String  | 隧道域名（HTTP/HTTPS） |
| updated\_at         | String  | 用户创建时间           |
| remote\_port        | String  | 用户更新时间           |
| project.id          | Integer | 项目 ID            |
| project.name        | String  | 项目名称             |
| project.description | String  | 项目描述             |
| project.user\_id    | Integer | 项目创建者 ID         |
| project.created\_at | String  | 项目创建时间           |
| project.updated\_at | String  | 项目更新时间           |
| project.balance     | Float   | 项目积分余额           |

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
