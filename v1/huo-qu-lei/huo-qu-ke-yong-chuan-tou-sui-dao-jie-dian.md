# 获取可用穿透隧道节点

### 接口描述

接口请求域名：lightart.top

此接口用于获取可供创建隧道的节点。

### 传入参数

以下请求参数列表仅列出了接口请求参数，完整公共参数列表见 [公共请求参数](../../gong-gong-qing-qiu-can-shu.md)。

无附加参数。

### 输出参数

| 参数名称           | 类型      | 描述          |
| -------------- | ------- | ----------- |
| id             | Integer | 节点 ID       |
| name           | String  | 节点名称        |
| domain         | String  | 节点域名        |
| price          | Float   | 节点价格（积分/分钟） |
| network\_limit | Integer | 节点共享网络带宽    |

### 示例

#### 输入示例

```
GET https://lightart.top/api/v1/_tunnels/create
```

#### 输出示例

```json
{
    "status":1,
    "data":[
        {
            "id":3,
            "name":"\u9999\u6e2f\u8f6c\u53d1\u670d\u52a1\u5668 1",
            "domain":"t.hk.s.awa.im",
            "price":0.012,
            "network_limit":30
        },{
            "id":4,
            "name":"\u7f8e\u56fdGIA \u975e\u6b63\u5f0f\u670d\u52a1\u5668",
            "domain":"t.us-gia.sp.s.awa.im",
            "price":0.01,
            "network_limit":10
        }
    ]
}
```
