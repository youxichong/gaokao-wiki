# 不等式

**前置知识**：[集合](set.md)

!!! note "考纲要求"
    理解不等式的性质，掌握一元二次不等式的解法；掌握基本不等式 $\sqrt{ab} \leqslant \frac{a+b}{2}$ 及其应用；了解二元一次不等式组与平面区域；理解线性规划及其应用（新高考对该部分要求有所降低）。

## 不等式的性质

设 $a, b, c, d \in \mathbb{R}$：

| 性质 | 内容 |
|------|------|
| 对称性 | $a > b \iff b < a$ |
| 传递性 | $a > b,\; b > c \Rightarrow a > c$ |
| 加法单调性 | $a > b \Rightarrow a + c > b + c$ |
| 乘法单调性 | $a > b,\; c > 0 \Rightarrow ac > bc$；$a > b,\; c < 0 \Rightarrow ac < bc$ |
| 同向可加 | $a > b,\; c > d \Rightarrow a + c > b + d$ |
| 同向同正可乘 | $a > b > 0,\; c > d > 0 \Rightarrow ac > bd$ |
| 同正可倒 | $a > b > 0 \Rightarrow \frac{1}{a} < \frac{1}{b}$ |
| 乘方性质 | $a > b > 0 \Rightarrow a^n > b^n\;(n \in \mathbb{N}^*)$ |
| 开方性质 | $a > b > 0 \Rightarrow \sqrt[n]{a} > \sqrt[n]{b}\;(n \in \mathbb{N}^*)$ |

## 一元二次不等式

形如 $ax^2 + bx + c > 0$（$\geqslant 0$，$< 0$，$\leqslant 0$）的不等式（$a \neq 0$）。

求解步骤：**一化**（化二次项系数为正）→ **二判**（求判别式 $\Delta = b^2 - 4ac$）→ **三求根** → **四写解集**。

| $\Delta$ | $y = ax^2 + bx + c\;(a>0)$ 的图像 | $ax^2 + bx + c > 0$ | $ax^2 + bx + c < 0$ |
|-----------|-----------------------------------|----------------------|---------------------|
| $\Delta > 0$（两实根 $x_1 < x_2$） | 开口向上，与 $x$ 轴交两点 | $x < x_1$ 或 $x > x_2$ | $x_1 < x_2 < x$ |
| $\Delta = 0$（重根 $x_0$） | 开口向上，与 $x$ 轴相切 | $x \neq x_0$ | 无解 |
| $\Delta < 0$ | 开口向上，与 $x$ 轴无交点 | $\mathbb{R}$ | 无解 |

## 基本不等式

$$
\frac{a + b}{2} \geqslant \sqrt{ab} \qquad (a, b \geqslant 0)
$$

当且仅当 $a = b$ 时取等号。

**常用变形**：

$$
a^2 + b^2 \geqslant 2ab,\qquad a + b \geqslant 2\sqrt{ab},\qquad ab \leqslant \left(\frac{a+b}{2}\right)^2
$$

**"一正二定三相等"**：使用基本不等式时需满足——
1. $a, b$ 均为正数；
2. 和或积为定值；
3. 取等条件能成立。

### 常见应用

| 目标 | 配凑技巧 | 示例 |
|------|----------|------|
| 求 $x + \frac{k}{x}$ 最小值 | 直接利用 $a + b \geqslant 2\sqrt{ab}$ | $x + \frac{1}{x} \geqslant 2\;(x > 0)$ |
| 求 $ax + \frac{b}{x}$ 最小值 | 同上 | $2x + \frac{1}{x} \geqslant 2\sqrt{2}$ |
| 求 $x(1-x)$ 最大值 | 构造和为定值 | $x(1-x) \leqslant \frac{1}{4}\;(x \in [0,1])$ |
| 求 $\frac{1}{a} + \frac{1}{b}$ 最小值 | 结合 $a+b$ 为定值 | 若 $a+b=1$，则 $\frac{1}{a}+\frac{1}{b} \geqslant 4$ |

## 其他重要不等式

- **柯西不等式**：$(a^2 + b^2)(c^2 + d^2) \geqslant (ac + bd)^2$
- **绝对值不等式**：$|a| - |b| \leqslant |a \pm b| \leqslant |a| + |b|$

## 例题

### 【例1】（基础题）

解不等式 $-x^2 + 3x + 10 \geqslant 0$。

??? note "解析"
    两边同乘 $-1$：$x^2 - 3x - 10 \leqslant 0$。
    
    因式分解：$(x - 5)(x + 2) \leqslant 0$。
    
    解得 $-2 \leqslant x \leqslant 5$。
    
    故解集为 $\{x \mid -2 \leqslant x \leqslant 5\}$。

### 【例2】（基本不等式）

已知 $x > 0$，求 $x + \frac{4}{x}$ 的最小值。

