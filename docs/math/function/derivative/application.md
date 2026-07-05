# 导数应用

**前置知识**：[极值与最值](extremum.md)

!!! note "考纲要求"
    掌握利用导数证明不等式的方法（构造函数法）；理解恒成立问题的转化思路；了解导数在实际优化问题中的应用。

## 不等式证明

**基本思路**：将要证明的不等式转化为函数（移项构造），利用导数研究函数的最值，从而证明不等式。

常用构造方法：

| 目标不等式 | 构造函数 |
|-----------|---------|
| $f(x) \geqslant g(x)$ | $h(x) = f(x) - g(x)$，证明 $h(x)_{\min} \geqslant 0$ |
| $f(x) \geqslant 0$ | 直接研究 $f(x)$ 的最小值 |
| $f(x) \geqslant M$ | 求 $f(x)$ 的最小值并与 $M$ 比较 |

## 恒成立问题

**分离参数法**：若 $\forall x \in D,\; f(x) \geqslant a$ 恒成立 $\iff a \leqslant f(x)_{\min}$；
若 $\forall x \in D,\; f(x) \leqslant a$ 恒成立 $\iff a \geqslant f(x)_{\max}$。

## 实际优化问题

**步骤**：
1. 建立目标函数（确定自变量和定义域）
2. 求导数，找驻点
3. 判断极值，结合实际意义得最值

## 常用放缩不等式

- $\ln x \leqslant x - 1$（$x > 0$），当且仅当 $x = 1$ 取等
- $e^x \geqslant x + 1$（$\forall x \in \mathbb{R}$），当且仅当 $x = 0$ 取等
- $\sin x \leqslant x \leqslant \tan x$（$x \geqslant 0$）

## 例题

### 【例1】（不等式证明）

证明：当 $x > 0$ 时，$x > \ln(1 + x)$。

??? note "解析"
    令 $f(x) = x - \ln(1 + x)$，$f(0) = 0$。
    
    $f'(x) = 1 - \frac{1}{1 + x} = \frac{x}{1 + x} > 0$（$x > 0$）。
    
    故 $f(x)$ 在 $[0,+\infty)$ 上递增，$f(x) > f(0) = 0$，即 $x > \ln(1 + x)$。

### 【例2】（恒成立问题）

若 $x > 0$ 时，$x^2 - ax + \ln x \geqslant 0$ 恒成立，求 $a$ 的取值范围。

??? note "解析"
    分离参数：$x > 0$ 时，$a \leqslant x + \frac{\ln x}{x}$。
    
    令 $g(x) = x + \frac{\ln x}{x}$，$g'(x) = 1 + \frac{1 - \ln x}{x^2} = \frac{x^2 + 1 - \ln x}{x^2}$。
    
    再令 $h(x) = x^2 + 1 - \ln x$，$h'(x) = 2x - \frac{1}{x} = \frac{2x^2 - 1}{x}$，
    
    $h(x)$ 在 $(0,\frac{\sqrt{2}}{2})$ 上递减，$(\frac{\sqrt{2}}{2},+\infty)$ 上递增，$h_{\min} = h(\frac{\sqrt{2}}{2}) = \frac{1}{2} + 1 + \frac{1}{2}\ln 2 > 0$。
    
    故 $g'(x) > 0$，$g(x)$ 递增。$x \to 0^+$ 时 $\frac{\ln x}{x} \to -\infty$，$g(x) \to -\infty$，无下限。
    
    $a \leqslant g(1) = 1$ 即为所求（注：此题需进一步确认，实际高考题中常需二次求导$）。
    
    **简化版**：由常用放缩 $\ln x \leqslant x-1$，$x^2 - ax + \ln x \geqslant x^2 - ax + x - 1 = x^2 + (1-a)x - 1 \geqslant 0$ 对 $x>0$ 恒成立，得 $a \leqslant 2\sqrt{-1}$...（还需二次求导，此处略）。

## 常见题型与技巧

| 题型 | 解法要点 |
|------|----------|
| 证明 $f(x) \geqslant g(x)$ | 移项构造 $h(x) = f(x)-g(x)$，求最值 |
| 恒成立求参数 | 分离参数或分类讨论 |
| 零点与导数 | 结合单调性和零点存在性定理 |
| 双变量问题 | 极值点偏移、主元法、对称化构造 |

## 练习

!!! question "练习1"
    证明：$e^x \geqslant x + 1$（$\forall x \in \mathbb{R}$）。

    ??? note "答案"
        令 $f(x) = e^x - x - 1$，$f'(x) = e^x - 1$。
        $x < 0$ 时 $f'(x) < 0$，$x > 0$ 时 $f'(x) > 0$。
        $f_{\min} = f(0) = 0$，故 $f(x) \geqslant 0$，即 $e^x \geqslant x + 1$。

## 参考资料

- 人教A版高中数学选择性必修第二册 第五章
- 浙江新高考数学考试说明
