# 获取穿透隧道配置文件

### 接口描述

接口请求域名：lightart.top

此接口用于删除穿透隧道。

### 传入参数

以下请求参数列表仅列出了接口请求参数，完整公共参数列表见 [公共请求参数](../gong-gong-qing-qiu-can-shu.md)。

<table><thead><tr><th>参数名称</th><th data-type="checkbox">必选</th><th data-type="select">类型</th><th>描述</th></tr></thead><tbody><tr><td>None</td><td>true</td><td></td><td>隧道 ID</td></tr></tbody></table>

### 输出参数

<table><thead><tr><th>参数名称</th><th data-type="select">类型</th><th>描述</th></tr></thead><tbody><tr><td>None</td><td></td><td>配置文件</td></tr></tbody></table>

### 示例

#### 输入示例

```
GET https://lightart.top/api/v1/_tunnels/233
```

#### 输出示例

```ini
# 这是你的配置文件，请将它填入frpc.ini
[common]
server_addr = t.hk.s.awa.im
server_port = 1024
user = 1ec3016f-5a36-6f4a-95a6-02423ff14202
token = lightart_top


# LoliArt 在 西安高防服务器 的 Static 于服务器 香港转发服务器 1
[3|74|1ec3016f-5a36-6f4a-95a6-024232D14202]
type = tcp
local_ip = 127.0.0.1
local_port = 80
remote_port = 12345
```
