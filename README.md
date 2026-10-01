# Tool Haven

本地运行的小工具合集。浏览器内完成计算，不上传数据。

## 页面

| 入口 | 说明 |
|------|------|
| `index.html` | 首页 + 全部工具（hash 同页切换） |
| `index.html#tool-password` | 密码生成器 |
| `index.html#tool-json` | JSON 格式化 / 校验 / 压缩 |
| `password-generator.html` | 跳转到 `#tool-password` |

路由统一前缀 `tool-`，例如 `#tool-json`，避免裸 `#json` 等歧义。

## 本地打开

双击 `index.html`，或用任意静态服务器打开项目根目录。

## 设计

- 配色：Graphite（近黑字 + 翠绿 `#0f7a5a`）
- 内容区限宽约 880px，宽屏双列目录
