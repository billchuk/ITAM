# 《国际贸易应用模型》P12：无约束社会最优（1.25）—（1.30）逐式推导

> **书目信息**：刘文革、裴莹编著，《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，ISBN 978-7-302-71633-4。  
> **页码**：按本次阅读标注为 P12；图片未完整显示印刷页眉页码，后续如需可据清晰页眉校订。  
> **位置**：第一章第三节“（四）无约束最优化方法”，公式（1.25）—（1.30）。  
> **关联笔记**：[P12 约束最优（1.22）—（1.24）](constrained-optimum-equations-1-22-to-1-24-p12.md)；[P11 市场均衡（1.17）—（1.21）](market-equilibrium-equations-1-17-to-1-21-p11.md)。

## 0. 何谓“无约束最优”？

与前一篇必须让企业靠售价自行覆盖固定成本的约束最优不同，这里**允许政府通过一次性（lump-sum）转移支付筹集或补偿固定成本**，因此规划者可以直接选择企业数量 $`n`$ 与每家企业产量 $`x`$，最大化整体效用。

“无约束”并不意味着没有任何资源限制，而是**不再额外要求企业必须靠垄断加成定价实现零利润**。全社会资源约束已经写入下面的效用表达式。

维持 P9–P11 的记号：

```math
y=\left(\sum_{i=1}^{n}x_i^\rho\right)^{1/\rho}, \quad \rho\in(0,1),\quad \beta=\frac{1-\rho}{\rho}>0.
```

对称状态下，所有品种数量相同 $`x_i=x`$，故根据（1.12）：

**式（A）**

$$\boxed{y=xn^{1/\rho}=x n^{1+\beta}}.$$

每家企业的总成本是 $`a+cx`$，其中 $`a>0`$ 是固定成本，$`c>0`$ 是边际成本。社会有 1 单位可用于消费和生产的资源，故：

**式（B）**

$$\boxed{x_0+n(a+cx)=1}, \qquad x_0=1-n(a+cx)\ge0.$$

设外层效用函数为 $`U(x_0,y)`$，两个边际效用记为：

```math
U_0\equiv\frac{\partial U}{\partial x_0}>0, \qquad U_y\equiv\frac{\partial U}{\partial y}>0.
```

以下默认连续 $`n>0`$、$`x>0`$ 的内点解、可微偏好和可行资源约束。现实企业数需取整数时，上述连续解是一种近似。

## 1. （1.25）直接代入资源约束的规划者问题

规划者选择 $`(n,x)`$ 最大化福利：

```math
\max_{n>0,\ x>0}\; u=U(x_0,y)
```

受制于资源约束 (B) 和 CES 对称聚合器 (A)。

代入：

**式（1.25）**

$$\boxed{ \max_{n,x}\; u(n,x)=U\!\left(1-n(a+cx),\,x n^{1+\beta}\right). }$$

特别注意：“所有企业产量相同”是这里采用的对称最优安排；最优化的**目标是效用 $`u`$，不是简单地把物理产量 $`n x`$ 最大化**。

## 2. （1.26）对单个企业产量 $`x`$ 的一阶条件

记：

$$x_0(n,x)=1-n(a+cx),\qquad y(n,x)=x n^{1+\beta}.$$

固定 $`n`$，有：

$$\frac{\partial x_0}{\partial x}=-nc, \qquad \frac{\partial y}{\partial x}=n^{1+\beta}.$$

利用复合函数链式法则：

```math
\begin{aligned} \frac{\partial u}{\partial x} &=U_0\frac{\partial x_0}{\partial x} +U_y\frac{\partial y}{\partial x}\\ &=-nc\,U_0+n^{1+\beta}U_y. \end{aligned}
```

内点最优要求 $`\partial u/\partial x=0`$：

**式（1.26）**

$$\boxed{-nc\,U_0+n^{1+\beta}U_y=0.}$$

将其移项：

