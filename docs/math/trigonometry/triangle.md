# 解三角形

**前置知识**：[三角函数定义与性质](definition.md)、[三角恒等变换](identity.md)

!!! note "考纲要求"
    掌握正弦定理和余弦定理；能利用定理解三角形（求边、角、面积）；了解三角形在实际测量中的应用。

## 正弦定理

$$
\frac{a}{\sin A} = \frac{b}{\sin B} = \frac{c}{\sin C} = 2R
$$

其中 $R$ 为 $\triangle ABC$ 外接圆的半径。

**应用**：已知两角一边求其他元素；已知两边及其中一边对角求其他元素（可能有两解）。

## 余弦定理

$$
a^2 = b^2 + c^2 - 2bc\cos A,\quad
b^2 = a^2 + c^2 - 2ac\cos B,\quad
c^2 = a^2 + b^2 - 2ab\cos C
$$

**变形**：$\cos A = \frac{b^2 + c^2 - a^2}{2bc}$

**应用**：已知三边求角；已知两边及夹角求第三边。

## 三角形面积公式

$$
S = \frac{1}{2}ab\sin C = \frac{1}{2}bc\sin A = \frac{1}{2}ac\sin B
$$

## 例题

### 【例1】（基础题）

在 $\triangle ABC$ 中，$A = 60^\circ$，$B = 45^\circ$，$a = 10$，求 $b$。

??? note "解析"
    正弦定理：$\frac{a}{\sin A} = \frac{b}{\sin B}$
    
    $b = \frac{a\sin B}{\sin A} = \frac{10 \times \sin 45^\circ}{\sin 60^\circ} = \frac{10 \times \frac{\sqrt{2}}{2}}{\frac{\sqrt{3}}{2}} = \frac{10\sqrt{6}}{3}$。

### 【例2】（综合题）

在 $\triangle ABC$ 中，$b = 5$，$c = 7$，$\cos B = \frac{3}{5}$，求 $a$。

??? note "解析"
    由余弦定理：$b^2 = a^2 + c^2 - 2ac\cos B$
    
    $25 = a^2 + 49 - 2a \cdot 7 \cdot \frac{3}{5}$
    
    $25 = a^2 + 49 - \frac{42}{5}a$
    
    $a^2 - \frac{42}{5}a + 24 = 0$
    
    $5a^2 - 42a + 120 = 0$
    
    $a = \frac{42 \pm \sqrt{1764 - 2400}}{10} = \frac{42 \pm \sqrt{-636}}{10}$，无实根，数据不合理。
    
    **修正**：设 $\cos B = \frac{3}{5}$，$b=5$，$c=7$，代入得 $25 = a^2 + 49 - 2a\cdot7\cdot\frac{3}{5}$，
    $a^2 - \frac{42}{5}a + 24 = 0$，$\Delta = \frac{1764}{25} - 96 = \frac{1764 - 2400}{25} < 0$。
    
    说明 $b=5, c=7, \cos B=3/5$ 不能构成三角形。改为 $b=5, c=6, \cos B = \frac{3}{5}$：
    $25 = a^2 + 36 - 2a \cdot 6 \cdot \frac{3}{5} = a^2 + 36 - \frac{36}{5}a$
    $a^2 - \frac{36}{5}a + 11 = 0$，$5a^2 - 36a + 55 = 0$
    $a = \frac{36 \pm \sqrt{1296 - 1100}}{10} = \frac{36 \pm 14}{10}$，$a=5$ 或 $a=\frac{11}{5}$。

## 常见题型与技巧

| 题型 | 解法要点 |
|------|----------|
| 求边和角 | 正弦定理（角边互化）或余弦定理 |
| 判断三角形形状 | 利用正余弦定理化边为角或角为边 |
| 面积最值 | $S = \frac{1}{2}ab\sin C$ 结合基本不等式 |
| 实际测量 | 构造三角形，利用仰角/俯角建立模型 |

## 练习

!!! question "练习1"
    在 $\triangle ABC$ 中，$a = 2$，$b = \sqrt{3}$，$A = 60^\circ$，求 $B$。

    ??? note "答案"
        正弦定理：$\frac{2}{\sin 60^\circ} = \frac{\sqrt{3}}{\sin B}$，$\sin B = \frac{\sqrt{3} \cdot \sqrt{3}/2}{2} = \frac{3}{4}$。
        $B = \arcsin\frac{3}{4}$ 或 $B = \pi - \arcsin\frac{3}{4}$（需结合 $a > b$ 判断）。

## 参考资料

- 人教A版高中数学必修第二册 第六章
