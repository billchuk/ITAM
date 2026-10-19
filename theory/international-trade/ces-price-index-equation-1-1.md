# 《国际贸易应用模型》P5 公式（1.1）：CES 价格指数的推导

> **笔记类型**：理论模型推导  
> **来源定位**：刘文革、裴莹《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，第 5 页（P5），公式（1.1）。  
> **ISBN**：978-7-302-71633-4  
> **知识标签**：International Trade · CES · Dixit–Stiglitz · Expenditure Minimization · Price Index  
> **核心问题**：为什么 CES 效用函数对应的价格指数是价格的 $`1-\sigma`$ 次幂积分，再整体取 $`1/(1-\sigma)`$ 次幂？

## 1. 原书问题与结论

原书给出连续品种形式的 CES 效用函数：

```math
U=\left[\int_{\omega\in\Omega}q(\omega)^\rho\,\mathrm d\omega\right]^{1/\rho}, \qquad 0<\rho<1.
```

令替代弹性（elasticity of substitution）为

```math
\sigma=\frac{1}{1-\rho}>1, \qquad \rho=\frac{\sigma-1}{\sigma}.
```

要推导第 5 页的**公式（1.1）**：

$$\boxed{P=\left[\int_{\omega\in\Omega}p(\omega)^{1-\sigma}\,\mathrm d\omega\right]^{\!\frac{1}{1-\sigma}}}.$$

这里 $`P`$ 是 **CES 综合价格指数**，准确说是达到一单位 CES 效用所需的**最小支出**（unit expenditure function），不是商品价格的算术平均值。

### 符号说明

| 符号 | 解释 |
| --- | --- |
| $`\Omega`$、$`\omega`$ | 可消费的商品品种集合与单个品种索引 |
| $`q(\omega)`$ | 品种 $`\omega`$ 的消费量 |
| $`p(\omega)>0`$ | 品种 $`\omega`$ 的单位价格 |
| $`U`$、$`\bar U`$ | CES 总效用及给定目标效用 |
| $`E`$ | 所有品种上的总消费支出 |
| $`\rho`$ | 效用函数的幂参数，$`0<\rho<1`$ |
| $`\sigma`$ | 品种间替代弹性，$`\sigma>1`$ |
| $`P`$ | CES 价格指数（单位效用的最低成本） |

假设各品种价格为正、所涉积分有限且为正，且消费者可以选择最优消费组合。

## 2. 建立支出最小化问题

在效用至少达到 $`\bar U>0`$ 的条件下，使消费总支出最小：

```math
\begin{aligned} \min_{\{q(\omega)\ge 0\}}\quad &E=\int_\Omega p(\omega)q(\omega)\,\mathrm d\omega,\\ \text{s.t.}\quad &\left[\int_\Omega q(\omega)^\rho\,\mathrm d\omega\right]^{1/\rho}\ge\bar U. \end{aligned}
```

因价格均为正，最优解满足效用约束等号成立。利用 $`\rho>0`$，等价约束是

$$\int_\Omega q(\omega)^\rho\,\mathrm d\omega=\bar U^\rho.$$

拉格朗日函数为

$$\mathcal L =\int_\Omega p(\omega)q(\omega)\,\mathrm d\omega +\lambda\left[\bar U^\rho-\int_\Omega q(\omega)^\rho\,\mathrm d\omega\right].$$

## 3. 一阶条件给出价格与需求的关系

对任意品种 $`\omega`$ 的 $`q(\omega)`$ 求一阶条件（连续品种下理解为变分）：

$$\frac{\delta\mathcal L}{\delta q(\omega)} =p(\omega)-\lambda\rho\,q(\omega)^{\rho-1}=0.$$

所以

$$p(\omega)=\lambda\rho\,q(\omega)^{\rho-1},$$

$$q(\omega)=\left[\frac{p(\omega)}{\lambda\rho}\right]^{\!\frac{1}{\rho-1}}.$$

由于

$$\frac{1}{\rho-1}=-\frac{1}{1-\rho}=-\sigma,$$

得到

**式（A）**

```math
\boxed{q(\omega)=A\,p(\omega)^{-\sigma}}, \qquad A\equiv(\lambda\rho)^\sigma>0.
```

**解释**：不同商品最优消费量的相对比例由其相对价格决定，且 $`\sigma`$ 越大，消费者在品种之间替代得越容易。

## 4. 将需求关系代回 CES 效用函数

从式 (A) 出发：

```math
\begin{aligned} U &=\left[\int_\Omega\bigl(Ap(\omega)^{-\sigma}\bigr)^\rho\,\mathrm d\omega\right]^{1/\rho}\\ &=A\left[\int_\Omega p(\omega)^{-\sigma\rho}\,\mathrm d\omega\right]^{1/\rho}. \end{aligned}
```

注意关键的参数恒等式：

$$-\sigma\rho =-\sigma\cdot\frac{\sigma-1}{\sigma} =1-\sigma.$$

