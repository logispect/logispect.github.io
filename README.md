# Tool Haven

本地运行的小工具合集。浏览器内完成计算，不上传敏感数据。

## 结构

```
index.html                 ← 首页目录
css/app.css                ← 共用样式
tools/password.html        ← 密码生成器
tools/json.html            ← JSON 格式化
tools/currency.html        ← 汇率转换
tools/timestamp.html       ← 时间戳互转
tools/base.html            ← 进制转换
ads.txt
```

旧链接 `#tool-password` / `#tool-json` / `#tool-currency` / `#tool-timestamp` / `#tool-base` 会在首页自动跳到对应工具页。

## 本地打开

双击 `index.html`，或用任意静态服务器打开项目根目录。

汇率工具若用 `file://` 打开可能无法请求外网接口，建议用本地服务器，或访问已部署站点。

## 设计

- 配色：Graphite（近黑字 + 翠绿 `#0f7a5a`）
- 内容区限宽约 880px，宽屏双列目录

## 汇率转换说明

- 金额换算在本地完成；仅拉取公开汇率表
- 数据源优先：jsDelivr（currency-api）→ open.er-api → Frankfurter
- 表缓存于 `localStorage`，默认 12 小时内复用；拿不到汇率则不换算
