# 股票投资分析系统

一个简单高效的个人股票投资分析工具，帮助个人投资者管理持仓、追踪收益。

## 功能特性

| 模块 | 功能 |
|------|------|
| **持仓管理** | 添加/删除股票持仓，支持股票代码搜索 |
| **收益看板** | 实时计算盈亏、收益率，展示汇总数据 |
| **新闻快讯** | 根据持仓股票显示相关财经新闻 |
| **数据管理** | 导出 CSV/JSON，导入 JSON 备份 |

## 项目结构

```
StockV2.0/
├── docs/              # GitHub Pages 静态页面
├── stock-app/         # React 主应用
│   ├── src/
│   │   ├── components/
│   │   │   ├── ui/              # 基础 UI 组件
│   │   │   └── dashboard/       # 业务组件
│   │   ├── services/            # 数据服务
│   │   ├── types/               # TypeScript 类型定义
│   │   └── utils/               # 工具函数
│   └── package.json
└── .github/
    └── workflows/               # GitHub Actions 工作流
```

## 快速开始

### 运行应用

```bash
cd stock-app
npm install
npm run dev
```

然后在浏览器打开 http://localhost:5173/

### 构建生产版本

```bash
npm run build
```

## 技术栈

- **前端框架**: React 18 + TypeScript
- **构建工具**: Vite
- **UI 库**: Tailwind CSS + shadcn/ui
- **图标**: Lucide React

## 在线演示

项目已部署至 GitHub Pages: [查看演示](https://tomking.github.io/StockV2.0/)

## 支持的股票代码

系统内置了以下 A 股常见股票用于测试（使用模拟数据）：

| 代码 | 名称 |
|------|------|
| 600519.SH | 贵州茅台 |
| 000858.SZ | 五粮液 |
| 600036.SH | 招商银行 |
| 601318.SH | 中国平安 |
| 000333.SZ | 美的集团 |
| 600276.SH | 恒瑞医药 |
| 002594.SZ | 比亚迪 |

> 注意：当前版本使用模拟数据，后续可接入真实 API

## 许可证

MIT License

---

**免责声明**: 本项目仅供学习和研究使用，数据不构成投资建议。
