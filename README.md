# ⚽ MCO Sports Quantitative Trading & Alpha Research

> **🛡️ Engineering & Data Integrity Notice / 工程与数据审计声明**
> This repository documents a systematic, discretionary football trading ledger. All historical exploratory records (V1) and live quantitative strategies (V2) are cryptographically timestamped via Git version control to ensure complete pre-match transparency, zero look-ahead bias, and full auditability for backtesting.
> *(本仓库记录了一个系统的、主观裁量型的足球交易账本。所有历史探索性记录（V1）和实时策略（V2）均通过 Git 版本控制进行密码学时间戳防伪，以确保绝对的赛前透明度、零前瞻偏差及可回测的完整审计性。)*

---

## 📈 V1 Strategy Baseline (Discretionary & Expert Intuition Phase) / V1 策略基准（主观裁量与专家直觉期）
* **Tracking Period / 追踪周期:** 2026-07-05 to 2026-07-20
* **Status / 状态:** Manual exploratory tracking phase driven entirely by human domain expertise, market pattern recognition, and odds-reading intuition (Matches 1–73). Archived for historical audit. *(完全由人类领域专业知识、市场模式识别与盘口直觉驱动的手工探索追踪阶段，已归档供历史审计)*
* **Total Tracked Matches / 总追踪场次:** 73
* **Cumulative Yield / 累计收益率 (Yield):** 16.32%
* **Capital Return / 投资回报率 (ROI):** 13.22%
* **Net PnL / 净盈亏:** +14.22 Units
* **Core Philosophy / 核心理念:** Proof of discretionary market edge. Demonstrates that human-in-the-loop odds-reading, when paired with strict pre-match Git timestamping, yields a positive mathematical expectation without hindsight bias. *(证明主观市场优势。表明人在环路的盘口阅读，若结合严格的赛前 Git 时间戳，能在无前瞻偏差的情况下产生正向数学期望。)*
* **Audit Verification / 审计验证:** All historical entries are securely locked via the repository's cryptographic commit history (21 commits recorded). *(所有历史条目均通过仓库的密码学提交历史安全锁定)*

---

## 🚀 V2 Quantitative Architecture (Active) / V2 量化架构（运行中）
Starting from Match #74, the ledger transitions to a strict, machine-readable schema designed for automated Python backtesting (`pandas` compatible). 
*(从第 74 场开始，账本过渡到专为自动化 Python 回测设计的严格、机器可读的标准结构。)*

### 📋 V2 Strategy Execution Ledger / V2 策略执行流水
> **🗄️ Database Redirect / 数据库重定向**
> To maintain dashboard readability and strict data separation, the continuous live ledger is maintained in a dedicated file. 
> *(为保持主页可读性与严格的数据分离，连续的实时账本维护在独立文件中。)*
> 
> 🔗 **[Click here to view the full V2 Live Ledger (点击此处查看 V2 完整实时账本) ➡️](./V2_Ledger.csv)**

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
