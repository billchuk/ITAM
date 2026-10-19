# 《国际贸易应用模型》P6：公式（1.2）CES 需求函数与销售收入函数推导

> **来源定位**：刘文革、裴莹《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，第 6 页（P6），公式（1.2）。  
> **ISBN**：978-7-302-71633-4  
> **关联笔记**：[公式（1.1）：CES 价格指数](ces-price-index-equation-1-1.md)  
> **核心问题**：为什么品种需求的相对价格指数为 $`-\sigma`$，而其销售收入的指数是 $`1-\sigma`$？

## 1. 原书公式与符号

书中公式（1.2）为：

$$
\boxed{q(\omega)=Q\left[\frac{p(\omega)}{P}\right]^{-\sigma}},
\qquad
\boxed{r(\omega)=R\left[\frac{p(\omega)}{P}\right]^{1-\sigma}}.
\tag{1.2}
$$

| 符号 | 含义 |
| :--- | :--- |
| $`\Omega`$、$`\omega`$ | 连续商品（品种）集合与单一品种 |
| $`q(\omega)`$ | 品种 $`\omega`$ 的最优需求量 |
| $`p(\omega)>0`$ | 品种 $`\omega`$ 的价格 |
| $`r(\omega)=p(\omega)q(\omega)`$ | 品种 $`\omega`$ 的支出／销售收入 |
| $`Q=U`$ | CES 综合消费数量指数，等于原书定义的效用水平 |
| $`P`$ | CES 综合价格指数（上文公式 1.1） |
| $`R=PQ=\int_\Omega r(\omega)\,\mathrm d\omega`$ | 总支出／总销售收入 |
| $`\sigma=1/(1-\rho)>1`$ | 品种之间的替代弹性 |

原书使用的 CES 效用函数为：

$$
U=\left[\int_\Omega q(\omega)^\rho\,\mathrm d\omega\right]^{1/\rho},
\qquad 0<\rho<1,\quad
\sigma=\frac{1}{1-\rho}.
$$

公式（1.1）已经推导出：

$$
\boxed{P=\left[\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega\right]^{1/(1-\sigma)}}.
\tag{1.1}
$$

假设价格为正、积分有限且消费者处于最优配置。这里没有给品种加权，也没有对品种数做归一化，严格遵照原书截图中的 CES 设定。

## 2. 一阶条件：为什么 $`q(\omega)\propto p(\omega)^{-\sigma}`$？

考虑给定目标效用 $`\bar U`$ 的支出最小化问题：

$$
\min_{\{q(\omega)\ge0\}}\int_\Omega p(\omega)q(\omega)\,\mathrm d\omega
\quad\text{s.t.}\quad
\int_\Omega q(\omega)^\rho\,\mathrm d\omega=\bar U^\rho.
$$

拉格朗日函数：

$$
\mathcal L=
\int_\Omega p(\omega)q(\omega)\,\mathrm d\omega
+\lambda\left[\bar U^\rho-
\int_\Omega q(\omega)^\rho\,\mathrm d\omega\right].
$$

对每个品种的消费量求一阶条件：

$$
p(\omega)=\lambda\rho\,q(\omega)^{\rho-1},
$$

从而

$$
q(\omega)=
\left[\frac{p(\omega)}{\lambda\rho}\right]^{1/(\rho-1)}.
$$

由 $`\rho=(\sigma-1)/\sigma`$ 可知

$$
\frac{1}{\rho-1}=-\sigma.
$$

令 $`A=(\lambda\rho)^\sigma>0`$，则有

$$
\boxed{q(\omega)=A\,p(\omega)^{-\sigma}}.
\tag{A}
$$

$`A`$ 对所有品种相同；下一步用 CES 总量和价格指数确定它。

## 3. 推导公式（1.2）的第一行：数量需求

将式 (A) 代入 CES 效用函数：

$$
\begin{aligned}
U
&=\left[\int_\Omega\bigl(Ap(\omega)^{-\sigma}\bigr)^\rho\,\mathrm d\omega\right]^{1/\rho}\\
&=A\left[\int_\Omega p(\omega)^{-\sigma\rho}\,\mathrm d\omega\right]^{1/\rho}.
\end{aligned}
$$

关键的参数关系：

$$
-\sigma\rho
=-\sigma\frac{\sigma-1}{\sigma}
=1-\sigma.
$$

利用价格指数定义

$$
\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega=P^{1-\sigma},
$$

因此

$$
\begin{aligned}
U
&=A\left[P^{1-\sigma}\right]^{1/\rho}\\
&=AP^{(1-\sigma)/\rho}
=AP^{-\sigma}.
\end{aligned}
$$

最后一步用到了

$$
\frac{1-\sigma}{\rho}
=\frac{1-\sigma}{(\sigma-1)/\sigma}=-\sigma.
$$

移项可得 $`A=UP^\sigma`$，代回式 (A)：

$$
\begin{aligned}
q(\omega)
&=UP^\sigma p(\omega)^{-\sigma}\\
&=U\left[\frac{p(\omega)}{P}\right]^{-\sigma}.
\end{aligned}
$$

原书规定 $`Q=U`$，所以

$$
\boxed{\displaystyle
q(\omega)=Q\left[\frac{p(\omega)}{P}\right]^{-\sigma}}.
\tag{1.2a}
$$

