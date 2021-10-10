# 公共请求参数

公共参数是用于标识用户的参数，如非必要，在每个接口单独的接口文档中不再对这些参数进行说明，但每次请求均需要携带这些参数，才能正常发起请求。

### 公共参数

<table><thead><tr><th>参数名称</th><th data-type="checkbox">必选</th><th data-type="select">类型</th><th>描述</th></tr></thead><tbody><tr><td>api_token</td><td>true</td><td></td><td>用户 token</td></tr></tbody></table>

### 参数描述

#### api_token

在每个请求当中都必须包含的参数，用户可以在 Lae 的个人信息里点击 “更新访问密钥” 按钮获取 `token`，此值只会显示一次，如忘记此密钥，只能更新密钥，
