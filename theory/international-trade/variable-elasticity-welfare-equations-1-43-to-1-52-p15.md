# 《国际贸易应用模型》P15：可变弹性下的福利比较（1.43）—（1.52）

> **教材**：刘文革、裴莹编著，《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，ISBN 978-7-302-71633-4。  
> **原书位置**：第一章“模型设定与推导”，**二、可变弹性的情形**，P15，公式（1.43）—（1.52）。  
> **上篇**：[P14（1.33）—（1.42）可变弹性需求与约束最优](variable-elasticity-equations-1-33-to-1-42-p14.md)；**下篇**：[P16（1.53）最优品种数比较](variable-elasticity-variety-equation-1-53-p16.md)。

## 0. 三套解与共同前提

- 下标 $`e`$：自由进入市场均衡（equilibrium）。
- 下标 $`c`$：有约束社会最优（constrained optimum），企业须独立覆盖固定成本。
- 下标 $`u`$：无约束社会最优（unconstrained optimum），允许一次性转移支付补偿固定成本。

沿用 P14 定义：

$$\rho(x)=\frac{xv'(x)}{v(x)},\quad \omega(x)=\frac{\gamma\rho(x)}{\gamma\rho(x)+1-\gamma},\quad \theta_{\mathrm{dd}}(x)=\frac{1+\beta(x)}{\beta(x)} =-\frac{v'(x)}{xv''(x)}.$$

假设 $`v>0`$、$`v'>0`$、$`v''<0`$、$`0<\rho(x)<1`$、$`\beta(x)>0`$、$`0<\gamma<1`$、$`a,c>0`$。讨论严格的不等式排序时，还要假定比较所涉及的区间内 $`\rho'(x)`$ 不变号，并且福利函数内点最优唯一、相关需求曲线满足局部稳定/单峰性等条件；**单凭某一点导数的符号不够推出全局排序**。

P14 的市场均衡条件（1.39）为：

**式（1.39）**

$$\boxed{ \frac{cx_e}{a+cx_e} =\frac{1}{1+\beta(x_e)}. }$$

约束社会最优的一阶条件（数学一致的版本）为：

**式（1.42）**

