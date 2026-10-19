# 《国际贸易应用模型》P16：公式（1.53）——可变弹性下的最优企业数比较

> **教材**：刘文革、裴莹编著，《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，ISBN 978-7-302-71633-4。  
> **原书定位**：P16，第一章“模型设定与推导”中**二、可变弹性的情形**的结尾，公式（1.53）。  
> **上一篇**：[P15：公式（1.43）—（1.52）约束和无约束福利比较](variable-elasticity-welfare-equations-1-43-to-1-52-p15.md)。  
> **范围**：本篇仅推导（1.53）；P16 下半页出现的“三、非对称情形”属于后续小节，本次不纳入。

## 1. 前一页提供的两类最优企业数

（1）有约束社会最优：企业必须靠销售收入自行覆盖总成本 $`a+cx_c`$。由 P14 的（1.40）及其受约束版本：

```math
\boxed{
n_c=\frac{\omega(x_c)}{a+cx_c}.
}
\tag{A}
```

（2）无约束社会最优：社会规划者可以通过一次性转移支付覆盖企业固定成本。由 P15 的（1.51）：

```math
\boxed{
n_u=\frac{\gamma}{a+cx_u}.
}
\tag{B}
```

其中 $`a>0`$ 为每企业固定成本，$`c>0`$ 为边际成本，$`x_c`$ 和 $`x_u`$ 分别为两种最优制度下的单企业产量。

## 2. 关键不等式：为什么 $`\omega(x)<\gamma`$？

P14 的定义（1.37）：

```math
\boxed{
\omega(x)=
\frac{\gamma\rho(x)}{\gamma\rho(x)+1-\gamma},
\quad
\rho(x)=\frac{xv'(x)}{v(x)}.
}
```

沿用 $`0<\gamma<1`$ 和 $`0<\rho(x)<1`$。

直接计算二者之差：

```math
\begin{aligned}
\gamma-\omega(x)
&=\gamma-\frac{\gamma\rho(x)}
{\gamma\rho(x)+1-\gamma}\\
&=\gamma\frac{\gamma\rho(x)+1-\gamma-\rho(x)}
{\gamma\rho(x)+1-\gamma}\\
&=\boxed{
\frac{\gamma(1-\gamma)[1-\rho(x)]}
{\gamma\rho(x)+1-\gamma}>0.
}
\end{aligned}
```

所以**无论 $`\rho'(x)`$ 的符号如何**，只要 $`0<\rho(x)<1`$：

```math
\boxed{0<\omega(x)<\gamma.}
\tag{C}
```

注意：这是$`\omega`$ 与 $`\gamma`$ 的**水平比较**，不需要另外讨论 $`\rho'`$ 的正负；而 P15 比较 $`x_u`$ 与 $`x_c`$ 则需要 $`\rho'`$ 和相关最优解的单交叉条件。

## 3. 原书公式（1.53）的直接推导

将不等式（C）代入有约束企业数（A），分母为正：

```math
\begin{aligned}
n_c
=\frac{\omega(x_c)}{a+cx_c}
&<\frac{\gamma}{a+cx_c}.
\end{aligned}
```

这就是书中公式：

```math
\boxed{
n_c=\frac{\omega(x_c)}{a+cx_c}
<\frac{\gamma}{a+cx_c}.
}
\tag{1.53}
```

**含义**：在相同的单企业成本规模 $`a+cx_c`$ 下，有约束最优分配给差异化商品部门的资源份额 $`\omega(x_c)`$ 小于无约束最优的部门资源份额 $`\gamma`$，故可支持的企业数低于 $`\gamma/(a+cx_c)`$。

**重要：公式（1.53）右侧不是 $`n_u`$**。真正的 $`n_u`$ 的分母是 $`a+cx_u`$，而非 $`a+cx_c`$。不能因此直接声称在所有情况下都有 $`n_c<n_u`$。

## 4. 如何结合 P15 的（1.52）判断 $`n_c`$ 与 $`n_u`$？

如果根据 P15 的比较静态与正则性条件，有：

```math
x_u<x_c,
```

