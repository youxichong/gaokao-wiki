# 空间角与距离

**前置知识**：[空间向量与立体几何](space-vector.md)

!!! note "考纲要求"
    掌握异面直线所成角、直线与平面所成角、二面角的求法；掌握点到平面距离的空间向量公式。能在立体几何解答题中完成建系、设点、求角与距离。

## 异面直线所成角

设两条异面直线的方向向量分别为 $\vec{a},\vec{b}$，所成角为 $\theta\in[0,\frac{\pi}{2}]$，则

$$
\cos\theta=\frac{|\vec{a}\cdot\vec{b}|}{|\vec{a}||\vec{b}|}
$$

## 直线与平面所成角

设直线 $l$ 的方向向量为 $\vec{s}$，平面 $\alpha$ 的法向量为 $\vec{n}$，直线与平面所成角为 $\theta\in[0,\frac{\pi}{2}]$，则

$$
\sin\theta=\frac{|\vec{s}\cdot\vec{n}|}{|\vec{s}||\vec{n}|}
$$

!!! tip "为什么是正弦"
    直线与平面所成角是直线与其在平面内投影的夹角；方向向量与法向量的夹角是它的余角，因此使用 $\sin\theta$。

## 二面角

设两个平面 $\alpha,\beta$ 的法向量分别为 $\vec{n}_1,\vec{n}_2$，二面角大小为 $\theta$。若题目要求锐角或钝角，结合图形判断符号；若只求大小，常用

$$
\cos\theta=\frac{|\vec{n}_1\cdot\vec{n}_2|}{|\vec{n}_1||\vec{n}_2|}
$$

## 点到平面的距离

设平面 $\alpha$ 的法向量为 $\vec{n}$，点 $P$ 为平面外一点，$A$ 为平面内一点，则点 $P$ 到平面 $\alpha$ 的距离为

$$
d=\frac{|\overrightarrow{AP}\cdot\vec{n}|}{|\vec{n}|}
$$

## 例题

### 【例1】（线面角）

在空间直角坐标系中，平面 $\alpha$ 的法向量为 $\vec{n}=(0,0,1)$，直线 $l$ 的方向向量为 $\vec{s}=(1,1,1)$，求直线 $l$ 与平面 $\alpha$ 所成角。

??? note "解析"
    设所成角为 $\theta$，则
    $$
    \sin\theta=\frac{|\vec{s}\cdot\vec{n}|}{|\vec{s}||\vec{n}|}=\frac{|1|}{\sqrt{1^2+1^2+1^2}\cdot1}=\frac{1}{\sqrt3}
    $$
    
    故 $\theta=\arcsin\frac{1}{\sqrt3}$。

### 【例2】（点面距）

已知平面 $\alpha$ 过点 $A(1,0,0)$，法向量 $\vec{n}=(2,-1,2)$，求点 $P(3,1,4)$ 到平面 $\alpha$ 的距离。

??? note "解析"
    $\overrightarrow{AP}=(2,1,4)$。
    
    $$
    d=\frac{|\overrightarrow{AP}\cdot\vec{n}|}{|\vec{n}|}=\frac{|2\cdot2+1\cdot(-1)+4\cdot2|}{\sqrt{2^2+(-1)^2+2^2}}=\frac{|4-1+8|}{3}=\frac{11}{3}
    $$

### 【例3】（二面角）

已知平面 $\alpha$ 的法向量 $\vec{n}_1=(1,1,0)$，平面 $\beta$ 的法向量 $\vec{n}_2=(1,0,1)$，求两平面所成锐二面角。

??? note "解析"
    $$
    \cos\theta=\frac{|\vec{n}_1\cdot\vec{n}_2|}{|\vec{n}_1||\vec{n}_2|}=\frac{|1|}{\sqrt2\cdot\sqrt2}=\frac12
    $$
    
    故锐二面角为 $60^\circ$。

## 常见题型与技巧

| 题型 | 公式 | 易错点 |
|------|------|--------|
| 异面直线角 | 方向向量夹角取锐角 | 忘记绝对值 |
| 线面角 | $\sin\theta=\frac{|\vec{s}\cdot\vec{n}|}{|\vec{s}||\vec{n}|}$ | 误用余弦 |
| 二面角 | 法向量夹角或其补角 | 需按题意判断锐/钝 |
| 点面距 | $d=\frac{|\overrightarrow{AP}\cdot\vec{n}|}{|\vec{n}|}$ | $A$ 必须取平面内点 |

## 练习

!!! question "练习1"
    直线方向向量 $\vec{s}=(2,0,1)$，平面法向量 $\vec{n}=(1,0,0)$，求直线与平面所成角的正弦值。

    ??? note "答案"
        $\sin\theta=\frac{|2|}{\sqrt5\cdot1}=\frac{2}{\sqrt5}=\frac{2\sqrt5}{5}$。

!!! question "练习2"
    平面过点 $A(0,1,0)$，法向量为 $\vec{n}=(1,2,2)$，求点 $P(1,3,2)$ 到该平面的距离。

    ??? note "答案"
        $\overrightarrow{AP}=(1,2,2)$，$d=\frac{|1+4+4|}{\sqrt{1+4+4}}=3$。

## 参考资料

- 人教A版高中数学选择性必修第一册 第一章
