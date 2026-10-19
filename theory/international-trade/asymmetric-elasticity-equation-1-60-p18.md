# 《国际贸易应用模型》P18：公式（1.60）——均衡综合价格指数对替代弹性参数的导数

> **教材**：刘文革、裴莹编著，《国际贸易应用模型》，清华大学出版社，2026 年 6 月第 1 版，ISBN 978-7-302-71633-4。  
> **章节**：第一章第三节“三、非对称情形”，P18，公式（1.60）。  
> **上一篇**：[P17 进入约束与最优角点（1.56）—（1.59）](asymmetric-entry-and-optimum-equations-1-56-to-1-59-p17.md)；[P16 两组候选均衡（1.54）—（1.55b）](asymmetric-two-groups-equations-1-54-to-1-55b-p16.md)。

## 1. 原书结论与问题

书中给出：

$$
\boxed{
\frac{\partial\ln\bar q_i}{\partial\beta_i}
=-\ln\bar n_i.
}
\tag{1.60}
$$

其中 $`i\in\{1,2\}`$ 表示两种候选商品组的任意一组，带横杠表示**只有该组生产时的候选对称均衡值**。

| 符号 | 含义 |
| :--- | :--- |
| $`\beta_i=(1-\rho_i)/\rho_i>0`$ | 组内 CES 参数 |
| $`\sigma_i=(1+\beta_i)/\beta_i=1+1/\beta_i`$ | 组内任意两个品种的替代弹性 |
| $`a_i>0`$ | 单家企业固定成本 |
| $`c_i>0`$ | 单位产出边际成本 |
| $`0<s<1`$ | 外层 Cobb–Douglas 对差异化商品部门的支出份额 |
| $`\bar p_i`$ | 只有组 $`i`$ 存在时的候选均衡单品种价格 |
| $`\bar n_i`$ | 对应候选均衡的企业数量（连续近似） |
| $`\bar q_i=\bar p_i\bar n_i^{-\beta_i}`$ | 组内 CES 复合商品的候选均衡价格指数 |

必须区分：公式（1.60）的左边对 $`\beta_i`$ 的微分，**保持 $`a_i,c_i,s`$ 固定，但允许均衡价格 $`\bar p_i`$ 和均衡品种数 $`\bar n_i`$ 随 $`\beta_i`$ 改变**。

## 2. 从（1.55a/b）取出三个关键等式

P16 对任一组 $`i`$，都已经推导出：

$$
\boxed{\bar p_i=c_i(1+\beta_i),}
\tag{A}
$$

$$
\boxed{\bar n_i=\frac{s\beta_i}{a_i(1+\beta_i)},}
\tag{B}
$$

$$
\boxed{
\bar q_i=\bar p_i\bar n_i^{-\beta_i}
=c_i(1+\beta_i)^{1+\beta_i}
\left(\frac{a_i}{s\beta_i}\right)^{\beta_i}.
}
\tag{C}
$$

下面两种方法都可以独立推出（1.60）。

## 3. 方法一：直接对显式价格指数求对数导数

由（C）：

$$
\bar q_i=c_i(1+\beta_i)^{1+\beta_i}
\left(\frac{a_i}{s\beta_i}\right)^{\beta_i}.
$$

取自然对数：

$$
\ln\bar q_i
=\ln c_i
+(1+\beta_i)\ln(1+\beta_i)
+\beta_i\ln\left(\frac{a_i}{s\beta_i}\right).
$$

逐项对 $`\beta_i`$ 求导：

第一项因 $`c_i`$ 固定而为零：

$$
\frac{\partial\ln c_i}{\partial\beta_i}=0.
$$

第二项利用乘积求导：

$$
\frac{\mathrm d}{\mathrm d\beta_i}
\left[(1+\beta_i)\ln(1+\beta_i)\right]
=\ln(1+\beta_i)+1.
$$

第三项利用乘积与链式法则：

$$
\begin{aligned}
\frac{\mathrm d}{\mathrm d\beta_i}
\left[\beta_i\ln\left(\frac{a_i}{s\beta_i}\right)\right]
&=\ln\left(\frac{a_i}{s\beta_i}\right)
+\beta_i\left(-\frac1{\beta_i}\right)\\
&=\ln\left(\frac{a_i}{s\beta_i}\right)-1.
\end{aligned}
$$

相加，其中常数 $`+1`$ 和 $`-1`$ **完全抵消**：

$$
\begin{aligned}
\frac{\partial\ln\bar q_i}{\partial\beta_i}
&=\ln(1+\beta_i)
+\ln\left(\frac{a_i}{s\beta_i}\right)\\
&=\ln\left(\frac{a_i(1+\beta_i)}{s\beta_i}\right)\\
&=-\ln\left(\frac{s\beta_i}{a_i(1+\beta_i)}\right).
\end{aligned}
$$

由（B）中 $`\bar n_i=s\beta_i/[a_i(1+\beta_i)]`$：

$$
\boxed{
\frac{\partial\ln\bar q_i}{\partial\beta_i}
=-\ln\bar n_i.
}
\tag{1.60}
$$

## 4. 方法二：从 $`\bar q_i=\bar p_i\bar n_i^{-\beta_i}`$ 出发

取对数：

$$
\ln\bar q_i=\ln\bar p_i-\beta_i\ln\bar n_i.
$$

对 $`\beta_i`$ 求导时，**价格与企业数都不是常数**，因此：

$$
\boxed{
\frac{\partial\ln\bar q_i}{\partial\beta_i}
=
\frac{\partial\ln\bar p_i}{\partial\beta_i}
-\ln\bar n_i
-\beta_i\frac{\partial\ln\bar n_i}{\partial\beta_i}.
}
\tag{D}
$$

