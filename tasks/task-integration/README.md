# 🍅 番茄钟游戏化浏览器插件

<div align="center">

**一款让你爱上专注的游戏化番茄钟**

[![GitHub license](https://img.shields.io/github/license/Levtain/pomodoro-game)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/Levtain/pomodoro-game)](https://github.com/Levtain/pomodoro-game/releases)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Levtain/pomodoro-game/pulls)

[English](README_EN.md) | 简体中文

</div>

---

## 📖 项目简介

这是一款**游戏化番茄钟浏览器插件**，通过深度游戏化、社交互动和智能推荐，解决现有番茄钟应用存在的"难以坚持"、"缺乏激励"、"功能单调"等核心痛点。

### 🎯 核心定位

> **"专注，也可以很有趣"**

### ✨ 核心特性

- 🎮 **深度游戏化体验** - 放置养成、RPG元素、成就系统
- 👥 **社交驱动** - 专注社区、好友PK、团队挑战
- 🤖 **智能推荐** - AI分析习惯、智能调整番茄时长
- 🎯 **数据可视化** - 专注效果分析、成就统计
- 🎨 **个性化主题** - 多种主题、自定义界面
- 🔄 **云端同步** - 多设备数据同步（高级版）

---

## 🚀 快速开始

### 安装插件

#### Chrome / Edge

1. 克隆项目到本地
```bash
git clone https://github.com/Levtain/pomodoro-game.git
cd pomodoro-game
```

2. 安装依赖
```bash
npm install
```

3. 构建插件
```bash
npm run build
```

4. 在浏览器中加载插件
   - 打开 `chrome://extensions/`
   - 开启"开发者模式"
   - 点击"加载已解压的扩展程序"
   - 选择 `dist` 文件夹

#### Firefox

1. 克隆项目并构建（同上）
2. 打开 `about:debugging#/runtime/this-firefox`
3. 点击"临时载入附加组件"
4. 选择 `dist` 目录下的 `.xpi` 文件

---

## 📸 功能演示

### 游戏化元素

```
┌─────────────────────────────────────┐
│         🎮 专注时间管理              │
├─────────────────────────────────────┤
│  ⭐ 等级: 15  💰 金币: 2,450         │
│  🎯 今日番茄: 8  ⏱️ 专注时长: 4小时   │
├─────────────────────────────────────┤
│  🎲 任务: 处理工作邮件               │
│  ⏰ 剩余时间: 18:25                  │
│  [暂停] [放弃] [完成]               │
├─────────────────────────────────────┤
│  🏆 最新成就                         │
│  🥇 专注达人 - 连续专注7天           │
│  🥈 早起鸟 - 早上完成3个番茄         │
└─────────────────────────────────────┘
```

### 游戏化系统

- 📈 **升级系统** - 完成番茄获得经验，提升等级
- 💰 **金币系统** - 完成任务获得金币，购买道具
- 🏆 **成就系统** - 完成挑战解锁成就徽章
- 🎨 **主题系统** - 解锁并使用精美主题
- 🐾 **宠物系统** - 养育你的专注伙伴（高级版）

---

## 🛠️ 技术栈

### 前端

- ⚛️ **React 18+** - UI框架
- ⚡ **Vite 5+** - 构建工具
- 🔷 **TypeScript** - 类型安全
- 🎨 **Tailwind CSS** - CSS框架
- 📦 **Zustand** - 状态管理
- 🎮 **Canvas API** - 游戏渲染

### 浏览器插件

- 🌐 **Chrome Extension Manifest V3** - 插件规范
- 🦊 **Firefox Extension** - 跨浏览器支持
- 🔧 **webextension-polyfill** - API统一

### 后端（高级版）

- 🟢 **Node.js** - 运行环境
- 🚂 **Express** - Web框架
- 🐘 **PostgreSQL** - 数据库
- 🔴 **Redis** - 缓存

---

## 📁 项目结构

```
pomodoro-game/
├── src/
│   ├── components/       # React组件
│   │   ├── PomodoroTimer/
│   │   ├── GameEngine/
│   │   ├── Achievement/
│   │   └── Theme/
│   ├── pages/           # 页面组件
│   │   ├── Popup/
│   │   ├── Options/
│   │   └── ContentScript/
│   ├── store/           # 状态管理
│   ├── game/            # 游戏引擎
│   │   ├── engine.ts    # 游戏循环
│   │   ├── state.ts     # 游戏状态
│   │   └── renderer.ts  # 渲染器
│   ├── utils/           # 工具函数
│   ├── hooks/           # 自定义Hooks
│   └── types/           # TypeScript类型
├── public/              # 静态资源
├── dist/                # 构建输出
├── scripts/             # 构建脚本
├── docs/                # 文档
└── tasks/               # 项目任务文档
    ├── task-market-research/      # 市场调研报告
    ├── task-tech-feasibility/     # 技术可行性报告
    └── task-integration/          # 方案整合（本目录）
```

---

## 🎮 核心功能

### 1. 番茄钟计时

- ⏱️ 标准25分钟工作 + 5分钟休息
- 🔄 支持自定义时长
- 📊 统计专注时长和番茄数
- 🔔 桌面通知提醒

### 2. 游戏化系统

#### 升级系统
- 完成番茄获得经验值
- 升级解锁新功能
- 等级显示和徽章

#### 金币系统
- 完成任务获得金币
- 金币可用于购买道具
- 每日签到奖励

#### 成就系统
- 多种成就类别
- 成就进度追踪
- 成就徽章展示

### 3. 社交功能（高级版）

- 👥 好友系统
- 🏆 排行榜
- 👊 好友PK
- 🌟 团队挑战

### 4. 智能推荐（高级版）

- 🤖 AI分析专注习惯
- 💡 智能推荐番茄时长
- 📊 专注效果分析
- 📈 趋势图和报表

### 5. 数据管理

- 💾 本地存储（MVP）
- ☁️ 云端同步（高级版）
- 📤 数据导出/导入
- 🔒 数据加密

---

## 📊 项目进度

### 当前阶段：MVP开发中

- [x] 市场调研报告
- [x] 技术可行性分析
- [x] 方案整合与Git仓库
- [ ] 项目初始化
- [ ] 基础架构搭建
- [ ] 番茄钟核心功能
- [ ] 游戏化系统
- [ ] UI/UX设计
- [ ] 测试与优化

### 开发计划

| 阶段 | 目标 | 周期 | 团队 |
|------|------|------|------|
| **MVP** | 验证核心假设 | 4-6周 | 1-2人 |
| **产品化** | 优化体验、扩大用户 | 8-12周 | 2-3人 |
| **规模化** | 生态建设、商业化升级 | 持续 | 3-5人 |

---

## 🤝 贡献指南

欢迎贡献代码、报告问题、提出建议！

### 如何贡献

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

### 开发规范

- 使用 TypeScript 编写代码
- 遵循 ESLint 规则
- 编写单元测试
- 更新相关文档

---

## 📜 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

---

## 🙏 致谢

- 感谢所有贡献者的付出
- 感谢 React 社区的支持
- 感谢 Chrome 和 Firefox 的插件生态

---

## 📞 联系我们

- 📧 邮箱：[待填写]
- 💬 Discord：[待填写]
- 🐦 Twitter：[待填写]
- 🌐 官网：[待填写]

---

<div align="center">

**⭐ 如果觉得这个项目有用，请给我们一个 Star！**

Made with ❤️ by the Pomodoro Game Team

</div>
