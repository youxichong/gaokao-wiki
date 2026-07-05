# 向量应用

**前置知识**：[数量积](dot-product.md)

!!! note "考纲要求"
    了解向量在几何和物理中的应用；理解用向量法解决几何问题的基本思路（坐标法或基底法）。

## 几何应用

**向量法解几何问题的步骤**：
1. 建立适当的坐标系（或选择基底）
2. 用坐标（或基底）表示几何元素
3. 进行向量运算
4. 将向量结果还原为几何结论

**常见几何问题**：

| 问题 | 向量方法 |
|------|----------|
| 证明垂直 | $\vec{a} \cdot \vec{b} = 0$ |
| 证明平行 | $\vec{a} = \lambda\vec{b}$ |
| 求夹角 | $\cos\theta = \frac{\vec{a}\cdot\vec{b}}{|\vec{a}||\vec{b}|}$ |
| 求距离 | $|\overrightarrow{AB}|$ |
| 三点共线 | $\overrightarrow{AB} = \lambda\overrightarrow{AC}$ |

## 物理应用

- **功**：$W = \vec{F} \cdot \vec{s}$（力与位移的数量积）
- **速度合成**：$\vec{v} = \vec{v}_1 + \vec{v}_2$
- **力的合成与分解**：平行四边形法则

## 例题

### 【例1】（几何应用）

证明：平行四边形两条对角线的平方和等于四条边的平方和。

??? note "解析"
    设平行四边形 $ABCD$，$\overrightarrow{AB} = \vec{a}$，$\overrightarrow{AD} = \vec{b}$。
    
    对角线 $\overrightarrow{AC} = \vec{a} + \vec{b}$，$\overrightarrow{DB} = \vec{a} - \vec{b}$。
    
    $|\overrightarrow{AC}|^2 + |\overrightarrow{DB}|^2 = |\vec{a} + \vec{b}|^2 + |\vec{a} - \vec{b}|^2$
    
    $= (|\vec{a}|^2 + 2\vec{a}\cdot\vec{b} + |\vec{b}|^2) + (|\vec{a}|^2 - 2\vec{a}\cdot\vec{b} + |\vec{b}|^2)$
    
    $= 2(|\vec{a}|^2 + |\vec{b}|^2) = |AB|^2 + |BC|^2 + |CD|^2 + |DA|^2$
    
    得证。

## 参考资料

- 人教A版高中数学必修第二册 第六章
