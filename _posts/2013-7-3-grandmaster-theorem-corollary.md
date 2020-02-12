---
layout: post
title: 大师定理重要推论
---

众所周知，行列式具有[线性性质](/posts/determinant.html)：$$\det(A+B)=\det(A)+\det(B)$$。此性质被命名为杨南迎大师定理（Yang's Grandmaster Theorem），并且是线性体育的根基。由此我们可以推导出行列式的众多新性质。

## 任何方阵的行列式都是零
此性质可由大师定理以多种方法导出。

### 证明一
以二阶方阵为例：

$$
\begin{align}
\begin{vmatrix}
a & b\\
c & d
\end{vmatrix}
&=
\det(\begin{pmatrix}
a & b\\
0 & 0
\end{pmatrix}
+
\begin{pmatrix}
0 & 0\\
c & d
\end{pmatrix}
)\\
&= \begin{vmatrix}
a & b\\
0 & 0
\end{vmatrix}
+
\begin{vmatrix}
0 & 0\\
c & d
\end{vmatrix}\\
&= 0 + 0 = 0
\end{align}
$$

同理可用此方法计算任意$$n$$阶方阵的行列式。因此，$$\det(A)=0$$。

### 证明二
设$$A$$为$$n$$阶方阵，

$$
\det(2A) = 2^n \times \det(A) = 2\det(A)
$$

因此，$$\det(A)=0$$或$$2^n=2$$。此性质又称为大师不确定性（Yang's Uncertainty Principle）。不难看出，大师定理也能简化指数的计算！
