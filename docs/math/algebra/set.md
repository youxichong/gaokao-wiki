# 集合

**前置知识**：无

!!! note "考纲要求"
    掌握集合的含义与表示方法，理解元素与集合的关系；掌握集合间的基本关系（子集、真子集、相等）；掌握集合的基本运算（交、并、补）；能使用 Venn 图表达集合的关系及运算。

## 定义

**集合**：把一些确定且互不相同的对象汇集在一起，构成一个整体，这个整体就是一个集合（简称**集**）。

**元素**：组成集合的各个对象称为该集合的**元素**。通常用大写字母 $A,B,C,\ldots$ 表示集合，用小写字母 $a,b,c,\ldots$ 表示元素。

若 $a$ 是集合 $A$ 的元素，记作 $a \in A$；否则记作 $a \notin A$。

**集合中元素的三个特性**：
- **确定性**：给定一个集合，任何一个对象是否属于该集合是确定的。
- **互异性**：集合中的元素互不相同。
- **无序性**：集合中的元素没有顺序。

**常用数集**：

| 符号 | 名称 |
|------|------|
| $\mathbb{N}$ | 自然数集（含 0） |
| $\mathbb{N}^*$ 或 $\mathbb{N}_+$ | 正整数集 |
| $\mathbb{Z}$ | 整数集 |
| $\mathbb{Q}$ | 有理数集 |
| $\mathbb{R}$ | 实数集 |
| $\mathbb{C}$ | 复数集 |

## 集合的表示法

1. **列举法**：将集合的元素一一列举出来，写在大括号内。如 $A = \{1, 2, 3, 4, 5\}$。

2. **描述法**：用元素满足的条件表示集合。如 $B = \{x \mid x > 3\}$ 或 $B = \{x \in \mathbb{R} \mid x^2 - 1 = 0\}$。

3. **图示法（Venn 图）**：用封闭曲线内部区域表示集合。

## 集合间的基本关系

| 关系 | 定义 | 记法 | Venn 图特征 |
|------|------|------|-------------|
| 子集 | $A$ 中任意元素都属于 $B$ | $A \subseteq B$（或 $B \supseteq A$） | $A$ 在 $B$ 内部 |
| 真子集 | $A \subseteq B$ 且 $A \neq B$ | $A \subsetneqq B$ | $A$ 在 $B$ 内部且不等 |
| 相等 | $A \subseteq B$ 且 $B \subseteq A$ | $A = B$ | 完全重合 |

**空集**：不含任何元素的集合，记作 $\varnothing$。规定空集是任何集合的子集，即 $\varnothing \subseteq A$。

!!! warning "易错提醒"
    空集是任何**非空**集合的真子集。解题时不要遗漏空集的情况。

**子集个数公式**：含有 $n$ 个元素的集合，其子集有 $2^n$ 个，真子集有 $2^n-1$ 个，非空真子集有 $2^n-2$ 个。

## 集合的基本运算

| 运算 | 定义 | 记法 | 性质 |
|------|------|------|------|
| 交集 | 属于 $A$ **且**属于 $B$ 的元素构成的集合 | $A \cap B = \{x \mid x \in A \text{ 且 } x \in B\}$ | $A \cap B \subseteq A,\; A \cap B \subseteq B$ |
| 并集 | 属于 $A$ **或**属于 $B$ 的元素构成的集合 | $A \cup B = \{x \mid x \in A \text{ 或 } x \in B\}$ | $A \subseteq A \cup B,\; B \subseteq A \cup B$ |
| 补集 | 全集 $U$ 中不属于 $A$ 的元素构成的集合 | $\complement_U A = \{x \mid x \in U \text{ 且 } x \notin A\}$ | $A \cup \complement_U A = U$ |

**运算律**：

$$
\begin{aligned}
A \cap B &= B \cap A, & A \cup B &= B \cup A & &\text{(交换律)} \\
(A \cap B) \cap C &= A \cap (B \cap C), & (A \cup B) \cup C &= A \cup (B \cup C) & &\text{(结合律)} \\
A \cap (B \cup C) &= (A \cap B) \cup (A \cap C), & A \cup (B \cap C) &= (A \cup B) \cap (A \cup C) & &\text{(分配律)}
\end{aligned}
$$

**De Morgan 律**：

$$
\complement_U (A \cap B) = (\complement_U A) \cup (\complement_U B), \qquad
\complement_U (A \cup B) = (\complement_U A) \cap (\complement_U B)
$$

## 例题

### 【例1】（基础题）

