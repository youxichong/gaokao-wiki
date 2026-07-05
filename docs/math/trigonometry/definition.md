# 三角函数定义与性质

**前置知识**：[角与弧度制](angle-radian.md)

!!! note "考纲要求"
    理解任意角三角函数的定义；掌握三角函数在各象限的符号规律；掌握同角三角函数的基本关系式；理解诱导公式及其应用。

## 定义

在平面直角坐标系中，设角 $\alpha$ 的终边与单位圆交于点 $P(x,y)$，则：

$$
\sin\alpha = y,\quad \cos\alpha = x,\quad \tan\alpha = \frac{y}{x}\;(x \neq 0)
$$

## 各象限符号

| 象限 | $\sin\alpha$ | $\cos\alpha$ | $\tan\alpha$ |
|------|-------------|-------------|-------------|
| 第一象限 | $+$ | $+$ | $+$ |
| 第二象限 | $+$ | $-$ | $-$ |
| 第三象限 | $-$ | $-$ | $+$ |
| 第四象限 | $-$ | $+$ | $-$ |

## 同角三角函数的基本关系

- **平方关系**：$\sin^2\alpha + \cos^2\alpha = 1$
- **商数关系**：$\tan\alpha = \frac{\sin\alpha}{\cos\alpha}$

## 诱导公式

| 公式 | 内容 |
|------|------|
| $\sin(\alpha + 2k\pi) = \sin\alpha$，$\cos(\alpha + 2k\pi) = \cos\alpha$ | 周期为 $2\pi$ |
| $\sin(\alpha + \pi) = -\sin\alpha$，$\cos(\alpha + \pi) = -\cos\alpha$ | 周期平移 |
| $\sin(-\alpha) = -\sin\alpha$，$\cos(-\alpha) = \cos\alpha$ | 奇偶性 |
| $\sin(\pi - \alpha) = \sin\alpha$，$\cos(\pi - \alpha) = -\cos\alpha$ | 互补角 |
| $\sin(\frac{\pi}{2} - \alpha) = \cos\alpha$，$\cos(\frac{\pi}{2} - \alpha) = \sin\alpha$ | 互余角 |

## 例题

### 【例1】（基础题）

已知 $\sin\alpha = \frac{3}{5}$ 且 $\alpha$ 为第二象限角，求 $\cos\alpha$ 和 $\tan\alpha$。

??? note "解析"
    由平方关系：$\cos^2\alpha = 1 - \sin^2\alpha = 1 - \frac{9}{25} = \frac{16}{25}$
    
    $\alpha$ 为第二象限角，$\cos\alpha < 0$，故 $\cos\alpha = -\frac{4}{5}$
    
    $\tan\alpha = \frac{\sin\alpha}{\cos\alpha} = \frac{3/5}{-4/5} = -\frac{3}{4}$

## 常见题型与技巧

| 题型 | 解法要点 |
|------|----------|
| 已知一个三角函数值求其他 | 平方关系配合象限符号 |
| 化简求值 | 利用诱导公式化到锐角 |
| 符号判断 | 根据终边所在象限判断 |

## 参考资料

- 人教A版高中数学必修第一册 第五章
