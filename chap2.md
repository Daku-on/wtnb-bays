---
marp: true
theme: academic
paginate: true
math: katex
---
<!-- _class: lead -->
# 『ベイズ統計の理論と方法』 渡辺澄夫 著

## 現時点でのまとめ 第2章

### Dakuon

#### 2023/02/07

---
<!-- _header: 実現可能性 -->
$x\in \mathbf{R}$について、$q(x)$を真の分布、$p(x| w)$を確率モデルとする。

定義 (実現可能なパラメタ集合$W_{00}$)): $W\subset \mathbf{R}$をパラメタ集合とする。

あるパラメタ$w\in W$に対して$q(x)=p(x|w)$とできるとき、$q(x)$は$p$によって実現可能といい、
$$W_{00} := \{w\in W \mid \forall x, \ p(x|w) = q(x)\}$$
とする。

---
<!-- _header: 平均対数損失関数 -->

平均対数損失関数$L(w)$を
$$\begin{aligned}
L(w) &:= -\displaystyle \int q(x)\log p(x|w) dx\\
&= -\int q(x) \log q(x) dx + \int q(x) \log \dfrac{q(x)}{p(x|w)}dx
\end{aligned}$$