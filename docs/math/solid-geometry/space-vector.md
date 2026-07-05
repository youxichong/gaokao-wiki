# 空间向量与立体几何

**前置知识**：[平面向量](../vector/index.md)、[点线面位置关系](position-relation.md)

!!! note "考纲要求"
    掌握空间向量的坐标表示和运算；能用空间向量证明平行、垂直关系；能用法向量求线面角、二面角和点到平面的距离。

## 空间向量坐标运算

设 $\vec{a}=(x_1,y_1,z_1)$，$\vec{b}=(x_2,y_2,z_2)$：

| 运算 | 公式 |
|------|------|
| 加法 | $\vec{a}+\vec{b}=(x_1+x_2,y_1+y_2,z_1+z_2)$ |
| 减法 | $\vec{a}-\vec{b}=(x_1-x_2,y_1-y_2,z_1-z_2)$ |
| 数乘 | $\lambda\vec{a}=(\lambda x_1,\lambda y_1,\lambda z_1)$ |
| 模 | $|\vec{a}|=\sqrt{x_1^2+y_1^2+z_1^2}$ |
| 数量积 | $\vec{a}\cdot\vec{b}=x_1x_2+y_1y_2+z_1z_2$ |

## 平行与垂直

### 线线关系

- $\vec{a}\parallel\vec{b}\iff \vec{a}=\lambda\vec{b}$
- $\vec{a}\perp\vec{b}\iff \vec{a}\cdot\vec{b}=0$

### 直线与平面

设直线 $l$ 的方向向量为 $\vec{s}$，平面 $\alpha$ 的法向量为 $\vec{n}$：

| 关系 | 向量条件 |
|------|----------|
| $l\parallel\alpha$ | $\vec{s}\perp\vec{n}$，即 $\vec{s}\cdot\vec{n}=0$ |
| $l\perp\alpha$ | $\vec{s}\parallel\vec{n}$ |

### 平面与平面

设平面 $\alpha,\beta$ 的法向量分别为 $\vec{n}_1,\vec{n}_2$：

| 关系 | 向量条件 |
|------|----------|
| $\alpha\parallel\beta$ | $\vec{n}_1\parallel\vec{n}_2$ |
| $\alpha\perp\beta$ | $\vec{n}_1\perp\vec{n}_2$，即 $\vec{n}_1\cdot\vec{n}_2=0$ |

## 法向量求法

若平面 $\alpha$ 内有两条不共线向量 $\vec{a},\vec{b}$，设法向量 $\vec{n}=(x,y,z)$，则

$$
\begin{cases}
\vec{n}\cdot\vec{a}=0\\
\vec{n}\cdot\vec{b}=0
\end{cases}
$$

解这个齐次方程组，取一个非零解即为法向量。

## 例题

### 【例1】（求法向量）

已知平面 $\alpha$ 内有两条不共线向量 $\vec{a}=(1,0,1)$，$\vec{b}=(0,2,1)$，求平面 $\alpha$ 的一个法向量。

??? note "解析"
    设法向量 $\vec{n}=(x,y,z)$，则
    $$
    \begin{cases}
    x+z=0\\
    2y+z=0
    \end{cases}
    $$
    取 $z=2$，得 $x=-2$，$y=-1$。
    
    故 $\vec{n}=(-2,-1,2)$ 是平面 $\alpha$ 的一个法向量。

### 【例2】（证明线面垂直）

在空间直角坐标系中，$A(0,0,0)$，$B(1,0,0)$，$C(0,1,0)$，$D(0,0,2)$。证明：$DO\perp$ 平面 $ABC$，其中 $O=A$。

??? note "解析"
    平面 $ABC$ 内有 $\overrightarrow{AB}=(1,0,0)$，$\overrightarrow{AC}=(0,1,0)$。
    
    $\overrightarrow{AD}=(0,0,2)$。
    
    $\overrightarrow{AD}\cdot\overrightarrow{AB}=0$，$\overrightarrow{AD}\cdot\overrightarrow{AC}=0$，且 $AB$ 与 $AC$ 相交。
    
    因此 $AD\perp$ 平面 $ABC$。

## 常见题型与技巧

| 题型 | 解法要点 |
|------|----------|
| 证明线线垂直 | 取方向向量，算数量积为 $0$ |
| 证明线面平行 | 证明直线方向向量垂直平面法向量 |
| 求平面法向量 | 设 $\vec{n}=(x,y,z)$，列两个垂直方程 |
| 证明面面垂直 | 证明两个平面法向量数量积为 $0$ |

## 练习

!!! question "练习1"
    平面内两向量为 $\vec{a}=(2,1,0)$，$\vec{b}=(1,-1,1)$，求该平面的一个法向量。

    ??? note "答案"
        设 $\vec{n}=(x,y,z)$，有 $2x+y=0$，$x-y+z=0$。取 $x=1$，得 $y=-2$，$z=-3$，故可取 $\vec{n}=(1,-2,-3)$。

## 参考资料

- 人教A版高中数学选择性必修第一册 第一章
