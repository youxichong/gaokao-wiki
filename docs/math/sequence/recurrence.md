# 递推数列

**前置知识**：[等差数列](arithmetic.md)、[等比数列](geometric.md)

!!! note "考纲要求"
    掌握由递推关系求通项公式的常见方法；理解 $a_n$ 与 $S_n$ 的关系。

## $a_n$ 与 $S_n$ 的关系

$$
a_n = \begin{cases}
S_1, & n = 1 \\
S_n - S_{n-1}, & n \geqslant 2
\end{cases}
$$

## 常见递推类型及解法

| 递推形式 | 方法 | 构造 |
|---------|------|------|
| $a_{n+1} = a_n + f(n)$ | 累加法 | $a_n = a_1 + \sum_{k=1}^{n-1} f(k)$ |
| $a_{n+1} = a_n \cdot f(n)$ | 累乘法 | $a_n = a_1 \cdot \prod_{k=1}^{n-1} f(k)$ |
| $a_{n+1} = pa_n + q$ | 构造等比 | $a_{n+1} - \lambda = p(a_n - \lambda)$，$\lambda = \frac{q}{1-p}$ |
| $a_{n+1} = pa_n + qn + r$ | 待定系数 | 设 $a_{n+1}+A(n+1)+B = p(a_n+An+B)$ |
| $a_{n+1} = \frac{pa_n}{qa_n + r}$ | 取倒数 | $\frac{1}{a_{n+1}} = \frac{r}{p}\cdot\frac{1}{a_n} + \frac{q}{p}$ |

## 例题

### 【例1】（累加法）

已知 $a_1 = 1$，$a_{n+1} = a_n + 2n$，求 $a_n$。

??? note "解析"
    $a_n = a_1 + \sum_{k=1}^{n-1} 2k = 1 + 2 \times \frac{(n-1)n}{2} = 1 + n(n-1) = n^2 - n + 1$

### 【例2】（构造等比）

已知 $a_1 = 1$，$a_{n+1} = 2a_n + 3$，求 $a_n$。

??? note "解析"
    设 $a_{n+1} + \lambda = 2(a_n + \lambda)$，展开得 $a_{n+1} = 2a_n + \lambda$。
    
    与 $a_{n+1} = 2a_n + 3$ 对比，$\lambda = 3$。
    
    故 $\{a_n + 3\}$ 是以 $a_1+3=4$ 为首项，$2$ 为公比的等比数列。
    
    $a_n + 3 = 4 \times 2^{n-1} = 2^{n+1}$，$a_n = 2^{n+1} - 3$。

## 参考资料

- 人教A版高中数学选择性必修第二册 第四章
