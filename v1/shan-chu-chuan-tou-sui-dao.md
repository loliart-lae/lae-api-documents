# 删除穿透隧道

### 接口描述

接口请求域名：lightart.top

此接口用于删除穿透隧道。

### 传入参数

以下请求参数列表仅列出了接口请求参数，完整公共参数列表见 [公共请求参数](../gong-gong-qing-qiu-can-shu.md)。

<table><thead><tr><th>参数名称</th><th data-type="checkbox">必选</th><th>类型</th><th>描述</th></tr></thead><tbody><tr><td>None</td><td>true</td><td>String</td><td>隧道 ID</td></tr></tbody></table>

### 输出参数

| 参数名称 | 类型     | 描述        |
| ---- | ------ | --------- |
| None | String | 被删除的隧道 ID |

### 示例

#### 输入示例

```
DELETE https://lightart.top/api/v1/_tunnels/233
```

#### 输出示例

```json
{
    "status": 1,
    "data": "233"
}
```
