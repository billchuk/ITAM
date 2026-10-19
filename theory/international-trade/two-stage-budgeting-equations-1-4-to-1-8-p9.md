# 《国际贸易应用模型》P9：公式（1.4）—（1.8）逐步推导

> **位置**：第 9 页（P9），“第三节 模型设定与推导——一、固定弹性的情形——（一）需求函数”。  
> **主题**：嵌套效用、组内 CES 价格指数、两阶段预算分配、部门间替代弹性和支出份额弹性。  
> **资料依据**：读者提供的原书 P9 图片；完整作者、书名版本与出版信息待补。  
> **先修**：[P5：CES 价格指数（1.1）](ces-price-index-equation-1-1.md)；[P6：CES 数量与收入需求（1.2）](ces-demand-revenue-equation-1-2.md)。

## 0. 研究问题与必要说明

这一页建立一个**双层（nested）消费模型**：

- **外层**：消费者在同质商品 $x_0$ 与差异化商品复合数量 $Y$ 之间作选择；
- **内层**：给定 $Y$，消费者在 $n$ 个差异化商品品种 $x_1,\ldots,x_n$ 之间寻找成本最低的组合。

通过**组内成本最小化**得到 $q$，再通过**组间效用最大化**得到支出分配 $s(q)$。

### 图片中需要留意的排印/记号问题

1. 原书的式（1.5）在 $\sum_{i=1}^{n}p_ix_i$ 后又出现一个孤立的 $\sum$。这个求和符号没有上下标和被求和对象，按经济学预算约束应写成 $x_0+\sum_{i=1}^{n}p_ix_i=I$。
2. 式（1.7）和（1.8）出现了小写 $s(q)$ 与大写 $S(q)$ 混用。因原书文字将 $s$ 定义为支出份额函数，**本文统一为小写 $s(q)$**。
3. 式（1.6）中的 $Y$ 与式（1.7）中的 $y$ 表示相同的复合商品数量，下文统一写作 $Y$。
4. **重要模型条件**：仅有“无差异曲面凸”以及组内 CES，并**不能**推出 $s$ 只依赖于 $q$，也不足以让（1.8）中的 $\sigma(q)$ 直接解释成通常的 Hicks/Allen 部门间替代弹性。要获得教材的简洁表达，可进一步要求**外层偏好 $U(x_0,Y)$ 是位似（homothetic）的**，且讨论内点解；或将 $\sigma(q)$ 明确定义为固定收入条件下的相对需求弹性，而不是不加说明地等同于补偿替代弹性。

## 1. 效用函数：式（1.4）

原书设定：

$$
\boxed{
u=U\left[x_0,\left(\sum_{i=1}^{n}x_i^\rho\right)^{1/\rho}\right],
\qquad 0<\rho<1.
}
\tag{1.4}
$$

定义差异化商品的 CES 复合数量：

$$
\boxed{
Y\equiv \left(\sum_{i=1}^{n}x_i^\rho\right)^{1/\rho}.
}
$$

效用函数于是可以写成：

$$
u=U(x_0,Y).
$$

| 记号 | 经济含义 |
| :--- | :--- |
| $x_0$ | 同质商品消费量，其价格被规范化为 1 |
| $x_i$ | 第 $i$ 种差异化商品的消费量 |
| $p_i>0$ | 差异化商品 $i$ 的价格 |
| $I$ | 消费者名义收入（消费预算） |
| $Y$ | 差异化商品的 CES 复合数量 |
| $q>0$ | 购买一单位 $Y$ 的**最小成本**，即组内 CES 价格指数 |
| $\rho\in(0,1)$ | 组内 CES 幂参数 |
| $\beta=(1-\rho)/\rho>0$ | 原书为转换价格指数而定义的参数 |
| $s(q)\in[0,1]$ | 差异化商品部门占名义收入的支出份额 |
| $\sigma_{\mathrm{out}}(q)$ | 外层 $x_0$ 与 $Y$ 之间的替代弹性，不等于组内品种间弹性 |
| $\theta(q)$ | 支出份额 $s(q)$ 对 $q$ 的对数弹性 |

组内替代弹性记为：

$$
\boxed{\sigma_{\mathrm{in}}=\frac{1}{1-\rho}>1.}
$$

**注意符号冲突**：之前公式（1.1）—（1.2）中的 $\sigma$ 是**品种之间**的替代弹性；本页（1.8）的 $\sigma(q)$ 指**两个部门/两种复合商品之间**的替代弹性。两个层级不可混淆。

## 2. 预算约束：式（1.5）