$$\boxed{ \frac{cx_c}{a+cx_c} =\frac{1}{1+\beta(x_c)} -\frac{\omega(x_c)x_c\rho'(x_c)}{\gamma\rho(x_c)}. }$$

设有约束目标效用写为 P14 的 $`u_c(x)`$，便可逐一比较。

## 1. （1.43）约束最优产量与市场产量如何比较？

先回忆 P14 求出的福利目标的对数导数：

**式（A）**

$$\frac{\mathrm d\ln u_c(x)}{\mathrm d\ln x} =\gamma\left[ \frac{1}{1+\beta(x)} -\frac{cx}{a+cx} -\frac{\omega(x)x\rho'(x)}{\gamma\rho(x)} \right].$$

**在市场均衡点 $`x_e`$ 上**，前两项根据（1.39）抵消：

**式（B）**

$$\left. \frac{\mathrm d\ln u_c(x)}{\mathrm d\ln x} \right|_{x_e} = -\frac{\omega(x_e)x_e\rho'(x_e)}{\rho(x_e)}.$$

因 $`\omega,x_e,\rho>0`$，其符号恰好**与 $`\rho'(x_e)`$ 相反**。

若受约束社会福利关于 $`x`$ 单峰且最大值位于内点：

- 当 $`\rho'(x)>0`$（相关区间内）时，市场点的福利斜率负，福利最优应向**更小产量**移动，即 $`x_c<x_e`$；
- 当 $`\rho'(x)<0`$ 时，市场点的福利斜率正，福利最优应向**更大产量**移动，即 $`x_c>x_e`$。

用无歧义的方式写出原书（1.43）：

**式（1.43）**

$$\boxed{ \begin{cases} x_c<x_e,&\rho'(x)>0,\\ x_c>x_e,&\rho'(x)<0. \end{cases} }$$

如果 $`\rho'(x)=0`$ 且相应最优唯一，二者在这个机制下趋于相同；若符号随 $`x`$ 变化、存在多个局部最优，应解原始问题，不能套用简单双向排序。

## 2. （1.44）两套价格如何比较？

有约束解和市场解均要求企业零利润：

**式（C）**

$$(p-c)x=a$$

移项并除以 $`x`$：

$$p=c+\frac{a}{x}$$

求导：

$$\frac{\mathrm dp}{\mathrm dx}=-\frac{a}{x^2}<0.$$

因此每企业产量越高，**摊到每单位商品上的固定成本越少，零利润价格越低**。从而：

**式（1.44）**

$$\boxed{ \begin{cases} p_c>p_e,&x_c<x_e,\\ p_c<p_e,&x_c>x_e. \end{cases} }$$

合并（1.43）：$`\rho'>0`$ 时 $`p_c>p_e`$；$`\rho'<0`$ 时 $`p_c<p_e`$。

请注意，与前一节固定弹性结论（1.24）不同，**现在有约束最优价格一般不等于市场价格**，原因在于 dd 弹性与加成会随产量改变。

## 3. （1.45）最优企业数与市场企业数的比较

P14 的对称支出份额和零利润条件给出：

**式（D）**

$$\boxed{ n(x)=\frac{\omega(x)}{a+cx}. }$$

注意：比较产量并不能仅仅通过固定的分母得出企业数排序，因为分子 $`\omega(x)`$ 也会随产量变化。严格求导：

**式（E）**

$$\begin{aligned} \frac{\mathrm d\ln n(x)}{\mathrm d\ln x} &=\frac{\mathrm d\ln\omega(x)}{\mathrm d\ln x} -\frac{cx}{a+cx}\\ &=[1-\omega(x)]\frac{x\rho'(x)}{\rho(x)} -\frac{cx}{a+cx}. \end{aligned}$$

于是，在相关均衡分支上若满足

**式（F）**

$$\boxed{ [1-\omega(x)]\frac{x\rho'(x)}{\rho(x)} <\frac{cx}{a+cx}, }$$

则 $`n'(x)<0`$，产量较高对应较少企业。这是原书 dd / DD 需求曲线和成本曲线排序的数学版本。

在该单调分支下：

**式（1.45）**

$$\boxed{ \begin{cases} n_c>n_e,&x_c<x_e,\\ n_c<n_e,&x_c>x_e. \end{cases} }$$

换句话说，若 $`\rho'>0`$，通常有约束规划者会选择**更多企业、每企业更小产量**；若 $`\rho'<0`$，则反过来。

对单调性作局部自检：在市场点 $`x_e`$，由（1.39）及（1.47）的关系可以把（E）写为

$$\left.\frac{\mathrm d\ln n}{\mathrm d\ln x}\right|_{x_e} =-\rho(x_e)-\omega(x_e)\frac{x_e\rho'(x_e)}{\rho(x_e)}.$$

由于市场条件要求 $`1/(1+\beta(x_e))>0`$，即 $`x_e\rho'/\rho>-\rho`$，且 $`0<\omega<1`$，可得该处导数严格小于零。**但局部下降不意味着不检查其它区间即可推出全局排序。**

## 4. （1.46）同质商品的支出和消费

式（1.36）说明，在名义收入 $`I=1`$ 下：

$$x_0=1-\omega(x).$$

而 P14 已证明：

$$\omega'(x)= \frac{\gamma(1-\gamma)\rho'(x)} {[\gamma\rho(x)+1-\gamma]^2},$$

所以 $`\omega'(x)`$ 与 $`\rho'(x)`$ 同号。

结合（1.43）：

- 若 $`\rho'>0`$，则 $`x_c<x_e`$，所以 $`\omega(x_c)<\omega(x_e)`$；
- 若 $`\rho'<0`$，则 $`x_c>x_e`$，但 $`\omega`$ 随 $`x`$ 下降，仍有 $`\omega(x_c)<\omega(x_e)`$。

两种情形统一得到：

$$x_{0c}=1-\omega(x_c) > 1-\omega(x_e)=x_{0e}.$$

所以原书（1.46）为：

**式（1.46）**

$$\boxed{x_{0c}>x_{0e}.}$$

这说明有约束福利最优配置在同质商品上的消费量高于市场均衡（在上述比较条件下成立）。

## 5. （1.47）$`\rho'(x)`$、$`\rho(x)`$ 与需求弹性之间的恒等式

从 $`\rho(x)=xv'(x)/v(x)`$ 出发，取对数：

$$\ln\rho=\ln x+\ln v'(x)-\ln v(x).$$

对 $`\ln x`$ 求导：

$$\begin{aligned} \frac{x\rho'(x)}{\rho(x)} &=1+\frac{xv''(x)}{v'(x)} -\frac{xv'(x)}{v(x)}\\ &=1+\frac{xv''(x)}{v'(x)}-\rho(x). \end{aligned}$$

由定义（1.35），有 $`1+xv''/v'=1/[1+\beta(x)]`$，因此：

**式（1.47）**

$$\boxed{ \frac{x\rho'(x)}{\rho(x)} =\frac{1}{1+\beta(x)}-\rho(x). }$$

这条公式解释了为何**需求弹性与效用规模弹性有关，但它们变化的符号未必相同**。若 $`v(x)=x^r`$、$`0<r<1`$，则 $`\rho=r`$ 是常数、$`\rho'=0`$，并且 $`\beta=(1-r)/r`$ 也是常数。

## 6. （1.48）无约束社会规划者的效用函数

在无约束最优中，不要求企业靠高于边际成本的售价覆盖 $`a`$，而由规划者将整个社会资源在两部门和产品品种之间分配：

$$x_0+n(a+cx)=1.$$

对称的差异化品种效用贡献是 $`\sum_i v(x_i)=n v(x)`$。代入（1.33）：

**式（1.48）**

$$\boxed{ u(n,x)=\bigl[nv(x)\bigr]^\gamma \bigl[1-n(a+cx)\bigr]^{1-\gamma}. }$$

这里约束已体现在括号中，须满足 $`n>0`$、$`x>0`$、$`n(a+cx)<1`$。

## 7. （1.49）无约束最优的边际成本价格

令 $`D=a+cx`$、$`x_0=1-nD`$，对（1.48）的对数求导。

对 $`x`$ 的 FOC：

**式（G）**

$$\boxed{ \frac{\gamma v'(x)}{v(x)} =\frac{(1-\gamma)nc}{x_0}. }$$

对 $`n`$ 的 FOC：

**式（H）**

$$\boxed{ \frac{\gamma}{n} =\frac{(1-\gamma)(a+cx)}{x_0}. }$$

这里下标 $`u`$ 表示将 $`x,n,x_0`$ 替换为无约束最优值。式（H）可以简化：

**式（I）**

$$\gamma[1-n(a+cx)]=(1-\gamma)n(a+cx)$$

整理后，得到无约束最优企业数的条件：

$$n_u(a+cx_u)=\gamma$$

故 $`x_{0u}=1-\gamma`$。

在消费者分配的一阶条件（见 P14）中，对称单品种价格需满足：

**式（J）**

$$p=\frac{\gamma x_0v'(x)}{(1-\gamma)nv(x)}$$

代入 $`x_{0u}=1-\gamma`$ 与 $`n_u=\gamma/(a+cx_u)`$：

$$\begin{aligned} p_u &=\frac{\gamma}{1-\gamma} \frac{(1-\gamma)v'(x_u)} {[\gamma/(a+cx_u)]v(x_u)}\\ &=(a+cx_u)\frac{v'(x_u)}{v(x_u)}. \end{aligned}$$

而式（G）与（H）相除正好给出 $`v'(x_u)/v(x_u)=c/(a+cx_u)`$，因此：

**式（1.49）**

$$\boxed{p_u=c.}$$

同样，这里的 $`p_u`$ 是**实现规划者配置的边际成本价格/影子实施价格**。企业按这一价格出售时无法自行收回固定成本，需要一次性转移支付。

## 8. （1.50）无约束最优的每企业产量

用上两条一阶条件之比：

$$\frac{v'(x_u)}{v(x_u)} =\frac{c}{a+cx_u}.$$

左右乘以 $`x_u`$：

$$\frac{x_uv'(x_u)}{v(x_u)} =\frac{cx_u}{a+cx_u}.$$

按 $`\rho(x)`$ 的定义：

**式（1.50）**

$$\boxed{ \frac{cx_u}{a+cx_u}=\rho(x_u). }$$

它是决定无约束最优单企业产量的隐式方程；只有具体给定 $`v(x)`$ 后才能进一步求解。

## 9. （1.51）无约束最优企业数量

由式（I），直接解出：

**式（1.51）**

$$\boxed{ n_u=\frac{\gamma}{a+cx_u}. }$$

因为同质品消费 $`x_{0u}=1-\gamma`$，在没有定价加成的社会规划者解中，差异化部门**资源份额**为 $`\gamma`$。

## 10. （1.52）无约束产量与有约束产量的比较

定义严格递增的成本份额函数：

$$g(x)=\frac{cx}{a+cx}, \qquad g'(x)=\frac{ca}{(a+cx)^2}>0.$$

无约束最优要求（1.50）：

**式（K）**

$$\boxed{g(x_u)=\rho(x_u)}.$$

而根据 P14 的受约束一阶条件（1.42）和恒等式（1.47），可将受约束 FOC 改写为：

**式（L）**

$$\begin{aligned} g(x_c) &=\rho(x_c)+\frac{x_c\rho'(x_c)}{\rho(x_c)} -\frac{\omega(x_c)x_c\rho'(x_c)}{\gamma\rho(x_c)}\\ &=\rho(x_c) +\underbrace{[1-\omega(x_c)]\,[1-\rho(x_c)]}_{>0} \frac{x_c\rho'(x_c)}{\rho(x_c)}. \end{aligned}$$

第二行使用了恒等式 $`1-\omega/\gamma=(1-\omega)(1-\rho)`$，该式可以直接从 $`\omega=\gamma\rho/(\gamma\rho+1-\gamma)`$ 验证。

因此，在受约束解 $`x_c`$ 处：

$$\operatorname{sgn}\bigl(g(x_c)-\rho(x_c)\bigr) =\operatorname{sgn}\rho'(x_c).$$

如果 $`g(x)-\rho(x)`$ 在比较区间内严格递增、具有唯一零点（这是**额外的单交叉/规律性条件**），则：

**式（1.52）**

$$\boxed{ \begin{cases} x_u<x_c,&\rho'(x)>0,\\ x_u>x_c,&\rho'(x)<0. \end{cases} }$$

即：若 $`\rho'>0`$，无约束最优选择更小的单企业产出；若 $`\rho'<0`$，则选择更大的单企业产出。只有（1.50）和（1.42）两个方程而没有形状约束时，不应声称这一排序总是无条件成立。

## 11. 常弹性退化例子：检查三套方案

令 $`v(x)=x^r`$，$`0<r<1`$。此时：

$$\rho(x)=r,\qquad \rho'(x)=0,\qquad \beta=\frac{1-r}{r},\qquad \omega=\frac{\gamma r}{\gamma r+1-\gamma}.$$

市场零利润（1.39）给出：

$$\frac{cx_e}{a+cx_e}=r \quad\Longrightarrow\quad x_e=\frac{ar}{c(1-r)}.$$

受约束条件（1.42）中的 $`\rho'`$ 修正项消失，故：

$$x_c=x_e.$$

无约束条件（1.50）也给出：

$$x_u=\frac{ar}{c(1-r)}=x_c=x_e.$$

但品种数不同：

$$n_c=n_e=\frac{\omega}{a+cx_e}, \qquad n_u=\frac{\gamma}{a+cx_u}.$$

由于 $`r<1\Rightarrow\omega<\gamma`$，因而 $`n_u>n_c=n_e`$。这说明**单企业产量可能相同，而品种数和福利依然不同**，与固定弹性结论相衔接。

## 12. 原书十个公式速查

| 编号 | 主结论 | 关键来源 |
| :--- | :--- | :--- |
| （1.43） | $`\rho'>0\Rightarrow x_c<x_e`$；$`\rho'<0\Rightarrow x_c>x_e`$ | 在 $`x_e`$ 处评价约束福利目标的斜率 |
| （1.44） | $`p_c=c+a/x_c`$ 与 $`p_e=c+a/x_e`$，价格排序反向 | 零利润价格随 $`x`$ 下降 |
| （1.45） | $`x_c<x_e\Rightarrow n_c>n_e`$（要求适当单调性） | 对 $`n(x)=\omega(x)/(a+cx)`$ 求导 |
| （1.46） | $`x_{0c}>x_{0e}`$ | $`\omega'`$ 与 $`\rho'`$ 同号 |
| （1.47） | $`x\rho'/\rho=1/(1+\beta)-\rho`$ | 对 $`\rho=xv'/v`$ 求导 |
| （1.48） | $`u=[nv(x)]^\gamma[1-n(a+cx)]^{1-\gamma}`$ | 资源约束与对称效用 |
| （1.49） | $`p_u=c`$ | 两条规划者 FOC + 实施价格条件 |
| （1.50） | $`cx_u/(a+cx_u)=\rho(x_u)`$ | 规划者 FOC 联立 |
| （1.51） | $`n_u=\gamma/(a+cx_u)`$ | 对 $`n`$ 求一阶条件 |
| （1.52） | $`\rho'>0\Rightarrow x_u<x_c`$；$`\rho'<0\Rightarrow x_u>x_c`$ | 对比无约束与受约束最优条件 |

**下一篇**：[P16（1.53）：进一步判断无约束与约束最优品种数量](variable-elasticity-variety-equation-1-53-p16.md)。

---

*对原书的序关系采取逐情形写法，以免“$`\lessgtr/\gtrless`$”重叠符号产生歧义。形状、唯一性及单调性条件是本笔记为了严格性补充的假设。*