$$n^{1+\beta}U_y=ncU_0.$$

在 $`n>0`$ 和 $`U_0>0`$ 的条件下除以 $`n^{1+\beta}U_0`$：

**式（C）**

$$\boxed{\frac{U_y}{U_0}=c n^{-\beta}.}$$

经济含义：再多生产一单位每品种产量，会消耗 $`nc`$ 单位同质商品资源，同时提高综合数量 $`n^{1+\beta}`$ 单位；最优时两种变化的边际效用价值相等。

## 3. （1.27）对企业数 $`n`$ 的一阶条件

固定每家企业产量 $`x`$，有：

$$\frac{\partial x_0}{\partial n}=-(a+cx),$$

$$\frac{\partial y}{\partial n} =\frac{\partial}{\partial n}\bigl[x n^{1+\beta}\bigr] =(1+\beta)x n^\beta.$$

应用链式法则：

```math
\begin{aligned} \frac{\partial u}{\partial n} &=U_0[-(a+cx)] +U_y[(1+\beta)x n^\beta]. \end{aligned}
```

内点最优条件：

**式（1.27）**

$$\boxed{ -(a+cx)U_0+(1+\beta)x n^\beta U_y=0. }$$

它是在“**增加一个品种**”时，固定和可变生产资源的额外消耗与多样性带来的额外效用相等的条件。

## 4. （1.28）从一阶条件得到边际成本定价 $`p_u=c`$

从上层消费选择（P9 两阶段预算最优化），消费者在 $`x_0`$ 与差异化品种综合数量 $`y`$ 之间的最优条件为：

**式（D）**

$$\boxed{q=\frac{U_y}{U_0},}$$

这里同质商品价格被标准化为 1，$`q`$ 是 CES 综合价格指数。

而规划者关于产量的条件（C）显示：

$$\frac{U_y}{U_0}=c n^{-\beta}.$$

因此实施规划者最优配置所需的综合相对价格满足：

$$q_u=c n^{-\beta}.$$

对称 CES 价格指数为：

$$q=p n^{-\beta}.$$

所以若以共同单品种售价 $`p_u`$ 实施最优安排：

**式（1.28）**

$$p_u n^{-\beta}=c n^{-\beta} \quad\Longrightarrow\quad \boxed{p_u=c.}$$

**理解重点**：规划者原始选择变量是 $`n,x`$，而非 $`p`$。（1.28）的 $`p_u`$ 是由最优边际替代率映射得到的**实施价格／影子价格**，并非对规划者原始目标直接对 $`p`$ 求导得出。

为何不同于 P11 市场均衡 $`p_e=c(1+\beta)`$？在无约束最优中，固定成本无需靠单件商品加价收回，可通过一次性转移支付覆盖，所以单件价格回到边际成本。

## 5. （1.29）联立两条 FOC 求最优单企业产量

由（1.27）：

$$(a+cx)U_0=(1+\beta)x n^\beta U_y.$$

将（1.26）给出的 $`U_y/U_0=c n^{-\beta}`$ 代入：

```math
\begin{aligned} a+cx &=(1+\beta)x n^\beta \frac{U_y}{U_0}\\ &=(1+\beta)x n^\beta(c n^{-\beta})\\ &=(1+\beta)cx. \end{aligned}
```

整理：

$$a+cx=cx+\beta cx \quad\Longrightarrow\quad a=\beta cx.$$

所以：

**式（1.29）**

$$\boxed{x_u=\frac{a}{c\beta}.}$$

与 P11 的自由进入均衡产出（1.20）比较：

$$\boxed{x_u=x_e=\frac{a}{c\beta}.}$$

两种制度下**每家企业最优产量可以相同，但品种数、售价、综合价格指数及社会福利未必相同**。

## 6. （1.30）转移支付下的消费者预算及最优企业数

按（1.28），无约束最优应采用 $`p_u=c`$。企业自行销售收入：

