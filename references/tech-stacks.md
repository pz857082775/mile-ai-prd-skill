# 技术栈推荐（按项目类型）

每个类型给：推荐栈 / 备选栈 / 不适用栈 / 选型理由 / 成本。默认偏好降本与可维护。

## PC 网站（管理后台 / 官网 / SaaS）
- 推荐：React/Vue3 + TypeScript + Node(NestJS)/Go + PostgreSQL + Tailwind/shadcn
- 备选：Next.js 全栈；Java(Spring Boot) + Vue
- 不适用：纯静态无后端交互时避免过度工程
- 理由：组件化、生态成熟、SEO 友好（Next）
- 成本：中

## H5（移动端网页 / 活动页 / 嵌入微信）
- 推荐：Vue3 + Vant / React + antd-mobile；Vite 构建
- 备选：uni-app（一套代码多端）
- 注意：移动端适配（rem/vw）、微信 JS-SDK 域名校验、首屏性能
- 成本：低-中

## 微信小程序
- 推荐：Taro / uni-app（React/Vue 语法，跨端）或 小程序原生
- 备选：原生 + 云开发（快速起步）
- 不适用：重度游戏用小程序游戏原生/Cocos
- 理由：跨端复用、开发快；云开发免运维
- 成本：中（需类目资质/审核）

## 微信小游戏
- 推荐：Cocos Creator / LayaAir（可视化+跨端）；或 小程序游戏原生 + Canvas
- 备选：Three.js（3D）
- 合规：版号、实名、防沉迷、广告规范
- 成本：中-高

## 网页小游戏
- 推荐：Canvas/WebGL + Phaser（2D）/ Three.js（3D）；TypeScript
- 备选：PixiJS（2D 高性能）
- 理由：无需上架，迭代快；注意首包体积与帧率
- 成本：中

## iOS APP
- 推荐：Swift + SwiftUI（原生）或 Flutter（跨端）
- 备选：React Native
- 合规：App Store 审核指南、HIG、IAP、隐私清单、ATT 弹窗
- 成本：高（上架周期、账号年费）

## Android APP
- 推荐：Kotlin + Jetpack Compose（原生）或 Flutter（跨端）
- 备选：React Native
- 合规：Material、Play 政策、权限最小化、SDK 合规
- 成本：高

## 跨端统一后台（多端共用）
- 推荐：Node(NestJS)/Go + PostgreSQL + Redis；API 网关统一鉴权
- 部署：云厂商/容器/Vercel(Serverless)
- 多端一致性：前端各自适配，共享 OpenAPI 契约
