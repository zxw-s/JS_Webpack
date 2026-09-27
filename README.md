# Webpack Frontend Project

> 基于 Webpack 打包的前端项目，支持 JavaScript / TypeScript。仓库仅提交源码，**不包含 node_modules、打包产物、本地环境配置与密钥信息**。

## 📖 项目简介

本项目使用 Webpack 作为模块打包工具，可用于 Vue / React / 原生JS项目。
支持模块打包、资源处理、代码压缩、热更新开发服务。

## 🧰 环境依赖

- Node.js >= 16.0
- 包管理器：npm / pnpm / yarn
- IDE：VS Code

## 📂 目录结构

```plaintext
.
├── public/ -- 静态资源
├── src/
│ ├── assets/ -- 图片、字体等资源
│ ├── components/ -- 组件
│ ├── pages/ -- 页面
│ ├── js/ -- 业务脚本
│ ├── style/ -- 样式文件
│ └── index.js -- 入口文件
├── webpack.config.js -- Webpack配置
├── package.json
├── .env.example -- 环境变量模板
├── .gitignore
└── README.md
```

## ⚙️ 项目命令

```bash
# 安装依赖
pnpm install

# 启动开发服务（热更新）
pnpm dev

# 生产环境打包
pnpm build
```

## 📌 开发规范

1. 环境变量：`.env.example` 提交模板，本地真实环境文件 `.env` / `.env.local` **禁止提交**
2. 前端代码严禁硬编码后端密钥、Token、数据库账号密码
3. 文件编码统一 UTF-8
4. 提交前执行 `pnpm build`，确认打包无报错

## ❗ 重要提醒

- `node_modules`、`dist` 打包产物由 gitignore 忽略，不上传仓库
- 前端代码浏览器可直接查看，敏感信息不能写在前端代码
- 大型静态资源谨慎提交到GitHub仓库

## ✅ GitHub提交自查清单

提交代码前逐项检查：

1. 代码中不存在密钥、token、隐私业务数据
2. 没有提交 node_modules、dist、build 产物
3. 没有提交本地环境变量文件 `.env` `.env.local`
4. 文件编码统一 UTF-8
5. 本地打包、运行验证通过
6. .gitignore 配置生效，检查待提交文件列表

## 📜 License

MIT