$$p_u x_u=c x_u.$$

企业需要负担的总成本是 $`a+c x_u`$，所以**每家企业仍缺少固定成本 $`a`$**：

$$\pi_u=(p_u-c)x_u-a=-a.$$

如果由消费者通过一次性税收筹集资金、再向每家企业补贴 $`a`$，共需 $`a n`$ 单位资源或收入。由此，消费者可用于市场购货的净名义收入为：

**式（E）**

$$\boxed{I_{\mathrm{net}}=1-an.}$$

必须满足 $`0<an<1`$，以保证净收入为正；**这些支付是再分配而非新生产资源**，但它们覆盖了企业需要预先支付的固定成本。

沿用对称市场需求（1.13）：

$$x=\frac{I_{\mathrm{net}}s(q)}{pn}.$$

代入 $`I_{\mathrm{net}}=1-an`$、$`q=pn^{-\beta}`$：

**式（F）**

$$\boxed{ x=(1-an)\frac{s(pn^{-\beta})}{pn}. }$$

最后在福利最优安排下，代入 $`p_u=c`$ 和 $`x_u=a/(c\beta)`$：

$$\frac{a}{c\beta} =(1-a n_u)\frac{s(cn_u^{-\beta})}{c n_u}.$$

左右同乘 $`c`$：

$$\frac{a}{\beta} =(1-a n_u)\frac{s(cn_u^{-\beta})}{n_u}.$$

再移项：

**式（1.30）**

$$\boxed{ \frac{s(cn_u^{-\beta})}{n_u} =\frac{a/\beta}{1-a n_u}. }$$

这是用来确定**无约束最优的活跃企业数 $`n_u`$** 的隐式方程，其解还须落在 $`0<n_u<1/a`$ 的可行域内。

当 $`s(q)`$ 不是一个具体的函数形式时，通常无法直接把 $`n_u`$ 写成简单显式公式；可以进一步给定外层效用形式后求解，或采用数值计算。

### 关于唯一性的补充

将（1.30）写为：

$$h(n)\equiv (1-an)\frac{s(cn^{-\beta})}{n}=\frac{a}{\beta}.$$

对 $`0<n<1/a`$：

$$\frac{\mathrm d\ln h(n)}{\mathrm d\ln n} =-\frac{an}{1-an}-1-\beta\theta(cn^{-\beta}).$$

如果此前（1.19）的条件 $`1+\beta\theta(q)>0`$ 在所有相关 $`q`$ 上成立，那么 $`h(n)`$ 在可行域内严格下降，因此方程**至多有一个解**；存在性仍须另行核查。

## 7. 与受约束最优、市场均衡对比

| 项目 | 自由进入市场 / 受约束最优 | 无约束社会最优 |
| :--- | :--- | :--- |
| 企业共同价格 | $`p_e=p_c=c(1+\beta)`$ | $`p_u=c`$ |
| 每家企业销量 | $`x_e=x_c=a/(c\beta)`$ | $`x_u=a/(c\beta)`$ |
| 固定成本的支付方式 | 依靠高于边际成本的售价自行收回 | 边际成本定价 + 一次性转移支付补偿 |
| 品种数 | $`s(p_e n_e^{-\beta})/(p_e n_e)=a/(\beta c)`$ | $`s(c n_u^{-\beta})/n_u=(a/\beta)/(1-a n_u)`$ |
| 消费者购货预算 | $`I=1`$ | $`I_{\mathrm{net}}=1-an_u`$ |

在允许恰当、无扭曲的转移支付且规划者解决的是同一个福利最大化问题时，无约束最优的福利弱优于受约束方案；但**不能不经求解就断言对任意偏好都必然有某个固定的品种数差距**。

## 8. 一个完整可手算的数值例子

取外层 Cobb–Douglas 效用使差异化部门的支出份额恒为：

$$s(q)=\alpha=\frac12,\qquad \theta(q)=0,$$