于是

**式（B）**

$$\boxed{U=A\left[\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega\right]^{1/\rho}}.$$

## 5. 计算最优总支出

将式 (A) 代入总支出定义：

```math
\begin{aligned} E &=\int_\Omega p(\omega)q(\omega)\,\mathrm d\omega\\ &=\int_\Omega p(\omega)\bigl[Ap(\omega)^{-\sigma}\bigr]\,\mathrm d\omega\\ &=A\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega. \end{aligned}
```

因此

**式（C）**

$$\boxed{E=A\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega}.$$

## 6. 两式相除，得到原书公式（1.1）

CES 效用函数对消费数量是**一次齐次**的。最优支出与目标效用成正比；故定义单位支出函数为 $`P=E/U`$（此处的 $`E`$ 必须是达到目标效用的**最小**支出）。

将 (C) 除以 (B)，得到

```math
\begin{aligned} P=\frac{E}{U} &=\frac{A\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega} {A\left[\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega\right]^{1/\rho}}\\[6pt] &=\left[\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega\right]^{1-1/\rho}. \end{aligned}
```

剩下的关键只是变换幂指数：

$$1-\frac{1}{\rho} =1-\frac{\sigma}{\sigma-1} =-\frac{1}{\sigma-1} =\frac{1}{1-\sigma}.$$

最终证明：

**式（1.1）**

$$\boxed{P=\left[\int_{\omega\in\Omega}p(\omega)^{1-\sigma}\,\mathrm d\omega\right]^{\!\frac{1}{1-\sigma}}}.$$

**推导逻辑一句话概括**：效用函数 $`\to`$ 支出最小化 $`\to`$ 一阶条件 $`\to`$ 最优数量与价格关系 $`\to`$ 分别代入 $`U`$、$`E`$ $`\to`$ 求 $`E/U`$。

## 7. 延伸：对应的商品需求函数

定义 $`I\equiv\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega=P^{1-\sigma}`$。由 (B)，

$$A=\frac{U}{I^{1/\rho}}.$$

而 $`I^{1/\rho}=P^{(1-\sigma)/\rho}=P^{-\sigma}`$，所以 $`A=UP^\sigma`$。

代入式 (A)，得到**给定效用水平**的 Hicksian（补偿）需求：

$$\boxed{q^h(\omega;p,U)=U\left(\frac{p(\omega)}P\right)^{-\sigma}}.$$

由 $`E=PU`$ 得到**给定名义总支出**的 Marshallian（非补偿）需求：

$$\boxed{q^m(\omega;p,E)=E\,p(\omega)^{-\sigma}P^{\sigma-1}}.$$

这是将 CES 结构进一步用于 Krugman、Melitz、Armington 等国际贸易模型的基础；但完整的双边贸易引力方程还需要贸易成本、供给和市场出清等条件。

## 8. 易错点与自查

1. **$`p(\omega)`$ 和 $`P`$ 不同**：前者是某个品种的价格，后者是 CES 综合价格指数。
2. **$`E=PU`$ 有最优化前提**：对于任意不满足支出最小化的消费组合，不能简单使用这个等式。
3. **指数不是 $`\rho`$**：替代弹性是 $`\sigma=1/(1-\rho)`$，所以会出现 $`-\sigma`$、$`1-\sigma`$。
4. **连续品种是积分**；若有 $`N`$ 个等权重离散品种，就相应改为求和：$`P=[\sum_{i=1}^{N}p_i^{1-\sigma}]^{1/(1-\sigma)}`$。
5. **不同的效用函数规范化可能改变价格指数常数**：原书式（1.1）对应这里的无权重、无品种数归一化设定。

### 一分钟数值检验

考虑两种等权重离散商品，$`p_1=p_2=10`$，$`\sigma=2`$（因此 $`\rho=1/2`$）：

$$P=(10^{-1}+10^{-1})^{-1}=5.$$

若目标效用 $`U=(\sqrt{q_1}+\sqrt{q_2})^2=1`$，支出最优时 $`q_1=q_2=1/4`$，于是

$$E=10\times\frac14+10\times\frac14=5=PU.$$

$`P`$ 低于商品的单价，是因为效用聚合器存在品种效应，并不意味着出现了打折价格。

## 9. 推荐延伸阅读

- Dixit, A. K., & Stiglitz, J. E. (1977). Monopolistic competition and optimum product diversity. *American Economic Review, 67*(3), 297–308.
- Krugman, P. (1980). Scale economies, product differentiation, and the pattern of trade. *American Economic Review, 70*(5), 950–959.
- Melitz, M. J. (2003). The impact of trade on intra-industry reallocations and aggregate industry productivity. *Econometrica, 71*(6), 1695–1725. https://doi.org/10.1111/1468-0262.00467

---

**本节教材来源**：刘文革, 裴莹. (2026). *国际贸易应用模型* (第1版). 清华大学出版社. 第 5 页，公式（1.1）。
