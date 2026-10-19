# 《国际贸易应用模型》P10：公式（1.9）—（1.16）逐式推导

> **原书位置**：第 10 页（P10），“第三节 模型设定与推导——一、固定弹性的情形——（一）需求函数”。  
> **重点**：CES 条件需求、价格指数的单品种价格弹性、张伯伦 dd / DD 需求曲线、对称均衡、相对需求与替代弹性。  
> **教材信息**：刘文革、裴莹编著，《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版；ISBN 978-7-302-71633-4。  
> **依据**：原书第 10 页（P10）照片及公式（1.9）—（1.16）。  
> **前一篇**：[P9 公式（1.4）—（1.8）推导](two-stage-budgeting-equations-1-4-to-1-8-p9.md)。

## 0. 准备：沿用 P9 的记号

模型中有 $`n`$ 个差异化商品，数量 $`x_i`$、价格 $`p_i`$，同质商品 $`x_0`$ 的价格规范化为 1，名义收入为 $`I`$：

$$
u=U\left[x_0,\left(\sum_{i=1}^n x_i^\rho\right)^{1/\rho}\right],
\qquad 0<\rho<1,\qquad
x_0+\sum_{i=1}^n p_ix_i=I.
$$

差异化商品的综合数量（P9 记为 $`Y`$，本页记为 $`y`$）和 CES 价格指数是

$$
y=\left(\sum_{i=1}^n x_i^\rho\right)^{1/\rho},
\qquad
q=\left(\sum_{i=1}^n p_i^{-1/\beta}\right)^{-\beta},
\qquad
\beta=\frac{1-\rho}{\rho}>0.
\tag{1.6}
$$

两个关键恒等式：

$$
\sigma_{\mathrm{in}}
=\frac{1}{1-\rho}=1+\frac1\beta,
\qquad
1-\sigma_{\mathrm{in}}=-\frac1\beta.
$$

如果差异化商品部门的名义支出份额为 $`s(q)`$，则

