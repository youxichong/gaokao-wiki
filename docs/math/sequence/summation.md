# 数列求和

**前置知识**：[等差数列](arithmetic.md)、[等比数列](geometric.md)

!!! note "考纲要求"
    掌握数列求和的常用方法：公式法、裂项相消法、错位相减法、分组求和法；能根据数列特点选择合适的方法。

## 公式法

直接利用等差或等比数列求和公式。

## 裂项相消法

将通项拆分为两项的差，在求和过程中相邻项抵消。

常见裂项形式：

| 通项 | 裂项 |
|------|------|
| $\frac{1}{n(n+1)}$ | $\frac{1}{n} - \frac{1}{n+1}$ |
| $\frac{1}{n(n+k)}$ | $\frac{1}{k}(\frac{1}{n} - \frac{1}{n+k})$ |
| $\frac{1}{(2n-1)(2n+1)}$ | $\frac{1}{2}(\frac{1}{2n-1} - \frac{1}{2n+1})$ |
| $\frac{1}{\sqrt{n} + \sqrt{n+1}}$ | $\sqrt{n+1} - \sqrt{n}$ |

## 错位相减法

适用于等差数列 $\times$ 等比数列形式的求和（如 $a_n = (kn+b)q^n$）。

步骤：写出 $S_n$ → 乘以公比得到 $qS_n$ → 相减 → 化简。

## 分组求和法

将数列分为几个可求和的部分分别求和。

## 例题

### 【例1】（裂项相消）

求 $S_n = \frac{1}{1\times2} + \frac{1}{2\times3} + \cdots + \frac{1}{n(n+1)}$。

??? note "解析"
    $\frac{1}{n(n+1)} = \frac{1}{n} - \frac{1}{n+1}$
    
    $S_n = (1 - \frac{1}{2}) + (\frac{1}{2} - \frac{1}{3}) + \cdots + (\frac{1}{n} - \frac{1}{n+1}) = 1 - \frac{1}{n+1} = \frac{n}{n+1}$

### 【例2】（错位相减）

求 $S_n = 1 \cdot 2 + 2 \cdot 2^2 + 3 \cdot 2^3 + \cdots + n \cdot 2^n$。

??? note "解析"
    $S_n = 1\cdot2 + 2\cdot2^2 + 3\cdot2^3 + \cdots + n\cdot2^n$
    
    $2S_n = \quad\quad 1\cdot2^2 + 2\cdot2^3 + \cdots + (n-1)\cdot2^n + n\cdot2^{n+1}$
    
    相减：$-S_n = 2 + 2^2 + 2^3 + \cdots + 2^n - n\cdot2^{n+1}$
    
    $-S_n = \frac{2(2^n-1)}{2-1} - n\cdot2^{n+1} = 2^{n+1} - 2 - n\cdot2^{n+1}$
    
    $S_n = (n-1)2^{n+1} + 2$

## 参考资料

- 人教A版高中数学选择性必修第二册 第四章