因 $x_0$ 的单价为 1，而第 $i$ 种差异化商品价格为 $p_i$，总预算为：

$$
\boxed{x_0+\sum_{i=1}^{n}p_ix_i=I.}
\tag{1.5}
$$

记差异化商品实际支出 $E_D=\sum_i p_ix_i$，故：

$$
x_0+E_D=I.
$$

下文将证明在组内达到最优组合时 $E_D=qY$，从而把多品种预算约束化为只有两个对象的预算约束：

$$
\boxed{x_0+qY=I.}
\tag{B}
$$

## 3. 组内成本最小化：推导式（1.6）的价格指数

### 3.1 优化问题

对任意给定的目标综合数量 $\bar Y>0$，选择 $\{x_i\}$ 使支出最小：

$$
\begin{aligned}
\min_{\{x_i\ge0\}}\quad &E_D=\sum_{i=1}^n p_ix_i,\\
\text{s.t.}\quad&\sum_{i=1}^{n}x_i^\rho=\bar Y^\rho.
\end{aligned}
$$

构造拉格朗日函数：

$$
\mathcal L
=\sum_{i=1}^n p_ix_i+
\lambda\left(\bar Y^\rho-\sum_{i=1}^n x_i^\rho\right).
$$

对任意内点 $x_i>0$，一阶条件为：

$$
\frac{\partial\mathcal L}{\partial x_i}
=p_i-\lambda\rho x_i^{\rho-1}=0.
$$

因此：

$$
p_i=\lambda\rho\,x_i^{\rho-1}.
$$

### 3.2 解出条件品种需求

$$
x_i
=\left(\frac{p_i}{\lambda\rho}\right)^{1/(\rho-1)}.
$$

定义 $\sigma_{\mathrm{in}}=1/(1-\rho)$，有：

$$
\frac{1}{\rho-1}=-\sigma_{\mathrm{in}}.
$$

令 $A=(\lambda\rho)^{\sigma_{\mathrm{in}}}$，从而：

$$
\boxed{x_i=A\,p_i^{-\sigma_{\mathrm{in}}}.}
\tag{C}
$$

定义正参数：

$$
\boxed{\beta\equiv\frac{1-\rho}{\rho}>0.}
$$

则：

$$
\sigma_{\mathrm{in}}
=\frac{1}{1-\rho}
=1+\frac{\rho}{1-\rho}
=1+\frac1\beta,
$$

以及：

$$
1-\sigma_{\mathrm{in}}=-\frac1\beta.
$$

所以式 (C) 还可写为：

$$
x_i=A\,p_i^{-(1+1/\beta)}.
$$

### 3.3 分别计算综合数量和最小支出

将式 (C) 代入 $Y$：

$$
\begin{aligned}
Y
&=\left(\sum_i (A p_i^{-\sigma_{\mathrm{in}}})^\rho\right)^{1/\rho}\\
&=A\left(\sum_i p_i^{-\sigma_{\mathrm{in}}\rho}\right)^{1/\rho}.
\end{aligned}
$$

由于：

$$
-\sigma_{\mathrm{in}}\rho
=-\frac{\rho}{1-\rho}
=-\frac1\beta,
$$

得到：

$$
\boxed{
Y=A\left(\sum_i p_i^{-1/\beta}\right)^{1/\rho}.
}
\tag{D}
$$

总支出则为：

$$
\begin{aligned}
E_D
&=\sum_i p_i x_i\\
&=A\sum_i p_i^{1-\sigma_{\mathrm{in}}}\\
&=A\sum_i p_i^{-1/\beta}.
\end{aligned}
$$

因此：

$$
\boxed{E_D=A\sum_i p_i^{-1/\beta}.}
\tag{E}
$$

### 3.4 计算单位综合数量的最低成本

定义 $q$ 为 $E_D/Y$：

$$
\begin{aligned}
q
=\frac{E_D}{Y}
&=\frac{A\sum_i p_i^{-1/\beta}}
{A\left(\sum_i p_i^{-1/\beta}\right)^{1/\rho}}\\
&=\left(\sum_i p_i^{-1/\beta}\right)^{1-1/\rho}.
\end{aligned}
$$

利用：

$$
1-\frac1\rho=-\frac{1-\rho}{\rho}=-\beta,
$$

于是：

$$
\boxed{
q=\left(\sum_{i=1}^{n}p_i^{-1/\beta}\right)^{-\beta}.
}
$$

连同 $Y$ 的定义，正好是原书式（1.6）：