首先由（A）：

$$
\bar p_i=c_i(1+\beta_i)
\quad\Longrightarrow\quad
\boxed{\frac{\partial\ln\bar p_i}{\partial\beta_i}
=\frac1{1+\beta_i}.}
$$

然后由（B）：

$$
\ln\bar n_i
=\ln s+\ln\beta_i-\ln a_i-\ln(1+\beta_i),
$$

所以：

$$
\boxed{
\frac{\partial\ln\bar n_i}{\partial\beta_i}
=\frac1{\beta_i}-\frac1{1+\beta_i}
=\frac1{\beta_i(1+\beta_i)}.
}
$$

代回（D）：

$$
\begin{aligned}
\frac{\partial\ln\bar q_i}{\partial\beta_i}
&=\frac1{1+\beta_i}
-\ln\bar n_i
-\beta_i\frac1{\beta_i(1+\beta_i)}\\
&=\frac1{1+\beta_i}
-\ln\bar n_i
-\frac1{1+\beta_i}\\
&=\boxed{-\ln\bar n_i}.
\end{aligned}
$$

**核心观察**：$`\beta_i`$ 上升会使单品种的加成售价上升，同时也使候选均衡企业数量上升；两者对 $`\ln\bar q_i`$ 的相应影响在求导后恰好抵消，最后剩下**CES 品种数幂指数自身改变**的影响。

## 5. 如何理解（1.60）的正负号？

注意：

$$
\bar n_i=\frac{s\beta_i}{a_i(1+\beta_i)}.
$$

如果 **$`\bar n_i>1`$**：

$$
\ln\bar n_i>0
\quad\Longrightarrow\quad
\frac{\partial\ln\bar q_i}{\partial\beta_i}<0.
$$

即 $`\beta_i`$ 增大，均衡综合价格指数降低。

若 $`\bar n_i=1`$，该导数为 0；若连续近似给出 $`0<\bar n_i<1`$，导数反而为正。但“少于一家企业”的候选数量在离散企业数模型中没有直接字面意义，因此应谨慎解释这一数学区域。

### 替代弹性 $`\sigma_i`$ 与 $`\beta_i`$ 方向相反

由：

$$
\boxed{\sigma_i=1+\frac1{\beta_i},}
$$

有：

$$
\frac{\mathrm d\sigma_i}{\mathrm d\beta_i}
=-\frac1{\beta_i^2}<0.
$$

所以 **$`\beta_i`$ 越大，组内品种间替代弹性 $`\sigma_i`$ 反而越小**。

在 $`\bar n_i>1`$ 的区域中，$`\beta_i`$ 上升意味着品种间变得更不容易替代（差异化更强），品种多样性效应更大，并伴随更低的复合价格指数。

若直接对真正的替代弹性求导：

$$
\frac{\mathrm d\beta_i}{\mathrm d\sigma_i}=-\beta_i^2,
$$

故：

$$
\boxed{
\frac{\partial\ln\bar q_i}{\partial\sigma_i}
=\beta_i^2\ln\bar n_i>0
\quad\text{当 }\bar n_i>1.
}
\tag{E}
$$

这意味着在这些条件下，品种间替代弹性**越高**，均衡综合价格指数**越高**；与书页文字关于“$`\beta`$ 高而自有价格弹性低”的解释一致。

## 6. 手算与符号检验

取：

$$
s=\frac12,\quad a_i=0.02,\quad c_i=2,\quad \beta_i=1.
$$

根据候选均衡表达式：

$$
\bar p_i=2(1+1)=4,
$$

$$
\bar n_i=\frac{0.5\times1}{0.02(1+1)}=12.5,
$$

$$
\bar q_i=\bar p_i\bar n_i^{-1}=\frac4{12.5}=0.32.
$$

由（1.60）：

$$
\left.\frac{\partial\ln\bar q_i}{\partial\beta_i}\right|_{\beta_i=1}
=-\ln12.5\approx-2.52573.
$$

在经济模型中把企业数连续化只是为求解析结果，数值示例得到非整数 $`12.5`$ 不意味着真实存在半家企业。

进一步的解析校验：$`\bar n_i=s\beta_i/[a_i(1+\beta_i)]`$，故

$$
\frac{\partial\ln\bar n_i}{\partial\beta_i}
=\frac1{\beta_i(1+\beta_i)},
$$

与方法二里的价格、数量调整完全一致。

## 7. 本页推导核心要点

- **基础价格**：$`\bar p_i=c_i(1+\beta_i)`$。
- **候选企业数**：$`\bar n_i=s\beta_i/[a_i(1+\beta_i)]`$。
- **综合价格指数**：$`\bar q_i=\bar p_i\bar n_i^{-\beta_i}`$。
- **链式求导**：$`\partial\ln\bar q_i/\partial\beta_i=-\ln\bar n_i`$。
- **经济解释**：该式表示综合价格指数对 CES 参数的**均衡总响应**，不是把 $`\bar p_i,\bar n_i`$ 机械固定所做的偏导。
- **使用边界**：默认 $`a_i,c_i,s`$ 不变、候选单组均衡条件有效，且采用连续品种数与大 $`n`$ 定价近似。

后面的 P18 正文用（1.60）讨论替代弹性差异、生产成本差异以及两种单组候选均衡的进入可行性。文字中的区域 A—G 对应书中图 1.2；图形比较不是新的公式，本篇只整理到（1.60）。

---

**教材引用**：刘文革, 裴莹. (2026). *国际贸易应用模型* (第1版). 清华大学出版社. 第 18 页，公式（1.60）。
