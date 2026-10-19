# 《国际贸易应用模型》P14：可变弹性模型（1.33）—（1.42）逐式推导

> **教材**：刘文革、裴莹编著，《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，ISBN 978-7-302-71633-4。  
> **原书位置**：第一章“模型设定与推导”，**二、可变弹性的情形**，P14。  
> **前文**：[P12 约束最优（1.22）—（1.24）](constrained-optimum-equations-1-22-to-1-24-p12.md)；[P12 无约束最优（1.25）—（1.30）](unconstrained-optimum-equations-1-25-to-1-30-p12.md)。  
> **下文**：[P15（1.43）—（1.52）福利排序](variable-elasticity-welfare-equations-1-43-to-1-52-p15.md)。

## 0. 符号与假设

有同质商品消费 $`x_0`$ 与 $`n`$ 个差异化品种的消费 $`x_i`$，每个企业生产一个品种。成本函数为 $`a+cx`$，其中固定成本 $`a>0`$、边际成本 $`c>0`$；同质商品单价规范化为 1，总收入为 $`I`$，均衡与福利计算部分采用 $`I=1`$。

令 $`v(x)>0`$、$`v'(x)>0`$、$`v''(x)<0`$，$`\gamma\in(0,1)`$。在需要讨论导数时假定 $`v`$ 足够光滑，内点最优存在。

| 记号 | 经济含义 |
| :--- | :--- |
| $`v(x)`$ | 单个品种消费量对差异化部门效用的贡献 |
| $`\gamma`$ | 同质商品与差异化部门之间 Cobb–Douglas 聚合的参数 |
| $`\rho(x)=xv'(x)/v(x)`$ | 单品种效用的**规模弹性**（不是前一节 CES 固定的 $`\rho`$ 参数） |
| $`\beta(x)`$ | 根据 dd 需求弹性变动的加成参数 |
| $`\omega(x)`$ | 差异化部门占名义收入的支出份额 |
| $`x_e,p_e,n_e`$ | 市场（自由进入）均衡产量、售价与企业数 |
| $`x_c`$ | 有约束福利最优下的每企业产量 |

应特别注意 **$`\rho(x)`$、$`\beta(x)`$ 现在均可随 $`x`$ 改变**，不能直接用前面固定弹性部分的常数替代。

## 1. （1.33）可变弹性偏好设定

原书将两部门效用写成：

**式（1.33）**

```math
\boxed{ u=x_0^{1-\gamma}\left[\sum_{i=1}^{n}v(x_i)\right]^\gamma, \qquad 0<\gamma<1. }
```

对比固定弹性 CES 形式：这里的内层不是 $`\bigl(\sum_i x_i^\rho\bigr)^{1/\rho}`$，而是一般加总 $`V=\sum_i v(x_i)`$。若 $`v`$ 不是齐次幂函数，组内偏好通常**不位似**，需求价格弹性也不再是固定常数。

## 2. （1.34）单企业 dd 需求弹性

预算为 $`x_0+\sum_i p_i x_i=I`$。给定 $`n`$，内部最优的边际替代率等于品种价格：

**式（A）**