以及：

$$\beta=1,\quad c=2,\quad a=\frac1{300}.$$

**市场均衡／约束最优**（见上一篇）：

$$p_e=p_c=4,\qquad x_e=x_c=\frac{a}{c\beta}=\frac1{600}, \qquad n_e=n_c=75.$$

于是综合价格指数 $`q_c=4/75`$。

**无约束最优**：

$$p_u=c=2,\qquad x_u=\frac1{600}.$$

对（1.30）代入 $`s=\alpha=1/2`$：

$$\frac{\alpha}{n_u} =\frac{a/\beta}{1-a n_u}.$$

解出：

$$\alpha\beta(1-a n_u)=a n_u \quad\Longrightarrow\quad \boxed{n_u=\frac{\alpha\beta}{a(1+\alpha\beta)}}.$$

再代入数值：

$$n_u =\frac{1/2}{(1/300)(1+1/2)}=100.$$

净收入为：

$$I_{\mathrm{net}}=1-a n_u =1-\frac{100}{300}=\frac23.$$

综合价格指数：

$$q_u=p_u n_u^{-\beta} =\frac{2}{100}=0.02.$$

验证对称需求：

```math
\begin{aligned} x &=\frac{I_{\mathrm{net}}\alpha}{p_u n_u}\\ &=\frac{(2/3)(1/2)}{2\times100} =\frac1{600}=x_u. \end{aligned}
```

验证资源约束：

$$x_0 =1-n_u(a+c x_u) =1-100\left(\frac1{300}+\frac2{600}\right) =\frac13.$$

验证总购货预算：

$$x_0+n_u p_u x_u =\frac13+100\times2\times\frac1{600} =\frac23 =I_{\mathrm{net}}.$$

因此：在**这个例子**中，最优无约束方案的品种数 $`100`$ 大于受约束的 $`75`$，边际成本价格低于市场价格，但每种商品的产出相同。这个数值结果是示例，不应直接概括成所有偏好下的定量规律。

## 9. 六个公式及其逻辑关系

| 公式 | 结果 | 推导来源 |
| :--- | :--- | :--- |
| （1.25） | $`\max_{n,x}U[1-n(a+cx),xn^{1+\beta}]`$ | 资源约束 + 对称 CES 聚合数量 |
| （1.26） | $`-ncU_0+n^{1+\beta}U_y=0`$ | 对企业产量 $`x`$ 求一阶条件 |
| （1.27） | $`-(a+cx)U_0+(1+\beta)xn^\beta U_y=0`$ | 对企业数量 $`n`$ 求一阶条件 |
| （1.28） | $`p_u=c`$ | 利用 $`q=U_y/U_0=pn^{-\beta}=cn^{-\beta}`$ |
| （1.29） | $`x_u=a/(c\beta)`$ | 联立两条一阶条件 |
| （1.30） | $`s(cn_u^{-\beta})/n_u=(a/\beta)/(1-an_u)`$ | 一次性转移支付 + 对称需求 + 最优价格与规模 |

**推导主线**：

$$\boxed{ \begin{gathered} u=U[1-n(a+cx),xn^{1+\beta}]\\ \Downarrow\\ \partial u/\partial x=0,\quad\partial u/\partial n=0\\ \Downarrow\\ p_u=c,\quad x_u=a/(c\beta)\\ \Downarrow\\ I_{\mathrm{net}}=1-an_u\\ \Downarrow\\ s(cn_u^{-\beta})/n_u=(a/\beta)/(1-an_u). \end{gathered} }$$

---

**教材引用**：刘文革, 裴莹. (2026). *国际贸易应用模型* (第1版). 清华大学出版社. 公式（1.25）—（1.30）；本篇 P12 页码沿用读者标注。

*本文件为学习辅助推导；关于连续品种数、内部解、一次性转移支付、唯一性和数值例子的说明为本笔记补充内容。*
