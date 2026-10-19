# ITAM — 《国际贸易应用模型》公式推导笔记

本仓库专门整理《国际贸易应用模型》教材中的公式推导。按原书页码和公式编号逐篇记录推导步骤、符号说明、模型假设、经济学含义以及必要的数学校验。
所有推导皆来自ChatGPT并辅以人工跟随推导检查

## 教材信息

- **书名**：《国际贸易应用模型》（新文科建设教材·国际经济与贸易系列）
- **编著者**：刘文革、裴莹
- **出版社**：清华大学出版社
- **版次**：2026 年 6 月第 1 版
- **ISBN**：978-7-302-71633-4
- **参考文献**：刘文革, 裴莹. (2026). *国际贸易应用模型* (第1版). 清华大学出版社.

## 公式推导目录

| 页码 | 公式 | 主题 |
| :--- | :--- | :--- |
| P5 | [(1.1)](theory/international-trade/ces-price-index-equation-1-1.md) | 第一章第二节第二部分 CES 价格指数 |
| P6 | [(1.2)](theory/international-trade/ces-demand-revenue-equation-1-2.md) | CES 数量需求与销售收入函数 |
| P9 | [(1.4)–(1.8)](theory/international-trade/two-stage-budgeting-equations-1-4-to-1-8-p9.md) | 第一章第三节第一部分需求函数 嵌套 CES、两阶段预算分配与支出份额弹性 |
| P10 | [(1.9)–(1.16)](theory/international-trade/ces-demand-curves-equations-1-9-to-1-16-p10.md) | 第一章第三节第一部分需求函数 dd / DD 需求曲线与替代弹性 |
| P11 | [(1.17)–(1.21)](theory/international-trade/market-equilibrium-equations-1-17-to-1-21-p11.md) | 第一章第三节第二部分市场均衡 垄断竞争市场均衡：加成定价、自由进入、均衡企业数和产出 |
| P12 | [(1.22)–(1.24)](theory/international-trade/constrained-optimum-equations-1-22-to-1-24-p12.md) | 第一章第三节第三部分最优约束：零利润约束、切线条件与最优价格 |
| P12 | [(1.25)–(1.30)](theory/international-trade/unconstrained-optimum-equations-1-25-to-1-30-p12.md) | 第一章第三节第四部分无约束最优化：社会规划者一阶条件、边际成本定价与最优企业数 |
| P14 | [(1.33)–(1.42)](theory/international-trade/variable-elasticity-equations-1-33-to-1-42-p14.md) | 第一章·可变弹性的情形：一般效用、可变需求弹性与有约束福利最优 |
| P15 | [(1.43)–(1.52)](theory/international-trade/variable-elasticity-welfare-equations-1-43-to-1-52-p15.md) | 第一章·可变弹性的情形：市场均衡、约束最优与无约束最优比较 |
| P16 | [(1.53)](theory/international-trade/variable-elasticity-variety-equation-1-53-p16.md) | 第一章·可变弹性的情形：最优企业数量比较 |
| P16 | [(1.54)–(1.55b)](theory/international-trade/asymmetric-two-groups-equations-1-54-to-1-55b-p16.md) | 第一章第三节第三部分非对称情形：两商品组效用与单组候选均衡 |
| P17 | [(1.56)–(1.59)](theory/international-trade/asymmetric-entry-and-optimum-equations-1-56-to-1-59-p17.md) | 第一章第三节第三部分非对称情形：盈利进入阻止条件与福利角点 |
| P18 | [(1.60)](theory/international-trade/asymmetric-elasticity-equation-1-60-p18.md) | 第一章第三节第三部分非对称情形：均衡价格指数对替代弹性参数的导数 |

## 整理规范

1. **遵循原书**：保留原书页码、公式编号与符号，必要时对易混淆符号增加说明。
2. **逐步推导**：写出前提假设、优化问题、拉格朗日函数、一阶条件及中间代数变换，避免跳步。
3. **严格区分**：注明原书直接给出的结论、本笔记补充的推导、额外使用的假设和疑似排印问题。
4. **检查排版**：行内公式使用 GitHub 兼容的数学定界方式，独立公式使用单行 `$$...$$`；**不要在数学块中使用 `\tag{...}`**，公式编号以独立的 Markdown 文本（如 `**式（1.44）**`）放在公式前。过长的推导优先拆成多个短公式。
5. **必要验证**：在适当情况下使用量纲、极限、数值例子及预算约束进行一致性检验。

> 目前仅收录《国际贸易应用模型》的公式推导笔记。笔记用于辅助理解，疑似教材错误均需结合上下文核查。