$$p_i=\frac{\partial u/\partial x_i}{\partial u/\partial x_0} =\frac{\gamma}{1-\gamma}\, \frac{x_0\,v'(x_i)}{\sum_j v(x_j)}.$$

在企业足够小、其他品种数量与整体支出/价格的变化可忽略的 dd **局部需求近似**中，把式 (A) 右侧除 $`v'(x_i)`$ 以外的共同因子视作常数，因此：

$$p_i\propto v'(x_i).$$

对数求导：

$$\frac{\mathrm d\ln p_i}{\mathrm d\ln x_i} =\frac{x_i v''(x_i)}{v'(x_i)}.$$

取倒数并改符号，得到需求弹性的绝对值：

**式（1.34）**

```math
\boxed{ -\frac{\partial\ln x_i}{\partial\ln p_i} =-\frac{v'(x_i)}{x_i v''(x_i)}>0. }
```

**严谨性提醒**：式（1.34）是“忽略单企业对整体需求环境的反馈”的 dd 弹性；有限品种数下若允许 $`x_0`$、$`V`$ 同时内生变化，直接从（A）得到的精确个体需求弹性通常还包含额外反馈项。

## 3. （1.35）用 $`\beta(x)`$ 表示可变需求弹性

类比 P10 的固定弹性参数，定义：

**式（1.35）**

$$\boxed{ \frac{1+\beta(x)}{\beta(x)} =-\frac{v'(x)}{xv''(x)}. }$$

因为 $`v'>0`$、$`v''<0`$，右边为正。要使 $`\beta(x)>0`$ 并得到有限的正加成，还需右侧大于 1，例如满足 $`-xv''(x)/v'(x)\in(0,1)`$。此时：

$$\frac{\beta(x)}{1+\beta(x)} =-\frac{xv''(x)}{v'(x)},$$

从而：

**式（B）**

$$\boxed{ \frac{1}{1+\beta(x)}=1+\frac{xv''(x)}{v'(x)}. }$$

这一恒等式将用来连接市场均衡、福利最优和 $`\rho'(x)`$。

## 4. （1.36）对称需求和同质品消费

令 $`x_i=x`$、$`p_i=p`$，则 $`V=n v(x)`$。由（A）：

$$p=\frac{\gamma}{1-\gamma}\frac{x_0 v'(x)}{n v(x)}.$$

乘以 $`nx`$ 并定义：

$$\rho(x)\equiv\frac{xv'(x)}{v(x)},$$

便有：

**式（C）**

$$npx=\frac{\gamma\rho(x)}{1-\gamma}x_0.$$

又因预算 $`x_0+npx=I`$，代入 $`x_0=I-npx`$：

$$npx=\frac{\gamma\rho(x)}{1-\gamma}(I-npx).$$

移项并除以 $`I`$：

$$\frac{npx}{I} =\frac{\gamma\rho(x)}{\gamma\rho(x)+1-\gamma}.$$

将右侧定义为 $`\omega(x)`$，于是：

**式（1.36）**

$$\boxed{ x=\frac{I\,\omega(x)}{np}, \qquad x_0=I[1-\omega(x)]. }$$

与此前支出份额 $`s(q)`$ 不同，这里在**对称状态**下，部门份额由单企业的消费量 $`x`$ 经 $`\rho(x)`$ 决定。

## 5. （1.37）定义 $`\omega(x)`$ 和 $`\rho(x)`$

上节给出了：

**式（1.37）**

$$\boxed{ \omega(x)=\frac{\gamma\rho(x)} {\gamma\rho(x)+1-\gamma}, \qquad \rho(x)=\frac{xv'(x)}{v(x)}. }$$

如果满足 $`0<\rho(x)<1`$，则 $`0<\omega(x)<\gamma<1`$。例如：

```math
\omega(x)<\gamma \iff \frac{\rho(x)}{\gamma\rho(x)+1-\gamma}<1 \iff(1-\gamma)\rho(x)<1-\gamma \iff\rho(x)<1.
```

还可以对 $`\omega`$ 求导：

**式（D）**

$$\frac{\mathrm d\omega}{\mathrm dx} =\frac{\gamma(1-\gamma)\rho'(x)} {[\gamma\rho(x)+1-\gamma]^2}.$$

所以 **$`\omega'(x)`$ 与 $`\rho'(x)`$ 同号**，这将在 P15 的（1.46）中用到。

## 6. （1.38）垄断竞争市场的可变加成定价

利润函数：

$$\pi_i=(p_i-c)x_i(p_i)-a.$$

一阶条件为：

$$x_i+(p_i-c)\frac{\partial x_i}{\partial p_i}=0.$$

除以 $`x_i`$，再乘以 $`p_i/p_i`$：

$$1+\frac{p_i-c}{p_i}\frac{\partial\ln x_i}{\partial\ln p_i}=0.$$

由（1.35）可得：

$$\frac{p_i-c}{p_i} =\frac{\beta(x_i)}{1+\beta(x_i)}.$$

于是：

$$p_i-c=\beta(x_i)c.$$

对称市场中：

**式（1.38）**

$$\boxed{ p_e=c[1+\beta(x_e)]. }$$

**区别于（1.17）**：现在 $`\beta`$ 随均衡产量变化，因此定价和最优规模需要联合确定，不再是常数加成独立于产量的简单情形。

## 7. （1.39）自由进入、零利润与均衡规模

自由进入均衡要求：

$$(p_e-c)x_e=a.$$

由（1.38）$`p_e-c=c\beta(x_e)`$，因此：

$$c\beta(x_e)x_e=a \quad\Longrightarrow\quad \beta(x_e)=\frac{a}{cx_e}.$$

故：

**式（1.39）**

$$\boxed{ \frac{cx_e}{a+cx_e} =\frac{1}{1+\beta(x_e)}. }$$

这是决定市场均衡每企业产量 $`x_e`$ 的**隐式方程**。要保证唯一解还需相应单调性与存在性条件。

## 8. （1.40）均衡企业数

式（1.36）在 $`I=1`$ 时给出：

$$n_e p_e x_e=\omega(x_e).$$

零利润意味着：

$$p_e x_e=a+cx_e.$$

结合两式：

$$n_e(a+cx_e)=\omega(x_e),$$

所以：

**式（1.40）**

$$\boxed{n_e=\frac{\omega(x_e)}{a+cx_e}.}$$

解释：差异化部门总支出是 $`\omega(x_e)`$，其中每家企业的总营业收入刚好覆盖 $`a+cx_e`$，故二者相除是活跃企业数。计算中将 $`n`$ 视为连续变量是大企业数近似。

## 9. （1.41）把有约束最优的效用写成 $`x`$ 的一元函数

**有约束最优**允许规划者选择 $`n,x`$，但必须让企业靠销售收入覆盖成本：

$$px=a+cx,\qquad p=c+\frac ax.$$

仍在 $`I=1`$ 和对称需求式（1.36）的前提下：

$$npx=\omega(x) \quad\Longrightarrow\quad \boxed{n=\frac{\omega(x)}{a+cx}},$$

$$\boxed{x_0=1-\omega(x)}.$$

代回式（1.33）：

**式（E）**

$$u(x)= [1-\omega(x)]^{1-\gamma} \left[\frac{\omega(x)v(x)}{a+cx}\right]^\gamma.$$

令 $`D(x)=\gamma\rho(x)+1-\gamma`$，则：

$$1-\omega(x)=\frac{1-\gamma}{D(x)}, \qquad \omega(x)=\frac{\gamma\rho(x)}{D(x)}.$$

代回式 (E)，可得：

```math
\begin{aligned} u(x) &=\left(\frac{1-\gamma}{D}\right)^{1-\gamma} \left[\frac{\gamma\rho(x)v(x)}{D(a+cx)}\right]^\gamma\\ &=\gamma^\gamma(1-\gamma)^{1-\gamma} \frac{\left[\rho(x)v(x)/(a+cx)\right]^\gamma} {\gamma\rho(x)+1-\gamma}. \end{aligned}
```

即原书公式：

**式（1.41）**

$$\boxed{ u(x)=\gamma^\gamma(1-\gamma)^{1-\gamma} \frac{\left[\dfrac{\rho(x)v(x)}{a+cx}\right]^\gamma} {\gamma\rho(x)+1-\gamma}. }$$

**这里的社会规划者只剩一个选择变量 $`x`$**，因为约束已经把 $`n`$、$`x_0`$ 表示为 $`x`$ 的函数。

## 10. （1.42）有约束最优的一阶条件和原书核对

对（1.41）取对数（忽略常数项）：

$$\ln u(x) =\gamma\left[\ln\rho(x)+\ln v(x)-\ln(a+cx)\right] -\ln D(x)+\text{常数}.$$

对 $`\ln x`$ 求导：

**式（F）**

```math
\begin{aligned} \frac{\mathrm d\ln u}{\mathrm d\ln x} &=\gamma\left[ \frac{x\rho'(x)}{\rho(x)} +\frac{xv'(x)}{v(x)} -\frac{cx}{a+cx} \right] -\frac{\gamma x\rho'(x)}{D(x)}\\ &=\gamma\left[ \rho(x)+\frac{x\rho'(x)}{\rho(x)} -\frac{cx}{a+cx} -\frac{x\rho'(x)}{D(x)} \right]. \end{aligned}
```

另外直接对 $`\rho(x)=xv'(x)/v(x)`$ 求对数导数：

**式（G）**

$$\frac{x\rho'(x)}{\rho(x)} =1+\frac{xv''(x)}{v'(x)}-\rho(x).$$

由（1.35）：

**式（H）**

$$\boxed{ \rho(x)+\frac{x\rho'(x)}{\rho(x)} =\frac{1}{1+\beta(x)}. }$$

在有约束最优内点 $`x_c`$，令（F）为零，利用（H）与 $`\omega(x)/[\gamma\rho(x)]=1/D(x)`$，得：

**式（1.42）**

$$\boxed{ \frac{cx_c}{a+cx_c} =\frac{1}{1+\beta(x_c)} -\frac{\omega(x_c)\,x_c\rho'(x_c)} {\gamma\rho(x_c)}. }$$

### 必须注明的书页疑点

这张照片的（1.42）左边印刷看起来是 $`cx_e/(a+x_e)`$，右边也使用 $`x_e`$，并且 $`\rho`$ 后的导数撇号不够清晰。

但从**紧挨其前的（1.41）求一阶条件**，毫无疑问应使用：
- **$`a+cx_c`$**：与本页（1.39）、（1.40）的总成本一致；
- **$`x_c`$**：这是有约束社会最优的解，而 $`x_e`$ 是市场均衡；
- **$`\rho'(x_c)`$**：该修正项来自对 $`\rho(x)`$ 求导，缺少撇号就无法成立。

因此在正式学习笔记中写为上面的“严格推导式”，同时将图片原式列为**待对照其它印次确认的排印/记号疑点**。绝不直接以疑似误印式代替数学推导。

## 11. 关键结果速览

| 公式 | 内容 | 逻辑来源 |
| :--- | :--- | :--- |
| （1.33） | $`u=x_0^{1-\gamma}[\sum_i v(x_i)]^\gamma`$ | 非齐次组内效用的模型设定 |
| （1.34） | $`-\partial\ln x_i/\partial\ln p_i=-v'(x_i)/(x_i v''(x_i))`$ | 局部 dd 需求：$`p_i\propto v'(x_i)`$ |
| （1.35） | $`(1+\beta(x))/\beta(x)=-v'(x)/(xv''(x))`$ | 定义可变加成函数 $`\beta(x)`$ |
| （1.36） | $`x=I\omega(x)/(np)`$，$`x_0=I[1-\omega(x)]`$ | 组间需求与预算 |
| （1.37） | $`\omega(x)=\gamma\rho(x)/[\gamma\rho(x)+1-\gamma]`$ | 内点最优的支出份额 |
| （1.38） | $`p_e=c[1+\beta(x_e)]`$ | 单企业利润最大化 |
| （1.39） | $`cx_e/(a+cx_e)=1/[1+\beta(x_e)]`$ | 零利润与最优定价联立 |
| （1.40） | $`n_e=\omega(x_e)/(a+cx_e)`$ | 对称支出与零利润 |
| （1.41） | 见第 9 节 | 消去 $`n,x_0`$，得到有约束福利函数 |
| （1.42） | 见第 10 节 | 对（1.41）求导，分辨市场与规划者条件 |

**对应下一篇**：[P15：可变弹性下的福利与市场比较（1.43）—（1.52）](variable-elasticity-welfare-equations-1-43-to-1-52-p15.md)。

---

*本文件用于逐式学习；公式（1.42）的疑点按照片和数学一致性标注，不宣称已完成出版社勘误核实。*