$$
\boxed{
Y=\left(\sum_{i=1}^{n}x_i^\rho\right)^{1/\rho},
\qquad
q=\left(\sum_{i=1}^{n}p_i^{-1/\beta}\right)^{-\beta}.
}
\tag{1.6}
$$

因此在组内最优配置下**严格有**：

$$
E_D=qY.
$$

对应的各品种条件需求可以进一步写成：

$$
\boxed{
x_i=Y\left(\frac{p_i}{q}\right)^{-\sigma_{\mathrm{in}}}.
}
\tag{F}
$$

**核对前文**：本页的 $q$ 相当于公式（1.1）中的综合价格指数 $P$，而本页的 $Y$ 相当于此前的综合数量 $Q$；只是此处改为有限个品种的求和形式。

## 4. 组间效用最大化：推导式（1.7）

有了 $E_D=qY$，原先 $n+1$ 种商品的预算约束变成：

$$
x_0+qY=I.
$$

消费者现在选择 $x_0$ 与 $Y$：

$$
\max_{x_0,Y\ge0} U(x_0,Y)
\quad\text{s.t.}\quad x_0+qY=I.
$$

对应拉格朗日函数：

$$
\mathcal L=U(x_0,Y)+\mu(I-x_0-qY).
$$

对**内点最优解**，一阶条件：

$$
U_{x_0}=\mu,\qquad U_Y=\mu q.
$$

故：

$$
\boxed{\frac{U_Y}{U_{x_0}}=q.}
\tag{G}
$$

这表示在最优配置时，差异化复合商品与同质商品的**边际替代率**等于相对价格 $q$。

定义差异化商品部门的支出份额：

$$
\boxed{s(q,I)\equiv\frac{qY(q,I)}{I}.}
\tag{H}
$$

那么仅从预算约束与份额定义就能得到：

$$
Y(q,I)=\frac{I\,s(q,I)}{q},
\qquad
x_0(q,I)=I[1-s(q,I)].
$$

**什么时候可以把 $s(q,I)$ 缩写为 $s(q)$？**

一个充分且标准的条件是：**外层效用 $U(x_0,Y)$ 表示位似偏好（homothetic preferences）**。例如外层为 Cobb–Douglas 或 CES 效用。此时在固定相对价格 $q$ 时，最优的 $Y/x_0$ 不随 $I$ 改变，因此支出份额也不随收入改变。

在这一条件下，$s(q,I)=s(q)$，得到：

$$
\boxed{
Y=I\frac{s(q)}{q},
\qquad
x_0=I[1-s(q)].
}
\tag{1.7}
$$

这就是式（1.7）。其中 $0<s(q)<1$ 表示两部门均消费的内点情况。

> **逻辑区别**：式（1.7）的代数分配关系来自**支出份额的定义**；要进一步声明“支出份额仅是 $q$ 的函数”，则还需外层偏好方面的假设，不能仅从式（1.4）中 CES 的**内层**结构推出。

## 5. 支出份额弹性：逐步推导式（1.8）

目标是解释：

$$
\boxed{
\theta(q)=[1-\sigma(q)]\,[1-s(q)]<1.
}
\tag{1.8}
$$

为避免与组内 $\sigma_{\mathrm{in}}$ 混淆，这里先将原书的 $\sigma(q)$ 记为 $\sigma_{\mathrm{out}}(q)$。

### 5.1 定义部门间的相对消费比例与替代弹性

设：

$$
t(q)\equiv\frac{Y}{x_0}.
$$

在外层偏好位似、内点解、同质商品价格为 1 的条件下，最优消费比例 $t$ 只随相对价格 $q$ 变化。

定义两部门间的**替代弹性**为：

$$
\boxed{
\sigma_{\mathrm{out}}(q)
\equiv-\frac{\mathrm d\ln(Y/x_0)}{\mathrm d\ln q}
=-\frac{\mathrm d\ln t(q)}{\mathrm d\ln q}.
}
\tag{J}
$$

这里负号表示相对价格上升时相对需求通常下降。对位似偏好，沿最优需求关系求出的该弹性与标准的等效用曲线替代弹性一致。

### 5.2 用支出份额表示相对需求比例

从式（1.7）：

$$
Y=\frac{Is(q)}q,\qquad x_0=I[1-s(q)].
$$

两式相除：

$$
\frac{Y}{x_0}
=\frac{s(q)}{q[1-s(q)]}.
$$

所以：

$$
\boxed{
\frac{s(q)}{1-s(q)}=q\,\frac{Y}{x_0}.
}
\tag{K}
$$

等式左侧是“差异化商品部门支出”与“同质商品部门支出”的比值（支出赔率），右侧是相对价格乘相对数量。

