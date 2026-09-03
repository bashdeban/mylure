# 🎣 路亚装备库 / Lure Tackle

纯本地、离线优先的路亚钓鱼装备管理与作钓分析工具。构建产物为单文件 HTML，双击即用，数据存于浏览器 IndexedDB，无需服务器与注册。

Pure-local, offline-first lure fishing tackle manager. Builds to a single HTML file — double-click to run, data stays in IndexedDB. No server, no sign-up.

# 🚀[点击这里直接使用](https://bashdeban.github.io/mylure/)
---

## 中文

### 功能

- **我的装备**：竿/轮/线/饵/钩/配件 六类档案，搜索与多级过滤，类型配色标识，一键复制
- **组合搭配**：自由搭配装备与 16 种内置钓组，实时兼容性检测（柄型匹配、投掷重量、线强等）与 0-100 评分
- **钓鱼计划**：多组合使用 + 分组合尾数，Open-Meteo 免费天气查询（含气压/风向）自动计算钓鱼指数与推荐时段
- **经验心得**：Markdown 撰写（六色高亮），关联钓组/水域/鱼种，全站点击即查
- **数据统计**：按时间段统计组合、地点（含时长/时均尾数/单次范围）及各装备使用率
- **其他**：中文/English/日本語 三语界面，手机端自适应，JSON 备份导入导出

### 快速开始

```bash
npm install
npm run build   # 产出单文件 dist/index.html，双击即离线使用
```

### 测试

```bash
npm test               # 数据层
npm run test:file      # 浏览器全流程（90+ 断言）
npm run test:migration # 数据库迁移
```

### 说明

- 数据仅在浏览器本地，请定期在「设置」导出 JSON 备份
- 天气查询需联网，其余功能完全离线
- 技术栈：Vue 3 + Dexie 4 + marked，运行时仅 3 个依赖

---

## English

### Features

- **Tackle**: rods / reels / lines / lures / hooks / accessories with search, filters, color-coded types, one-click duplicate
- **Combos**: pair gear with 16 built-in rigs; live compatibility checks (handle match, casting weight, line rating) with a 0–100 score
- **Trips**: multiple combos per trip with per-combo counts; free Open-Meteo weather (pressure/wind) auto-computes a fishing index and best hours
- **Notes**: Markdown notes (six-color highlights) linked to rigs / waters / species, clickable everywhere
- **Stats**: usage rankings by combo, location (hours, fish/hour, per-trip range) and gear across date ranges
- **More**: 中文/English/日本語 UI, mobile responsive, JSON backup import/export

### Quick Start

```bash
npm install
npm run build   # single-file dist/index.html, works offline via double-click
```

### Notes

- Data lives only in the browser — export JSON backups from Settings regularly
- Weather lookup needs internet; everything else is fully offline
- Stack: Vue 3 + Dexie 4 + marked — just 3 runtime dependencies
