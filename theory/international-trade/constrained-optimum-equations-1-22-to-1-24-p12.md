# 《国际贸易应用模型》P12：约束社会最优（1.22）—（1.24）推导

> **书目信息**：刘文革、裴莹编著，《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，ISBN 978-7-302-71633-4。  
> **原书定位**：P12，第一章第三节“（三）最优约束”，公式（1.22）—（1.24）。  
> **上一节**：[P11 市场均衡（1.17）—（1.21）](market-equilibrium-equations-1-17-to-1-21-p11.md)。  
> **下一节**：[无约束社会最优（1.25）—（1.30）](unconstrained-optimum-equations-1-25-to-1-30-p12.md)。

## 0. 问题背景

**目标**：在对称生产、企业零利润（不允许亏损）的约束下，选择品种数 $`n`$ 与每种品种的价格 $`p`$，使社会福利最大。

在前文两阶段预算模型、名义收入 $`I=1`$ 的规范化下，若外层偏好满足相应条件，则对于给定预算，降低差异化商品综合价格指数 $`q`$ 可以提高福利。因此原书把问题写成：

$$
\min_{n>0,\ p>c}\quad q(p,n)=p n^{-\beta},
\qquad \beta=\frac{1-\rho}{\rho}>0.
$$

这里

- $`n`$：对称活跃企业（品种）数；通常在此用连续变量近似。
- $`p`$：每种差异化商品的共同价格。
- $`a>0`$：每家企业的固定成本。
- $`c>0`$：每单位产出的边际成本。
- $`s(q)\in(0,1)`$：差异化商品部门在消费者总预算中的支出份额。
- $`\theta(q)=\mathrm d\ln s(q)/\mathrm d\ln q`$：支出份额对综合价格的弹性。

### 对原书图片中目标函数的校勘

图片的目标写法看起来是 $`\min pn^{-d}`$（上标字形近似 $`d`$），但此前公式（1.12）已明确给出 $`q=pn^{-\beta}`$。本节优化的对象只能是这一 CES 综合价格指数，因此统一采用 $`pn^{-\beta}`$。如需正式判定是否印刷错误，应再与清晰原版或其它印次核对。

## 1. （1.22）从零利润条件得到社会规划者的约束

由 P10 对称需求式（1.13），以及 $`I=1`$：

$$
x=\frac{s(q)}{pn},
\qquad
q=pn^{-\beta}.
$$

每家企业利润为：

$$
\pi=(p-c)x-a.
$$

在利润恰好为零的约束边界上：

$$
(p-c)x=a.
$$

代入需求 $`x=s(q)/(pn)`$：

$$
(p-c)\frac{s(q)}{pn}=a.
$$

再代入 $`q=pn^{-\beta}`$：

$$
\boxed{
(p-c)\frac{s(pn^{-\beta})}{pn}=a.
}
\tag{1.22}
$$

这是最优约束问题的**绑定零利润约束**。也可理解为在社会规划者不能通过税收和一次性补贴弥补亏损时，每个企业至少要靠销售收入覆盖固定成本。

> 注：纯粹的“不亏损”约束本来是 $`\pi\ge0`$；原书在求解时取 $`\pi=0`$。这要求最优解落在约束边界，而不是任意 $`p,n`$ 自动满足的恒等式。以下遵照教材讨论的绑定约束情形。

## 2. （1.23）目标函数与约束曲线的切线条件

为了清楚看到“沿目标水平曲线”与“沿约束曲线”的替代率，选取 $`\ln p`$ 与 $`\ln n`$ 为横纵坐标。

### 2.1 目标价格指数保持不变的斜率

$$
\ln q=\ln p-\beta\ln n.
$$

全微分：

$$
\mathrm d\ln q=\mathrm d\ln p-\beta\,\mathrm d\ln n.
$$

在一条 $`q`$ 不变的等值曲线上，$`\mathrm d\ln q=0`$，故：

$$
\boxed{
\left.\frac{\mathrm d\ln p}{\mathrm d\ln n}\right|_{q}
=\beta.
}
\tag{A}
$$

### 2.2 零利润曲线上价格与企业数的替代斜率

令：

$$
F(p,n)\equiv\frac{(p-c)s(q)}{pn}=a.
$$

因 $`p>c`$，取对数：

$$
\ln F=\ln(p-c)+\ln s(q)-\ln p-\ln n.
$$

对 $`p`$ 的对数微分（$`n`$ 固定时 $`\partial\ln q/\partial\ln p=1`$）：

$$
\begin{aligned}
\frac{\partial\ln F}{\partial\ln p}
&=\frac{p}{p-c}
+\theta(q)-1\\
&=\boxed{\frac{c}{p-c}+\theta(q)}.
\end{aligned}
$$

对 $`n`$ 的对数微分（$`p`$ 固定时 $`\partial\ln q/\partial\ln n=-\beta`$）：

$$
\begin{aligned}
\frac{\partial\ln F}{\partial\ln n}
&=\theta(q)(-\beta)-1\\
&=\boxed{-[1+\beta\theta(q)]}.
\end{aligned}
$$

因为约束要求 $`F=a`$ 保持不变，因此：

$$
0=
\left[\frac{c}{p-c}+\theta(q)\right]\mathrm d\ln p
-[1+\beta\theta(q)]\mathrm d\ln n.
$$

在相应分母非零的内点处，约束曲线的斜率为：

$$
\boxed{
\left.\frac{\mathrm d\ln p}{\mathrm d\ln n}\right|_{F=a}
=\frac{1+\beta\theta(q)}{c/(p-c)+\theta(q)}.
}
\tag{B}
$$