### 5.3 两边取对数并对 $\ln q$ 求导

对式 (K) 两边取对数：

$$
\ln s(q)-\ln[1-s(q)]
=\ln q+\ln\left(\frac{Y}{x_0}\right).
$$

两边对 $\ln q$ 求导，右侧是：

$$
\frac{\mathrm d}{\mathrm d\ln q}
\left[\ln q+\ln\left(\frac{Y}{x_0}\right)\right]
=1-\sigma_{\mathrm{out}}(q).
$$

左侧注意链式法则：

$$
\begin{aligned}
\frac{\mathrm d}{\mathrm d\ln q}
\{\ln s(q)-\ln[1-s(q)]\}
&=\left[\frac1{s(q)}+\frac1{1-s(q)}\right]
\frac{\mathrm d s(q)}{\mathrm d\ln q}\\[4pt]
&=\frac{q\,s'(q)}{s(q)[1-s(q)]}.
\end{aligned}
$$

因此：

$$
\boxed{
\frac{q\,s'(q)}{s(q)[1-s(q)]}
=1-\sigma_{\mathrm{out}}(q).
}
\tag{L}
$$

### 5.4 定义 $s(q)$ 的价格弹性

原书将 $\theta$ 定义为：

$$
\boxed{
\theta(q)\equiv\frac{q\,s'(q)}{s(q)}
=\frac{\mathrm d\ln s(q)}{\mathrm d\ln q}.
}
$$

在式 (L) 两边乘以 $1-s(q)$：

$$
\boxed{
\theta(q)=
[1-\sigma_{\mathrm{out}}(q)]\,[1-s(q)].
}
\tag{1.8}
$$

恢复原书记号 $\sigma_{\mathrm{out}}(q)=\sigma(q)$，即为：

$$
\boxed{
\theta(q)=[1-\sigma(q)][1-s(q)]<1.
}
$$

若为严格内点 $0<s(q)<1$，且替代弹性 $\sigma_{\mathrm{out}}(q)>0$，则 $1-s(q)\in(0,1)$，$1-\sigma_{\mathrm{out}}(q)<1$，所以 $\theta(q)<1$。注意 **$\theta(q)$ 不一定大于零**。

### 5.5 更一般偏好下必须如何解释？

若外层 $U(x_0,Y)$ **非位似**，最优份额通常是 $s(q,I)$ 而非 $s(q)$。固定名义收入 $I$，式 (K) 仍然成立，但是求导得到的是：

$$
\frac{\partial\ln s(q,I)}{\partial\ln q}\bigg|_I
=\left[1-\varepsilon_t^{M}(q,I)\right][1-s(q,I)],
$$

其中

$$
\varepsilon_t^{M}(q,I)
\equiv-\frac{\partial\ln[Y(q,I)/x_0(q,I)]}{\partial\ln q}\bigg|_I
$$

是**固定收入**的相对 Marshallian 需求弹性。这在一般非位似偏好下**不必等于**保持效用不变的部门间替代弹性。

因此，截图中从（1.4）直接声称“可以证明（1.8）”省略了重要假设或定义。本笔记保留原书最终形式，但清晰列出其成立的充分条件。

## 6. 经济学解释与比较静态

式（1.8）将支出份额对综合价格的反应分成两个部分：

$$
\underbrace{\theta(q)}_{\substack{\text{份额}\\\text{价格弹性}}}
=
\underbrace{[1-\sigma_{\mathrm{out}}(q)]}_{\text{部门替代程度}}
\underbrace{[1-s(q)]}_{\text{其他部门支出份额}}.
$$

在内点且 $\sigma_{\mathrm{out}}>0$ 时：

| 部门间替代弹性 | $\theta(q)$ | 经济含义 |
| :--- | :--- | :--- |
| $0<\sigma_{\mathrm{out}}<1$ | 正 | 差异化部门综合价格上涨时，名义支出份额反而上升 |
| $\sigma_{\mathrm{out}}=1$ | 零 | 支出份额不随相对价格变化（如外层 Cobb–Douglas） |
| $\sigma_{\mathrm{out}}>1$ | 负 | 差异化部门综合价格上涨时，名义支出份额下降 |

与先前的 CES 品种需求比较：**品种间替代弹性** $\sigma_{\mathrm{in}}=1/(1-\rho)>1$ 是组内性质；而这里的**部门间弹性** $\sigma_{\mathrm{out}}$ 可小于、等于或大于 1，取决于外层 $U$。

## 7. 两个可检验的例子

### 7.1 外层 Cobb–Douglas：$\theta(q)=0$

令：

$$
U(x_0,Y)=x_0^{1-\alpha}Y^\alpha,\qquad 0<\alpha<1.
$$

组间最优分配为：

$$
x_0=(1-\alpha)I,\qquad
Y=\frac{\alpha I}{q},
\qquad
s(q)=\alpha.
$$

因 Cobb–Douglas 的部门间替代弹性为 $\sigma_{\mathrm{out}}=1$：

$$
\theta(q)=\frac{qs'(q)}{s(q)}=0
=(1-1)(1-\alpha).
$$

### 7.2 外层 CES：直接验证式（1.8）

令（为区分组内 $\rho$，这里使用另一参数 $\eta>0$）：

$$
U(x_0,Y)=
\left[a\,x_0^{(\eta-1)/\eta}
+b\,Y^{(\eta-1)/\eta}\right]^{\eta/(\eta-1)},
\quad a,b>0,\quad \eta\ne1.
$$

一阶条件 $U_Y/U_{x_0}=q$ 给出：

$$
\frac{Y}{x_0}=\left(\frac{b}{a q}\right)^\eta.
$$

因此：

$$
\frac{s(q)}{1-s(q)}
=q\,\frac{Y}{x_0}
=\left(\frac ba\right)^\eta q^{1-\eta}.
$$

化为显式份额函数：

$$
\boxed{
s(q)=\frac{(b/a)^\eta q^{1-\eta}}
{1+(b/a)^\eta q^{1-\eta}}.
}
$$

取对数导数：

$$
\boxed{
\frac{\mathrm d\ln s(q)}{\mathrm d\ln q}
=(1-\eta)\,[1-s(q)].
}
$$

因为外层 CES 的替代弹性正是 $\sigma_{\mathrm{out}}=\eta$，所以与式（1.8）完全一致。

### 7.3 与式（1.6）—（1.7）一起做数值核对

令 $n=2,\rho=1/2$、$p_1=p_2=2$，则

$$
\beta=1,\qquad
q=(2^{-1}+2^{-1})^{-1}=1.
$$

令外层效用为 $U(x_0,Y)=x_0^{1/2}Y^{1/2}$、收入 $I=100$：

$$
s(q)=1/2,\qquad x_0=50,\qquad Y=50.
$$

组内 $\sigma_{\mathrm{in}}=2$，条件品种需求：

$$
x_1=x_2=Y(2/1)^{-2}=12.5.
$$

校验总预算：

$$
x_0+p_1x_1+p_2x_2
=50+2(12.5)+2(12.5)=100=I.
$$

校验复合数量：

$$
Y=(\sqrt{12.5}+\sqrt{12.5})^2=50.
$$

因此（1.4）—（1.7）内部一致，并且外层 Cobb–Douglas 给出（1.8）中的 $\theta=0$。

## 8. 五个原书公式的逻辑关系

| 编号 | 公式 | 从哪里来 |
| :--- | :--- | :--- |
| （1.4） | $u=U[x_0,(\sum_i x_i^\rho)^{1/\rho}]$ | **模型设定**：嵌套效用与组内 CES |
| （1.5） | $x_0+\sum_i p_ix_i=I$ | **预算约束**：同质商品价格规范化为 1 |
| （1.6） | $Y=(\sum_i x_i^\rho)^{1/\rho}$，$q=(\sum_i p_i^{-1/\beta})^{-\beta}$ | **定义 + 组内成本最小化** |
| （1.7） | $Y=Is(q)/q$，$x_0=I[1-s(q)]$ | **支出份额定义 + 组间最优选择**；$s$ 仅依赖于 $q$ 需额外条件 |
| （1.8） | $\theta(q)=[1-\sigma_{\mathrm{out}}(q)][1-s(q)]$ | **对支出份额赔率取对数求导**；标准替代弹性解释需外层位似等条件 |

**最值得记住的主线：**

$$
\boxed{
\text{嵌套效用}
\ \longrightarrow\
\text{组内 CES 成本最小化}
\ \longrightarrow\
q
\ \longrightarrow\
x_0+qY=I
\ \longrightarrow\
s(q)
\ \longrightarrow\
\theta(q).
}
$$

---

**扩展方向**：在固定弹性模型之外，可考察非位似上层偏好、非 CES 的组内聚合、部门间替代弹性的变化以及双边贸易模型中的可贸易品部门需求。

*原书页码：P9。对排印不一致和隐含假设的说明为本笔记的推导补充，不视为原文直接给出的定义。*