$$
y=\frac{I s(q)}q,
\qquad
x_0=I[1-s(q)],
\qquad
\theta(q)=\frac{q s'(q)}{s(q)}.
\tag{1.7–1.8}
$$

这里按前一篇笔记，**默认外层偏好满足使 $`s`$ 只依赖相对综合价格 $`q`$ 的条件**（例如外层位似偏好），且考虑内点解。若外层非位似，份额一般应写为 $`s(q,I)`$，下面的固定收入价格偏导仍可相应推广。

注意：$`q`$ 是复合价格指数；$`\rho,\beta`$ 控制**组内**品种替代弹性，不能与上层部门间替代弹性 $`\sigma_{\mathrm{out}}(q)`$ 混淆。

## 1. （1.9）品种需求函数：组内成本最小化

给定要获得的综合数量 $`y`$，最小化支出

$$
\min_{\{x_i\}}\sum_{i=1}^n p_ix_i
\quad\text{s.t.}\quad
\sum_{i=1}^n x_i^\rho=y^\rho.
$$

拉格朗日函数

$$
\mathcal L=\sum_i p_ix_i+
\lambda\left[y^\rho-\sum_i x_i^\rho\right].
$$

一阶条件

$$
p_i=\lambda\rho x_i^{\rho-1}
\quad\Longrightarrow\quad
x_i=(\lambda\rho)^{1/(1-\rho)}p_i^{-1/(1-\rho)}.
$$

令 $`A=(\lambda\rho)^{\sigma_{\mathrm{in}}}`$，得到 $`x_i=Ap_i^{-\sigma_{\mathrm{in}}}`$。代入 CES 数量聚合式，

$$
\begin{aligned}
y
&=A\left(\sum_i p_i^{-\sigma_{\mathrm{in}}\rho}\right)^{1/\rho}\\
&=A\left(\sum_i p_i^{-1/\beta}\right)^{1/\rho}\\
&=A\left(q^{-1/\beta}\right)^{1/\rho}
=Aq^{-\sigma_{\mathrm{in}}}.
\end{aligned}
$$

所以 $`A=yq^{\sigma_{\mathrm{in}}}`$，品种条件需求为（补全原书中遗漏的综合数量系数 $`y`$）：

$$
\boxed{
x_i=y\left(\frac q{p_i}\right)^{1/(1-\rho)}
=y\left(\frac q{p_i}\right)^{1+1/\beta}.
}
\tag{1.9}
$$

**原书核对**：P10 图片的（1.9）右边印为 $`(q/p_i)^{1/(1-\rho)}`$，缺少 $`y`$。在一般数量单位下，右侧是 **$`x_i/y`$** 而不是 $`x_i`$；若未显式设 $`y=1`$，应补上 $`y`$。将这个遗漏当作排印/记号问题，不将其视为新的经济假设。

代入 P9 的 $`y=Is(q)/q`$，可得到**完整的非条件需求**：

$$
\boxed{
x_i=I\,s(q)\,q^{\sigma_{\mathrm{in}}-1}\,p_i^{-\sigma_{\mathrm{in}}}.
}
\tag{A}
$$

这一步对于后面区分大样本近似与精确弹性至关重要。

## 2. （1.10）单个品种价格对 $`q`$ 的影响

从（1.6）

$$
q=\left(\sum_{j=1}^n p_j^{-1/\beta}\right)^{-\beta}.
$$

取对数并对 $`\ln p_i`$ 求偏导（其他品种价格不变）：

$$
\begin{aligned}
\frac{\partial\ln q}{\partial\ln p_i}
&=-\beta
\frac{\partial}{\partial\ln p_i}
\ln\left(\sum_j p_j^{-1/\beta}\right)\\
&=-\beta\,
\frac{(-1/\beta)p_i^{-1/\beta}}{\sum_jp_j^{-1/\beta}}\\
&=\frac{p_i^{-1/\beta}}{\sum_jp_j^{-1/\beta}}.
\end{aligned}
$$

又有 $`\sum_jp_j^{-1/\beta}=q^{-1/\beta}`$，因此

$$
\boxed{
\frac{\partial\ln q}{\partial\ln p_i}
=\left(\frac q{p_i}\right)^{1/\beta}
\equiv w_i.
}
\tag{1.10}
$$

进一步验证 $`w_i`$ 是**组内支出份额**：

$$
\frac{p_i x_i}{qy}
=\frac{p_i y(q/p_i)^{\sigma_{\mathrm{in}}}}{qy}
=\left(\frac q{p_i}\right)^{\sigma_{\mathrm{in}}-1}
=\left(\frac q{p_i}\right)^{1/\beta}
=w_i.
$$

因而 $`\sum_i w_i=1`$。当各品种对称（$`p_i=p`$），则 $`w_i=1/n`$。

重要限定：仅说“$`n`$ 很大”还不足以保证某个特定商品的份额很小；需额外排除某一品种占据不成比例的大份额。在对称市场中，$`w_i=1/n\to0`$。

## 3. （1.11）dd 需求曲线的自身价格弹性

### 3.1 大品种数近似（教材展示的公式）

对（1.9）取对数：

$$
\ln x_i=\ln y+\sigma_{\mathrm{in}}\ln q
-\sigma_{\mathrm{in}}\ln p_i.
$$

如果一家企业规模很小，变动自己的 $`p_i`$ 对 $`q`$ 和总体部门购买力的影响均可忽略，则

$$
\boxed{
\left.\frac{\partial\ln x_i}{\partial\ln p_i}\right|_{\mathrm{dd}}
\simeq-\sigma_{\mathrm{in}}
=-\frac1{1-\rho}
=-\frac{1+\beta}{\beta}.
}
\tag{1.11}
$$

它是**其他企业价格不变**时，单一企业所面对的较陡峭（绝对弹性通常较大）的价格竞争关系，传统上称为张伯伦的 **dd 曲线**。

**原书核对**：图片中（1.11）左侧印为 $`\partial\ln q/\partial\ln p_i`$，但从（1.10）知道它应为正的份额 $`w_i`$，绝不可能同时等于负数 $`-1/(1-\rho)`$。与文字及一阶条件一致的左侧应是 $`\partial\ln x_i/\partial\ln p_i`$。

### 3.2 有限 $`n`$ 的精确修正（比课本近似更一般）

不忽略 $`q`$ 和 $`s(q)`$ 对单品种涨价的反应，从（A）：

$$
\ln x_i
=\ln I+\ln s(q)
+(\sigma_{\mathrm{in}}-1)\ln q
-\sigma_{\mathrm{in}}\ln p_i.
$$

对 $`\ln p_i`$ 求偏导：

$$
\frac{\partial\ln x_i}{\partial\ln p_i}
=-\sigma_{\mathrm{in}}
+\left[
\underbrace{\frac{\mathrm d\ln s(q)}{\mathrm d\ln q}}_{\theta(q)}
+\sigma_{\mathrm{in}}-1\right]
\frac{\partial\ln q}{\partial\ln p_i}.
$$

利用（1.10）及 $`\sigma_{\mathrm{in}}-1=1/\beta`$：

$$
\boxed{
\frac{\partial\ln x_i}{\partial\ln p_i}
=-\left(1+\frac1\beta\right)
+\left[\frac1\beta+\theta(q)\right]w_i.
}
\tag{B}
$$

对称均衡时 $`w_i=1/n`$，即

$$
\frac{\partial\ln x_i}{\partial\ln p_i}
=-\left(1+\frac1\beta\right)
+\frac1n\left[\frac1\beta+\theta(q)\right].
$$

所以（1.11）是 $`n`$ 大、$`w_i`$ 很小情形的近似，并非有限 $`n`$ 的精确自身价格弹性。

作为附带结果，对 $`j\ne i`$：

$$
\boxed{
\frac{\partial\ln x_i}{\partial\ln p_j}
=\left[\frac1\beta+\theta(q)\right]w_j.
}
\tag{C}
$$

若 $`1/\beta+\theta(q)>0`$，另一品种提价会提高本品种需求，即**总需求意义上的交叉价格效应为正**。这也揭示了（1.15）的另一个经济学含义。

## 4. （1.12）对称市场中的复合数量和价格

假设所有差异化品种数量相等、价格相等：

$$
x_1=\cdots=x_n=x,\qquad
p_1=\cdots=p_n=p.
$$

组内数量指数：

$$
\begin{aligned}
y
&=\left(\sum_{i=1}^n x^\rho\right)^{1/\rho}\\
&=(nx^\rho)^{1/\rho}
=xn^{1/\rho}.
\end{aligned}
$$

由于

$$
\frac1\rho=1+\beta,
$$

因此

$$
\boxed{y=x\,n^{1/\rho}=x\,n^{1+\beta}}.
$$

价格指数：

$$
\begin{aligned}
q
&=\left(\sum_{i=1}^{n}p^{-1/\beta}\right)^{-\beta}\\
&=(np^{-1/\beta})^{-\beta}
=p\,n^{-\beta}.
\end{aligned}
$$

所以教材（1.12）为

$$
\boxed{
y=x\,n^{1/\rho}=x\,n^{1+\beta},
\qquad
q=p\,n^{-(1-\rho)/\rho}=p\,n^{-\beta}.
}
\tag{1.12}
$$

$`y/x=n^{1/\rho}`$ 可体现种类多样性对 CES 综合数量的影响；$`q/p=n^{-\beta}`$ 是同一效用规范化下的多样性对应的复合价格指数效应，**并不是实际单件商品突然打折**。

## 5. （1.13）对称市场中的单品种需求

由 P9（1.7）

$$
y=\frac{I\,s(q)}q.
$$

再由（1.12）$`x=yn^{-1/\rho}`$ 和 $`q=pn^{-\beta}`$：

$$
\begin{aligned}
x
&=\frac{I s(q)}{pn^{-\beta}}\cdot n^{-1/\rho}\\
&=\frac{I s(q)}p\,n^{\beta-1/\rho}.
\end{aligned}
$$

由于 $`1/\rho=1+\beta`$，有 $`\beta-1/\rho=-1`$，从而

$$
\boxed{
x=\frac{I s(q)}{pn},
\qquad q=pn^{-\beta}.
}
\tag{1.13}
$$

也可由对称预算分配直接验证：

$$
npx=Is(q)\quad\Longrightarrow\quad x=\frac{I s(q)}{np}.
$$

这里的 $`x`$ 指 **所有企业同价同量的对称状态下每一家企业的需求量**。

## 6. （1.14）DD 曲线：所有企业同时变价

DD 曲线将 $`n`$ 和名义收入 $`I`$ 固定，所有企业的价格 $`p`$ **同步变化**（沿对称状态比较）。

从（1.13）：

$$
\ln x=\ln I+\ln s(q)-\ln p-\ln n.
$$

对共同价格 $`\ln p`$ 求导，且

$$
q=pn^{-\beta}
\quad\Longrightarrow\quad
\frac{\mathrm d\ln q}{\mathrm d\ln p}=1.
$$

因此

$$
\begin{aligned}
\frac{\mathrm d\ln x}{\mathrm d\ln p}
&=\frac{\mathrm d\ln s(q)}{\mathrm d\ln q}
\frac{\mathrm d\ln q}{\mathrm d\ln p}-1\\
&=\theta(q)-1.
\end{aligned}
$$

得到：

$$
\boxed{
\left.\frac{\mathrm d\ln x}{\mathrm d\ln p}\right|_{\mathrm{DD}}
=-[1-\theta(q)].
}
\tag{1.14}
$$

**记号核对**：截图（1.14）的分母为 $`\partial\ln p_i`$，但这里的计算是**同时调整全部价格**，严格写法应对**共同价格** $`p`$ 作总导数 $`\mathrm d\ln p`$。单个企业价格的偏导应使用上一节的公式（B）。

由 P9（1.8）：

$$
\theta(q)=[1-\sigma_{\mathrm{out}}(q)][1-s(q)].
$$

因此：

$$
\begin{aligned}
1-\theta(q)
&=1-[1-\sigma_{\mathrm{out}}(q)][1-s(q)]\\
&=s(q)+\sigma_{\mathrm{out}}(q)[1-s(q)].
\end{aligned}
$$

在内点 $`0<s(q)<1`$ 且 $`\sigma_{\mathrm{out}}(q)>0`$ 时，$`1-\theta(q)>0`$，所以 DD 需求曲线向下倾斜。注意这里的 $`\sigma_{\mathrm{out}}`$ 是**外层部门之间**的替代弹性，与内层的 $`\sigma_{\mathrm{in}}`$ 是不同对象。

## 7. （1.15）比较 dd 与 DD 的弹性

由（1.11）的近似与（1.14）：

$$
\varepsilon_{\mathrm{dd}}\simeq-\left(1+\frac1\beta\right),
\qquad
\varepsilon_{\mathrm{DD}}=-[1-\theta(q)].
$$

在两者均向下倾斜时，需求越有弹性，负的价格弹性的**绝对值**越大。

如果 **dd 的需求弹性绝对值大于 DD**，则：

$$
\begin{aligned}
|\varepsilon_{\mathrm{dd}}|>|\varepsilon_{\mathrm{DD}}|
&\iff 1+\frac1\beta>1-\theta(q)\\
&\iff\boxed{\frac1\beta+\theta(q)>0}.
\end{aligned}
$$

即原书公式：

$$
\boxed{\frac1\beta+\theta(q)>0.}
\tag{1.15}
$$

**重要纠错**：图片的原文在（1.15）前称之为“**DD 曲线更具有弹性**”的条件，但是该不等式实际表示 **dd 比 DD 更有弹性**，方向恰好相反。若反过来要求 DD 更有弹性，应为 $`1/\beta+\theta(q)<0`$。这里保留原书（1.15）数式并明确这一文字与数式的冲突。

同一条件也能从有限 $`n`$ 的交叉价格弹性（C）得到：如果 $`1/\beta+\theta(q)>0`$，价格较高的竞争品种会将需求转移到本品种。

### 极简例子

外层 Cobb–Douglas 时 $`s(q)=\alpha`$、$`\theta(q)=0`$，若 $`\beta=1`$：

$$
\varepsilon_{\mathrm{dd}}\simeq-2,\qquad
\varepsilon_{\mathrm{DD}}=-1.
$$

于是（1.15）显然满足：$`1/\beta+\theta=1>0`$，但 **dd 是更有弹性的曲线**。

## 8. （1.16）任意两种商品间的相对需求

由条件需求（1.9），对于 $`i\ne j`$：

$$
x_i=y(q/p_i)^{\sigma_{\mathrm{in}}},
\qquad
x_j=y(q/p_j)^{\sigma_{\mathrm{in}}}.
$$

两式相除，公共的 $`y`$ 和 $`q`$ 完全抵消：

$$
\begin{aligned}
\frac{x_i}{x_j}
&=\frac{(q/p_i)^{\sigma_{\mathrm{in}}}}{(q/p_j)^{\sigma_{\mathrm{in}}}}\\
&=\left(\frac{p_j}{p_i}\right)^{\sigma_{\mathrm{in}}}.
\end{aligned}
$$

得到书中：

$$
\boxed{
\frac{x_i}{x_j}
=\left(\frac{p_j}{p_i}\right)^{1/(1-\rho)}.
}
\tag{1.16}
$$

两边取对数：

$$
\ln(x_i/x_j)
=-\sigma_{\mathrm{in}}\ln(p_i/p_j).
$$

因此：

$$
\boxed{
-\frac{\mathrm d\ln(x_i/x_j)}
{\mathrm d\ln(p_i/p_j)}
=\sigma_{\mathrm{in}}
=\frac1{1-\rho}.
}
$$

这里对相对价格作变动，并保持其它必要的相对价格或最优配置约束一致；指数给出 CES 聚合器**组内任意两个品种的恒定替代弹性**，并不依赖外层支出份额函数 $`s(q)`$。

## 9. 一致性核查：局部和整体价格变化为何不同？

完整非条件需求是

$$
x_i=I s(q) q^{1/\beta}p_i^{-(1+1/\beta)}.
$$

对于任意 $`j`$，其价格对 $`x_i`$ 的对数偏导：

$$
\frac{\partial\ln x_i}{\partial\ln p_j}
=\left(\frac1\beta+\theta(q)\right)w_j
-\left(1+\frac1\beta\right)\mathbf{1}\{i=j\}.
$$

其中 $`w_j`$ 是第 $`j`$ 个品种的部门内支出份额，$`\sum_j w_j=1`$。

若把**全部** $`p_j`$ 同时提高同一微小比例，则对数弹性之和是

$$
\begin{aligned}
\sum_{j=1}^{n}\frac{\partial\ln x_i}{\partial\ln p_j}
&=\left(\frac1\beta+\theta(q)\right)\sum_j w_j
-\left(1+\frac1\beta\right)\\
&=\theta(q)-1.
\end{aligned}
$$

这正是（1.14）：**DD 弹性等于所有价格方向上偏导数的总和，不等于其中任意一个单独偏导数**。这是理解 dd / DD 两曲线最有用的数学关系。

## 10. 数值自检（可手算）

令 $`n=100`$、$`\rho=1/2`$、$`\beta=1`$、所有 $`p_i=2`$，外层 Cobb–Douglas，$`s(q)=1/2`$、$`\theta(q)=0`$，名义收入 $`I=100`$。

由（1.12）：

$$
q=2\times100^{-1}=0.02.
$$

由（1.13）：

$$
x=\frac{100\times0.5}{2\times100}=0.25.
$$

由（1.12）：

$$
y=x\,100^2=2500.
$$

代回正确的（1.9）：

$$
y(q/p)^2=2500(0.02/2)^2=0.25=x.
$$

校验组内预算：

$$
np\,x=100\times2\times0.25=50=Is(q)=q y.
$$

最后：

$$
\varepsilon_{\mathrm{dd}}\simeq-2,\quad
\varepsilon_{\mathrm{dd,finite}}=-2+\frac1{100}=-1.99,\quad
\varepsilon_{\mathrm{DD}}=-1.
$$

可以直观看出大 $`n`$ 近似、有限 $`n`$ 修正和共同价格变动之间的区别。

## 11. 原书八个公式速查表

| 公式 | 关键结果 | 关键步骤或适用范围 |
| :--- | :--- | :--- |
| （1.9） | $`x_i=y(q/p_i)^{1/(1-\rho)}`$ | 组内 CES 成本最小化；原书图片疑似漏写 $`y`$ |
| （1.10） | $`\partial\ln q/\partial\ln p_i=(q/p_i)^{1/\beta}`$ | 对价格指数取对数微分，等于组内支出份额 |
| （1.11） | $`\varepsilon_{\mathrm{dd}}\simeq-(1+\beta)/\beta`$ | 单一品种独立提价，忽略小份额品种对 $`q,s`$ 的反馈 |
| （1.12） | $`y=xn^{1+\beta},\quad q=pn^{-\beta}`$ | 对称状态：各品种价格和数量相同 |
| （1.13） | $`x=Is(q)/(pn)`$ | 对称市场的部门支出除以品种数和价格 |
| （1.14） | $`\varepsilon_{\mathrm{DD}}=-[1-\theta(q)]`$ | **所有**企业的价格共同变化，固定 $`n,I`$ |
| （1.15） | $`1/\beta+\theta(q)>0`$ | 表示近似 dd 的弹性绝对值**大于** DD，而不是反过来 |
| （1.16） | $`x_i/x_j=(p_j/p_i)^{1/(1-\rho)}`$ | 条件品种需求相除，读出组内替代弹性 |

### 进一步阅读

- [P5：公式（1.1）CES 价格指数](ces-price-index-equation-1-1.md)
- [P6：公式（1.2）CES 数量和收入需求](ces-demand-revenue-equation-1-2.md)
- [P9：公式（1.4）—（1.8）嵌套 CES 与支出份额弹性](two-stage-budgeting-equations-1-4-to-1-8-p9.md)

---

**本节教材来源**：刘文革, 裴莹. (2026). *国际贸易应用模型* (第1版). 清华大学出版社. 第 10 页，公式（1.9）—（1.16）。

**使用说明**：本笔记依照读者拍摄的 P10 原书页面撰写。对（1.9）、（1.11）、（1.14）的疑似排印/记号问题以及（1.15）相关文字的方向冲突进行了**数学核对并明确标注**；尚未与其它书籍版本核对，因此不把这些问题断言为已确认的正式勘误。
