# 三角恒等变换

**前置知识**：[三角函数定义与性质](definition.md)

!!! note "考纲要求"
    掌握两角和与差的正弦、余弦、正切公式；掌握二倍角公式；能运用公式进行化简、求值和证明。

## 两角和与差公式

$$
\begin{aligned}
\sin(\alpha \pm \beta) &= \sin\alpha\cos\beta \pm \cos\alpha\sin\beta \\
\cos(\alpha \pm \beta) &= \cos\alpha\cos\beta \mp \sin\alpha\sin\beta \\
\tan(\alpha \pm \beta) &= \frac{\tan\alpha \pm \tan\beta}{1 \mp \tan\alpha\tan\beta}
\end{aligned}
$$

## 二倍角公式

$$
\begin{aligned}
\sin 2\alpha &= 2\sin\alpha\cos\alpha \\
\cos 2\alpha &= \cos^2\alpha - \sin^2\alpha = 2\cos^2\alpha - 1 = 1 - 2\sin^2\alpha \\
\tan 2\alpha &= \frac{2\tan\alpha}{1 - \tan^2\alpha}
\end{aligned}
$$

## 降幂升幂公式

$$
\sin^2\alpha = \frac{1 - \cos 2\alpha}{2},\qquad \cos^2\alpha = \frac{1 + \cos 2\alpha}{2}
$$

## 辅助角公式

$$
a\sin x + b\cos x = \sqrt{a^2 + b^2}\sin(x + \varphi)
$$

其中 $\varphi$ 满足 $\sin\varphi = \frac{b}{\sqrt{a^2+b^2}},\; \cos\varphi = \frac{a}{\sqrt{a^2+b^2}}$。

## 例题

### 【例1】（基础题）

求 $\sin 75^\circ$ 的值。

??? note "解析"
    $\sin 75^\circ = \sin(45^\circ + 30^\circ) = \sin45^\circ\cos30^\circ + \cos45^\circ\sin30^\circ$
    
    $= \frac{\sqrt{2}}{2} \cdot \frac{\sqrt{3}}{2} + \frac{\sqrt{2}}{2} \cdot \frac{1}{2} = \frac{\sqrt{6} + \sqrt{2}}{4}$。

### 【例2】（综合题）

已知 $\cos\alpha = \frac{3}{5}$，$\alpha \in (0, \frac{\pi}{2})$，求 $\sin 2\alpha$。

??? note "解析"
    $\sin\alpha = \sqrt{1 - \cos^2\alpha} = \sqrt{1 - \frac{9}{25}} = \frac{4}{5}$
    
    $\sin 2\alpha = 2\sin\alpha\cos\alpha = 2 \times \frac{4}{5} \times \frac{3}{5} = \frac{24}{25}$。

## 常见题型与技巧

| 题型 | 解法要点 |
|------|----------|
| 求值化简 | 观察角的关系，选择合适的公式 |
| 证明恒等式 | 从繁到简，统一角或函数名 |
| 辅助角应用 | 将 $a\sin x + b\cos x$ 合并求最值 |

## 参考资料

- 人教A版高中数学必修第一册 第五章