由于 $`a,c>0`$：

```math
a+cx_u<a+cx_c
\quad\Longrightarrow\quad
\frac{\gamma}{a+cx_u}>
\frac{\gamma}{a+cx_c}.
```

与（1.53）连接：

```math
\boxed{
n_u=\frac{\gamma}{a+cx_u}
>
\frac{\gamma}{a+cx_c}
>n_c.
}
\tag{D}
```

因此：

```math
\boxed{
x_u<x_c\ \Longrightarrow\ n_u>n_c.
}
```

在 P15 的充分条件下，若 $`\rho'(x)>0`$ 导致 $`x_u<x_c`$，就得到**无约束最优需要更多品种、更小的单企业生产规模**。

反过来，如果 $`x_u>x_c`$，那么：

```math
\frac{\gamma}{a+cx_u}
<
\frac{\gamma}{a+cx_c}.
```

但是 $`n_c`$ 本来就小于右端，因此**两者都小于同一个上界，不能直接排序**：

```math
n_c<\frac{\gamma}{a+cx_c},
\qquad
n_u<\frac{\gamma}{a+cx_c}.
```

是否仍有 $`n_u>n_c`$，取决于“无约束资源份额更高”能否抵消“无约束每企业成本更高”的效应。

一个直接可检验的**充要条件**是：

```math
\begin{aligned}
n_u>n_c
&\iff\frac{\gamma}{a+cx_u}>
\frac{\omega(x_c)}{a+cx_c}\\
&\iff
\boxed{
\frac{a+cx_u}{a+cx_c}<
\frac{\gamma}{\omega(x_c)}.
}
\end{aligned}
\tag{E}
```

其中：

```math
\frac{\gamma}{\omega(x_c)}
=\frac{\gamma\rho(x_c)+1-\gamma}{\rho(x_c)}>1.
```

式（E）将两种力量清楚拆分为**企业规模/成本差异**与**部门资源份额差异**。它比孤立看（1.53）更有解释力。

## 5. 常弹性特例自检

令 $`v(x)=x^r`$，$`0<r<1`$。那么 $`\rho(x)=r`$ 为常数、$`\rho'(x)=0`$。前文已经得到：

```math
x_e=x_c=x_u=\frac{ar}{c(1-r)}.
```

于是两种制度的每企业成本一样，记为 $`D=a+cx`$，但是：

```math
\omega=\frac{\gamma r}{\gamma r+1-\gamma}<\gamma.
```

所以：

```math
\boxed{
n_c=\frac{\omega}{D}
<
\frac{\gamma}{D}=n_u.
}
```

例如 $`\gamma=1/2`$、$`r=1/2`$、$`a=0.01`$、$`c=1`$：

```math
x_c=x_u=0.01,\qquad
\omega=\frac13,\qquad D=0.02.
```

因而：

```math
n_c=\frac{1/3}{0.02}\approx16.67,
\qquad
n_u=\frac{1/2}{0.02}=25.
```

企业数作为连续变量是模型的近似；若必须为整数，进入条件和福利解还要做相应离散调整。

## 6. 本页结论与阅读边界

| 关系 | 结论 | 条件 |
| :--- | :--- | :--- |
| $`\omega(x_c)`$ 与 $`\gamma`$ | $`\omega(x_c)<\gamma`$ | $`0<\rho(x_c)<1,\ 0<\gamma<1`$ |
| （1.53） | $`n_c<\gamma/(a+cx_c)`$ | 同上及 $`a+cx_c>0`$ |
| $`n_c`$ 与 $`n_u`$ | 当 $`x_u<x_c`$，必有 $`n_c<n_u`$ | （1.53）与分母单调 |
| 当 $`x_u>x_c`$ | $`n_c`$ 与 $`n_u`$ 不能仅由（1.53）比较 | 需要进一步使用式（E） |

---

**教材引用**：刘文革、裴莹（2026），《国际贸易应用模型》，清华大学出版社，第 16 页，式（1.53）。

*页面后续的“三、非对称情形”将按之后提供的对应公式单独建档。*