### 2.3 两条曲线相切，得到（1.23）

对于内部受约束最优，两条曲线的斜率相等：

$$
\beta=\frac{1+\beta\theta(q)}{c/(p-c)+\theta(q)}.
$$

等价地：

$$
\boxed{
\frac{\dfrac{c}{p-c}+\theta(q)}
{1+\beta\theta(q)}
=\frac1\beta.
}
\tag{1.23}
$$

**为什么会有 $`\theta(q)`$？** 因为改变 $`p`$ 或 $`n`$ 都会改变 CES 价格指数 $`q`$，进而改变差异化商品部门的总支出份额 $`s(q)`$。单凭固定 $`s`$ 的假设不能复现教材的完整式（1.23）。

这里需要 $`s(q)>0`$、$`p>c`$，并在使用式（1.23）时要求 $`1+\beta\theta(q)\ne0`$。教材上一节（1.19）通常使用更强条件 $`1+\beta\theta(q)>0`$。

## 3. （1.24）化简一阶条件，求最优受约束价格

将（1.23）交叉相乘：

$$
\beta\left[\frac{c}{p-c}+\theta(q)\right]
=1+\beta\theta(q).
$$

左右两边的 $`\beta\theta(q)`$ **完全抵消**：

$$
\beta\frac{c}{p-c}=1.
$$

因此：

$$
p-c=\beta c
\quad\Longrightarrow\quad
\boxed{
p_c=c(1+\beta).
}
\tag{1.24}
$$

**关键经济学含义**：在该 CES/对称/绑定零利润模型中，虽然部门支出份额可能随着 $`q`$ 变化，但它对最优加成价格的影响在一阶条件中相互抵消。因此最优受约束价格形式与市场均衡加成定价一致。

与前一篇（1.17）对比：

$$
p_e=c(1+\beta)
=\boxed{p_c}.
$$

同样的零利润约束（1.22）与市场均衡方程（1.18）也给出相同的企业数候选解：

$$
\frac{s(p_c n_c^{-\beta})}{p_c n_c}
=\frac{a}{\beta c}.
$$

若满足前述单调性、可行性与存在性条件，并且两边选择同一解：

$$
\boxed{n_c=n_e,\quad p_c=p_e,\quad x_c=x_e.}
$$

### 一阶条件是否真的是极小值？

仅有切线方程不足以自动保证极小值。可以进一步沿着零利润约束计算：

$$
\left.\frac{\mathrm d\ln q}{\mathrm d\ln p}\right|_{F=a}
=1-\beta
\frac{c/(p-c)+\theta(q)}{1+\beta\theta(q)}
=\boxed{\frac{1-\beta c/(p-c)}{1+\beta\theta(q)}}.
\tag{C}
$$

如果 $`1+\beta\theta(q)>0`$，且在同一可行连续分支上，分子在 $`c<p<c(1+\beta)`$ 为负，在 $`p>c(1+\beta)`$ 为正，所以 $`q`$ 先降后升，$`p_c`$ 是该分支的价格指数极小点。对**全局**最优仍需检查可行域边界与其他分支。

## 4. 数值校验：受约束最优与自由进入均衡重合

取 Cobb–Douglas 外层效用，使 $`s(q)=1/2`$、$`\theta(q)=0`$；再取：

$$
\beta=1,\quad c=2,\quad a=\frac1{300},\quad I=1.
$$

根据（1.24）：

$$
p_c=2(1+1)=4.
$$

由（1.22）：

$$
(4-2)\frac{1/2}{4n_c}=\frac1{300}
\quad\Longrightarrow\quad
\boxed{n_c=75}.
$$

每家企业产出：

$$
x_c=\frac{s}{p_c n_c}
=\frac{1/2}{4\times75}
=\frac1{600}.
$$

检验每家利润：

$$
(p_c-c)x_c-a
=2\times\frac1{600}-\frac1{300}=0.
$$

价格指数：

$$
q_c=p_c n_c^{-\beta}=\frac4{75}.
$$

再核对（1.23）：

$$
\frac{c/(p_c-c)+\theta}{1+\beta\theta}
=\frac{2/(4-2)+0}{1+0}=1=\frac1\beta.
$$

完全一致。

## 5. 三个公式速查

| 编号 | 结果 | 核心来源 |
| :--- | :--- | :--- |
| （1.22） | $`(p-c)s(pn^{-\beta})/(pn)=a`$ | 对称企业需求 + 绑定零利润 |
| （1.23） | $`[c/(p-c)+\theta(q)]/[1+\beta\theta(q)]=1/\beta`$ | 目标价格指数等值线与约束曲线斜率相等 |
| （1.24） | $`p_c=c(1+\beta)`$ | （1.23）交叉相乘，抵消 $`\theta(q)`$ |

## 6. 与下一节的关系

本节保留了“企业不能亏损”的限制，故规划者选择的是有加成的共同价格 $`p_c`$。下一篇在**允许一次性转移支付补贴固定成本**时，证明没有企业零利润定价约束的福利最优满足边际成本定价 $`p_u=c`$，但最优单企业产出仍为 $`a/(c\beta)`$。

[继续阅读：P12 无约束社会最优（1.25）—（1.30）](unconstrained-optimum-equations-1-25-to-1-30-p12.md)

---

*教材来源：刘文革、裴莹（2026），《国际贸易应用模型》，清华大学出版社，第 12 页。目标函数中疑似字母 $`d/\beta`$ 的识读属于本笔记的校勘说明，并非正式勘误结论。*