> **经济含义**：单个品种价格相对 CES 综合价格 $`P`$ 越高，最优消费数量越低。$`\sigma`$ 越大，消费者对相对价格变化越敏感。

## 4. 推导公式（1.2）的第二行：支出和销售收入

按定义，品种收入等于价格乘销量：

$$
r(\omega)=p(\omega)q(\omega).
$$

代入 (1.2a)：

$$
r(\omega)=p(\omega)Q\left[\frac{p(\omega)}{P}\right]^{-\sigma}.
$$

把单个价格改写成 $`p(\omega)=P[p(\omega)/P]`$：

$$
\begin{aligned}
r(\omega)
&=PQ\left[\frac{p(\omega)}{P}\right]\left[\frac{p(\omega)}{P}\right]^{-\sigma}\\
&=PQ\left[\frac{p(\omega)}{P}\right]^{1-\sigma}.
\end{aligned}
$$

由原书定义 $`R=PQ`$，得到

$$
\boxed{\displaystyle
r(\omega)=R\left[\frac{p(\omega)}{P}\right]^{1-\sigma}}.
\tag{1.2b}
$$

所以 $`-\sigma`$ 变成 $`1-\sigma`$ 的唯一代数原因，就是收入函数比数量需求函数**多乘了一个价格**：

$$
p(\omega)\times p(\omega)^{-\sigma}
=p(\omega)^{1-\sigma}.
$$

## 5. 为什么总支出恰好是 $`R=PQ`$？

这一点可以直接验证：

$$
\begin{aligned}
\int_\Omega r(\omega)\,\mathrm d\omega
&=\int_\Omega R\left[\frac{p(\omega)}{P}\right]^{1-\sigma}\,\mathrm d\omega\\
&=R\,P^{\sigma-1}\int_\Omega p(\omega)^{1-\sigma}\,\mathrm d\omega\\
&=R\,P^{\sigma-1}P^{1-\sigma}\\
&=R.
\end{aligned}
$$

这里利用了公式（1.1），因此所有品种的销售收入确实加总为总支出 $`R`$。更根本地说，CES 聚合器对数量**一次齐次**，最优支出函数满足 $`R=PU=PQ`$。

## 6. 与 Marshallian 和 Hicksian 需求的区别

当给定目标效用（综合数量）$`Q`$ 时：

$$
\boxed{q^h(\omega;p,Q)
=Q\left[\frac{p(\omega)}P\right]^{-\sigma}}.
$$

这是支出最小化对应的 **Hicksian（补偿）需求**。

当给定总预算／名义支出 $`R`$ 时，由 $`Q=R/P`$：

$$
\begin{aligned}
q^m(\omega;p,R)
&=\frac{R}{P}\left[\frac{p(\omega)}P\right]^{-\sigma}\\
&=R\,P^{\sigma-1}p(\omega)^{-\sigma}.
\end{aligned}
$$

这是效用最大化对应的 **Marshallian（非补偿）需求**。两种写法在给定同一最优分配且 $`R=PQ`$ 时相容，但应明确哪一个总量被固定。

## 7. 数值校验

考虑两个对称的**离散**品种（对应把积分改为求和），令 $`p_1=p_2=10`$、$`\sigma=2`$、$`Q=1`$。

根据 (1.1)：

$$
P=(10^{-1}+10^{-1})^{-1}=5,\qquad R=PQ=5.
$$

根据 (1.2a)：

$$
q_1=q_2=1\times(10/5)^{-2}=\frac14.
$$

根据 (1.2b)：

$$
r_1=r_2=5\times(10/5)^{-1}=2.5.
$$

因此：

$$
r_1+r_2=2.5+2.5=5=R.
$$

两条需求表达式与预算约束一致。

## 8. 易错点与模型应用

1. **$`P`$ 不是品种价格**：$`p(\omega)/P`$ 是相对综合价格。
2. **$`Q`$ 不是把消费数量简单相加**：$`Q=U`$ 是 CES 聚合数量指数；在原书的特定规范化下成立。
3. **$`R`$ 为支出总额**：无论从消费者看还是企业看，这里的 $`r(\omega)`$ 是品种支出／销售收入，而不是利润。
4. **价格变动的比较静态需说明控制变量**：在 $`R,P`$ 给定时，$`r(\omega)\propto p(\omega)^{1-\sigma}`$；如果价格变动同时改变 $`P`$ 或 $`R`$，须把这些内生变化计入。
5. **结构引力模型尚需额外结构**：这里仅推导 CES 品种需求和收入；要得到双边贸易方程，还需贸易成本、产地、市场出清等假设。

## 9. 相关文献

- Dixit, A. K., & Stiglitz, J. E. (1977). Monopolistic competition and optimum product diversity. *American Economic Review, 67*(3), 297–308.
- Krugman, P. (1980). Scale economies, product differentiation, and the pattern of trade. *American Economic Review, 70*(5), 950–959.
- Melitz, M. J. (2003). The impact of trade on intra-industry reallocations and aggregate industry productivity. *Econometrica, 71*(6), 1695–1725. https://doi.org/10.1111/1468-0262.00467

---

**关联阅读：** [上一篇：公式（1.1）CES 价格指数推导](ces-price-index-equation-1-1.md)。

**本节教材来源**：刘文革, 裴莹. (2026). *国际贸易应用模型* (第1版). 清华大学出版社. 第 6 页，公式（1.2）。
