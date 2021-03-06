# 中文 era 游戏版本信息数据中心 API（临时）

## 使用方法

### 获取最新版本信息

GET `api.erag.eu.org/游戏名/version`

### 前往该文件的网盘页面

GET `api.erag.eu.org/游戏名/file`

### 直接下载最新版本游戏

GET `api.erag.eu.org/游戏名/download`

## Todo

- [x] Auto CI/CD Workflow (GitHub Action)
- [x] 接入 Cloudflare KV 数据库
- [ ] 设计 Token 鉴权和 fail to ban 机制（考虑 IP 白名单）
- [x] `/游戏名/download` 统一跳转到下载分流 CDN
- [ ] `/游戏名/version` 判断 UA，如果是浏览器就渲染全部信息，否则只返回版本号和下载链接

### 长期目标

- [x] 将当前的临时域名（`era-data.lackb.fun`）替换为正式域名（`api.erag.eu.org`）
- [ ] 将当前的临时架构（Cloudflare Worker）替换为正式网站后端 API（技术栈待定）
