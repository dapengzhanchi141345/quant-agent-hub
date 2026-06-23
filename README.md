# Quant Agent Hub 💹

**量化交易 AI Agent 技能集** — MT5 EA 策略开发 + A股量化分析工具包

---

## 概述

收录 11 个量化交易 Skills，覆盖从 MT5 EA 开发到 A 股量化分析的全链条。基于 [WorkBuddy](https://www.codebuddy.cn) AI 助手平台，每个 Skill 加载即可赋予 AI 对应的量化专业能力。

---

## 目录结构

```
quant-agent-hub/
├── skills/
│   ├── mt5-ea-expert/            # MT5 EA 策略开发专家 v2.0（40KB）
│   ├── redquant-ashare-quant/    # RedQuant A股量化策略
│   ├── a-stock-analysis/         # A股综合技术分析
│   ├── etf-assistant/            # ETF 基金投资助手
│   ├── t-trading/                # T+0 交易策略
│   ├── ac-stock-ultrashort/      # A股超短线交易
│   ├── market-pulse/             # 市场脉搏/情绪分析
│   ├── a-stock-market-sentiment/ # A股市场情绪分析
│   ├── stock-price-checker/      # 股票价格查询
│   ├── aakshare/                 # AKShare 财经数据接口
│   └── eastmoney-tools/          # 东方财富工具集
├── .gitignore
└── README.md
```

---

## Skills 详情

| 技能 | 核心能力 |
|------|---------|
| **mt5-ea-expert** | MQL5 EA 全栈开发。市场状态自适应（Regime Switching）、多策略融合、波动率仓位管理、Kelly 公式、Walk-Forward 优化、HMM 隐马尔可夫检测、Hurst 指数、贝叶斯概率更新 |
| **redquant-ashare-quant** | A股量化策略开发。因子分析、回测框架、统计套利、多因子模型、风格轮动 |
| **a-stock-analysis** | 技术面+基本面综合诊断。K线形态、均线系统、MACD/KDJ/RSI、量价关系、支撑阻力、财报分析 |
| **etf-assistant** | ETF 全品种覆盖（宽基/行业/跨境/商品）。折溢价套利、网格交易、定投策略、行业轮动 |
| **t-trading** | T+0 回转交易策略。底仓管理、日内波段、高频差价、仓位滚动 |
| **ac-stock-ultrashort** | 超短线交易体系。集合竞价、打板策略、龙虎榜、连板分析、情绪周期 |
| **market-pulse** | 市场全景监控。大盘情绪、板块轮动、资金流向、北向资金、融资融券 |
| **a-stock-market-sentiment** | 情绪量化分析。恐慌贪婪指数、涨停跌停统计、成交量异动、舆情分析 |
| **stock-price-checker** | 实时行情查询。个股详情、K线数据、分时图、盘口数据 |
| **aakshare** | AKShare 财经数据接口封装。股票/基金/期货/宏观/新闻数据全量获取 |
| **eastmoney-tools** | 东方财富数据工具。龙虎榜、资金流向、北向资金、财报日历 |

---

## 使用方式

```bash
# 克隆仓库
git clone https://github.com/dapengzhanchi141345/quant-agent-hub.git

# 复制技能到 WorkBuddy
cp -r quant-agent-hub/skills/* ~/.workbuddy/skills/

# 在 WorkBuddy 中加载
Skill({ skill: "mt5-ea-expert" })
```

---

## 适用场景

| 场景 | 推荐技能 |
|------|---------|
| 开发 MT5 EA 策略 | `mt5-ea-expert` + `aakshare`（数据回测） |
| A 股短线交易 | `ac-stock-ultrashort` + `a-stock-analysis` + `market-pulse` |
| 量化策略研究 | `redquant-ashare-quant` + `aakshare` + `eastmoney-tools` |
| ETF 投资管理 | `etf-assistant` + `market-pulse` |
| 每日复盘分析 | `a-stock-market-sentiment` + `stock-price-checker` |

---

## 许可

MIT License
