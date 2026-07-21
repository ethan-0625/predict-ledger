# ⚽ MCO Sports Quantitative Trading & Alpha Research

> **🛡️ Engineering & Data Integrity Notice / 工程与数据审计声明**
> This repository documents a systematic, discretionary football trading ledger. All historical exploratory records (V1) and live quantitative strategies (V2) are cryptographically timestamped via Git version control to ensure complete pre-match transparency, zero look-ahead bias, and full auditability for backtesting.
> *(本仓库记录了一个系统的、主观裁量型的足球交易账本。所有历史探索性记录（V1）和实时策略（V2）均通过 Git 版本控制进行密码学时间戳防伪，以确保绝对的赛前透明度、零前瞻偏差及可回测的完整审计性。)*

---
## 📊 Ledger Architecture & Evolution / 账本架构与演进

This repository tracks discretionary sports trading performance through a structured, data-driven framework. To maintain historical integrity and scientific rigor, the ledger is divided into two versions:

本仓库通过结构化、数据驱动的框架来追踪主观体育交易表现。为保持历史完整性与科学严谨性，账本演进划分为两个版本：
## 📈 V1 Strategy Baseline (Discretionary & Expert Intuition Phase) / V1 策略基准（主观裁量与专家直觉期）
### 1. V1 Legacy Ledger (`V1_Legacy_Ledger.csv`)

* **Status:** Archived / Legacy 🏛️  
  *状态：* 已归档 / 历史存档 🏛️
* **Tracking Period / 追踪周期:** 2026-07-05 to 2026-07-20
* **Total Tracked Matches / 总追踪场次:** 73
* **Cumulative Yield / 累计收益率:** ~~16.32%~~ ➡️ 17.86%  
  *(Note: Yield was recalculated and corrected after normalizing the turnover tracking metric to ensure strict mathematical consistency. / 注：因对底层流水统计口径进行了标准化，收益率已重新校准，以确保严密的数学自洽。)*
* **Capital Return / 投资回报率 (ROI):** 13.22%
* **Net PnL / 净盈亏:** +14.22 Units
* **Max Drawdown / 最大回撤:** -[13.91] Units
* **Core Philosophy / 核心理念:** Proof of discretionary market edge. Demonstrates that human-in-the-loop odds-reading, when paired with strict pre-match Git timestamping, yields a positive mathematical expectation without hindsight bias. *(证明主观市场优势。表明人在环路的盘口阅读，若结合严格的赛前 Git 时间戳，能在无前瞻偏差的情况下产生正向数学期望。)*
* **Audit Verification / 审计验证:** All historical entries are securely locked via the repository's cryptographic commit history (21 commits recorded). *(所有历史条目均通过仓库的密码学提交历史安全锁定)*

### 🏛️ V1 Legacy Snapshot (Match #3 - #76)
The repository archives the complete V1 historical dataset (`V1_Legacy_Ledger.csv`), featuring 73 live-trading records with integrated performance tracking (`Turnover`, `Cum PnL`, `Yield%`, `ROI%`) and cryptographic commit URLs. While it lacks explicit market-type definitions (e.g., `+/-` for Asian Handicap, `O/U` for Over/Under, and `1/X/2` for 1X2 odds), all odds values strictly reflect the market state at the exact timestamp of each commit. If line movements occurred prior to closing, auditors should cross-reference the corresponding market lines for verification. *(Note: Bookmakers for matches #3–22 are Crown, while all remaining matches are Pinnacle).*
*(本仓库归档了完整的 V1 历史数据集 `V1_Legacy_Ledger.csv`，包含 73 场实盘记录，并集成了性能追踪指标（总流水、累计盈亏、收益率、ROI）及密码学提交链接。尽管它缺乏对亚盘、大小球和欧赔的显式市场类型定义（如 `+/-`、`O/U`、`1/X/2`），但所有赔率数值均严格以每次提交（Commit）的时间戳为准。若在闭盘前发生盘口升降，审计时请对照相应的盘口进行比对。（注：第 3-22 场的博彩公司为皇冠，其余均为平博）。)*

> 🗄️ **V1 Archive Redirect / V1 历史存档重定向**
> The complete uncompressed historical dataset is available for direct audit and backtesting analysis. 
> *(完整的历史数据集已开放，可供直接审计与回测分析。)*
> 
> 🔗 **[Click here to view the V1 Legacy Ledger (点击此处查看 V1 历史账本) ➡️](./V1_Legacy_Ledger.csv)**

## 🚀 V2 Quantitative Architecture (Active) / V2 量化架构（运行中）
With the launch of the V2 architecture, the event counter resets to Match #1. The ledger now strictly adheres to a machine-readable schema designed for automated Python backtesting (pandas compatible). 
*(随着 V2 架构的启用，比赛计数器从第 1 场重新开始。账本现已全面过渡到专为自动化 Python 回测设计的严格、机器可读标准结构。)*

### 📋 V2 Strategy Execution Ledger / V2 策略执行流水
> **🗄️ Database Redirect / 数据库重定向**
> To maintain dashboard readability and strict data separation, the continuous live ledger is maintained in a dedicated file. 
> *(为保持主页可读性与严格的数据分离，连续的实时账本维护在独立文件中。)*
> 
> 🔗 **[Click here to view the full V2 Discretionary Ledger (点击此处查看 V2 完整主观账本) ➡️](./V2_Discretionary_Ledger.csv)**

---
### 📖 V2 Data Dictionary (Key Variables) / 数据字典（核心变量声明）
To ensure clear backtesting parameters and eliminate ambiguity in data auditing, the categorical variables are defined as follows:
*(为确保明确的回测参数并消除数据审计中的歧义，核心分类变量严格定义如下：)*

* **`Conviction` (Discretionary Confidence Score / 主观确信度):**
  * `3` = **High (高)**: Core conviction trade. Deep fundamental or market alpha identified. *(核心主战仓位。已识别出深度的基本面或市场 Alpha。)*
  * `2` = **Medium (中)**: Standard system output. Aligns with baseline quantitative parameters. *(常规模型输出。符合基础量化参数设定。)*
  * `1` = **Low (低)**: Exploratory/Edge case. Placed primarily for data gathering and tracking new patterns. *(探索性/边缘测试单。主要用于数据收集和追踪新盘口模式。)*

* **`Bookmaker` (Execution Venue / 执行机构):** 
  Standardized institutional abbreviations (e.g., `PIN` = Pinnacle, `BF` = Betfair). 
  *(标准化的机构简称，例如：`PIN` = 平博，`BF` = 必发交易所。)*

## ⚠️ Disclaimer / 免责声明
**Not Financial Advice (NFA).** The data, strategies, and historical records provided in this repository are strictly for educational, research, and technical demonstration purposes. They do not constitute financial, investment, or betting advice. Sports markets are highly volatile, and past performance is not indicative of future results. The repository owner assumes absolutely no liability for any financial losses incurred by utilizing the information, signals, or code within this project. Trade and wager strictly at your own risk.
*(非财务建议。本仓库提供的所有数据、策略及历史记录仅用于教育、学术研究及技术展示目的，绝不构成任何财务、投资或博彩建议。体育市场具有高度波动性，过往业绩不代表未来表现。仓库所有者对任何人因使用本项目中的信息、信号或代码而导致的任何财务损失概不负责。任何跟单或交易行为的风险均由您自行承担。)*