??? note "解析"
    由基本不等式：
    
    $$
    x + \frac{4}{x} \geqslant 2\sqrt{x \cdot \frac{4}{x}} = 2\sqrt{4} = 4
    $$
    
    当且仅当 $x = \frac{4}{x}$，即 $x = 2$（$x > 0$）时取等号。
    
    故最小值为 $4$。

### 【例3】（综合应用）

已知 $x > 0,\; y > 0$，且 $\frac{1}{x} + \frac{1}{y} = 1$，求 $x + y$ 的最小值。

??? note "解析"
    方法一（乘"1"法）：
    
    $$
    x + y = (x + y)\left(\frac{1}{x} + \frac{1}{y}\right) = 2 + \frac{y}{x} + \frac{x}{y}
    $$
    
    由基本不等式：$\frac{y}{x} + \frac{x}{y} \geqslant 2\sqrt{\frac{y}{x} \cdot \frac{x}{y}} = 2$
    
    所以 $x + y \geqslant 4$，当且仅当 $\frac{y}{x} = \frac{x}{y}$ 即 $x = y = 2$ 时取等号。
    
    方法二（代入法）：由 $\frac{1}{x} + \frac{1}{y} = 1$ 得 $y = \frac{x}{x - 1}$（$x > 1$），
    
    $x + y = x + \frac{x}{x - 1} = x + 1 + \frac{1}{x - 1} = (x - 1) + \frac{1}{x - 1} + 2 \geqslant 2\sqrt{(x-1)\cdot\frac{1}{x-1}} + 2 = 4$

### 【例4】（线性规划初步）

画出不等式组 $\begin{cases} x + y \geqslant 1 \\ x - y \leqslant 1 \\ x \geqslant 0 \end{cases}$ 表示的平面区域。

??? note "解析"
    分别画出三条直线：
    
    1. $x + y = 1$（取上方）
    2. $x - y = 1$（取下方）
    3. $x = 0$（取右侧）
    
    三条直线围成的三角形区域（含边界）即为所求平面区域。
    
    注：新高考对此部分要求较低，了解基本画法即可。

## 常见题型与技巧

| 题型 | 特征 | 解法要点 | 易错点 |
|------|------|----------|--------|
| 一元二次不等式 | $ax^2 + bx + c > 0$ | 因式分解或求根公式 | 二次项系数为负时忘变方向 |
| 分式不等式 | $\frac{f(x)}{g(x)} > 0$ | 转化为乘积形式，注意分母不为零 | 分母为零的情况 |
| 基本不等式求最值 | 求 $x + \frac{k}{x}$ 等最值 | 配凑"和定"或"积定" | 忽视"正"的条件 |
| 不等式恒成立 | 对 $\forall x$ 恒成立 | 分离参数或判别式法 | 端点验证 |
| 线性规划（含参） | 目标函数含参数 | 数形结合，平移直线 | 边界取等判断 |

## 练习

!!! question "练习1"
    解不等式 $x^2 - 5x + 6 < 0$。

    ??? note "答案"
        $(x - 2)(x - 3) < 0$，解得 $2 < x < 3$。

!!! question "练习2"
    求 $y = x + \frac{1}{x - 1}\;(x > 1)$ 的最小值。

    ??? note "答案"
        $y = (x - 1) + \frac{1}{x - 1} + 1 \geqslant 2\sqrt{(x-1)\cdot\frac{1}{x-1}} + 1 = 3$。当 $x = 2$ 时取最小值 $3$。

!!! question "练习3"
    已知 $x > 0,\; y > 0,\; x + y = 1$，求 $\frac{1}{x} + \frac{4}{y}$ 的最小值。

    ??? note "答案"
        $\frac{1}{x} + \frac{4}{y} = (x + y)\left(\frac{1}{x} + \frac{4}{y}\right) = 5 + \frac{y}{x} + \frac{4x}{y} \geqslant 5 + 2\sqrt{\frac{y}{x} \cdot \frac{4x}{y}} = 9$。当 $y = 2x = \frac{2}{3}$ 时取最小值 $9$。

## 拓展与延伸

!!! tip "拓展"
    - **不等式与函数**：一元二次不等式本质上对应二次函数图像的在 $x$ 轴上下问题，与函数的零点、值域紧密相关。
    - **柯西不等式的向量形式**：$\vec{a} \cdot \vec{b} \leqslant |\vec{a}||\vec{b}|$，这与不等式 $(\sum a_i^2)(\sum b_i^2) \geqslant (\sum a_i b_i)^2$ 等价。
    - **排序不等式**：同序和 $\geqslant$ 乱序和 $\geqslant$ 反序和，是竞赛数学的常见工具。

## 参考资料

- 人教A版高中数学必修第一册 第二章
- 人教A版高中数学必修第一册 第五章（基本不等式）
- 浙江新高考数学考试说明
