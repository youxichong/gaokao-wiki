# 数量积

**前置知识**：[平面向量基本定理](basis.md)

!!! note "考纲要求"
    理解平面向量数量积的定义；掌握数量积的坐标运算；理解向量投影的概念；能用数量积判断向量的垂直关系。

## 定义

$$
\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos\theta \quad (\theta = \langle\vec{a},\vec{b}\rangle)
$$

**坐标形式**：若 $\vec{a} = (x_1, y_1)$，$\vec{b} = (x_2, y_2)$，则

$$
\vec{a} \cdot \vec{b} = x_1x_2 + y_1y_2
$$

## 性质

- $\vec{a} \perp \vec{b} \iff \vec{a} \cdot \vec{b} = 0 \iff x_1x_2 + y_1y_2 = 0$
- $\vec{a} /\!/ \vec{b} \iff \vec{a} \cdot \vec{b} = \pm |\vec{a}||\vec{b}| \iff x_1y_2 = x_2y_1$
- $\vec{a} \cdot \vec{a} = |\vec{a}|^2$
- $\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|} = \frac{x_1x_2 + y_1y_2}{\sqrt{x_1^2 + y_1^2}\sqrt{x_2^2 + y_2^2}}$

## 投影

$\vec{b}$ 在 $\vec{a}$ 方向上的投影为：

$$
|\vec{b}|\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}|}
$$

## 例题

### 【例1】（基础题）

已知 $\vec{a} = (2,3)$，$\vec{b} = (-1,2)$，求 $\vec{a} \cdot \vec{b}$ 和 $\cos\langle\vec{a},\vec{b}\rangle$。

??? note "解析"
    $\vec{a} \cdot \vec{b} = 2 \times (-1) + 3 \times 2 = -2 + 6 = 4$
    
    $|\vec{a}| = \sqrt{4 + 9} = \sqrt{13}$，$|\vec{b}| = \sqrt{1 + 4} = \sqrt{5}$
    
    $\cos\theta = \frac{4}{\sqrt{13} \cdot \sqrt{5}} = \frac{4}{\sqrt{65}} = \frac{4\sqrt{65}}{65}$

### 【例2】（垂直判定）

已知 $\vec{a} = (1,2)$，$\vec{b} = (3,m)$，且 $\vec{a} \perp \vec{b}$，求 $m$。

??? note "解析"
    $\vec{a} \perp \vec{b} \iff \vec{a} \cdot \vec{b} = 0$
    
    $1 \times 3 + 2 \times m = 0$，$3 + 2m = 0$，$m = -\frac{3}{2}$。

## 参考资料

- 人教A版高中数学必修第二册 第六章