已知集合 $A = \{x \in \mathbb{R} \mid x^2 - 3x + 2 = 0\}$，$B = \{x \in \mathbb{N} \mid 0 < x < 5\}$，求 $A \cap B$。

??? note "解析"
    先化简集合：
    
    $A = \{x \mid x^2 - 3x + 2 = 0\} = \{1, 2\}$
    
    $B = \{x \in \mathbb{N} \mid 0 < x < 5\} = \{1, 2, 3, 4\}$
    
    $\therefore A \cap B = \{1, 2\}$。

### 【例2】（含参问题）

已知集合 $A = \{x \mid x^2 - 5x + 6 = 0\}$，$B = \{x \mid mx - 1 = 0\}$。若 $B \subseteq A$，求实数 $m$ 的值。

??? note "解析"
    $A = \{2, 3\}$
    
    由 $B \subseteq A$：
    
    - 若 $B = \varnothing$，则 $m = 0$，满足条件。
    - 若 $B = \{2\}$，则 $2m - 1 = 0$，$m = \frac{1}{2}$。
    - 若 $B = \{3\}$，则 $3m - 1 = 0$，$m = \frac{1}{3}$。
    - 若 $B = A$，则 $B = \{2, 3\}$，但 $B$ 至多含一个元素，不成立。
    
    综上，$m = 0$ 或 $m = \frac{1}{2}$ 或 $m = \frac{1}{3}$。

### 【例3】（补集运算）

设全集 $U = \{1, 2, 3, 4, 5, 6\}$，$A = \{1, 3, 5\}$，$B = \{2, 4, 6\}$。求 $\complement_U (A \cup B)$ 和 $(\complement_U A) \cap (\complement_U B)$，并验证 De Morgan 律。

??? note "解析"
    $A \cup B = \{1, 2, 3, 4, 5, 6\} = U$，$\complement_U (A \cup B) = \varnothing$
    
    $\complement_U A = \{2, 4, 6\} = B$，$\complement_U B = \{1, 3, 5\} = A$
    
    $(\complement_U A) \cap (\complement_U B) = \{2, 4, 6\} \cap \{1, 3, 5\} = \varnothing$
    
    验证得 $\complement_U (A \cup B) = (\complement_U A) \cap (\complement_U B)$，De Morgan 律成立。

## 常见题型与技巧

| 题型 | 特征 | 解法要点 | 易错点 |
|------|------|----------|--------|
| 集合表示互化 | 列举法与描述法互相转化 | 注意元素性质 | 描述法易忽略定义域 |
| 集合间关系判断 | 判断包含、相等关系 | 定义法、列举法 | 忽略空集 |
| 交并补运算 | 求集合的交、并、补 | Venn 图辅助 | 运算顺序错误 |
| 含参集合问题 | 集合含参数，求参数范围 | 分类讨论 | 遗漏空集情况 |
| 新定义集合 | 自定义集合运算符号 | 回归定义 | 混淆运算规则 |

## 练习

!!! question "练习1"
    设集合 $A = \{1, 2, 3\}$，$B = \{2, 3, 4\}$，求 $A \cup B$、$A \cap B$。

    ??? note "答案"
        $A \cup B = \{1, 2, 3, 4\}$，$A \cap B = \{2, 3\}$。

!!! question "练习2"
    已知 $A = \{x \mid -2 \leqslant x \leqslant 3\}$，$B = \{x \mid x < -1 \text{ 或 } x > 4\}$。用区间表示 $A \cap B$、$A \cup B$。

    ??? note "答案"
        $A \cap B = [-2, -1)$，$A \cup B = (-\infty, 3] \cup (4, +\infty)$。

!!! question "练习3"
    集合 $A = \{x \in \mathbb{R} \mid ax^2 + 2x + 1 = 0\}$ 只有一个元素，求实数 $a$ 的值。

    ??? note "答案"
        若 $a = 0$：方程为 $2x + 1 = 0$，$x = -\frac{1}{2}$，恰有一解。
        
        若 $a \neq 0$：判别式 $\Delta = 4 - 4a = 0$，得 $a = 1$。
        
        综上，$a = 0$ 或 $a = 1$。

## 拓展与延伸

!!! tip "拓展"
    - **集合的基数**：有限集合的元素个数记为 $|A|$。容斥原理：$|A \cup B| = |A| + |B| - |A \cap B|$。
    - **集合论视角**：集合是现代数学的基础语言。ZFC 公理系统为集合论提供了严格的公理化基础，是大学数学系「数理逻辑」课程的起点。

## 参考资料

- 人教A版高中数学必修第一册 第一章
- 浙江新高考数学考试说明
