---
marp: true
theme: academic
paginate: true
math: katex
---
<!-- _class: lead -->
# 『ベイズ統計の理論と方法』 渡辺澄夫 著

## 現時点でのまとめ 第1章

### Dakuon

#### 2023/02/07
---
<!-- _header: スライドタイトル -->
定義 (事後分布): $0 < \beta\in \mathbf{R} < \infty$を逆温度とし、パラメータ$w$の事後分布を
$$p(w|X^n) = \dfrac{1}{Z_n(\beta)}\phi(w)\prod_{i=1}^{n}p(X_i|w)^{\beta} $$
とする。

ここでのポイントは逆温度$\beta$の導入である。「スペクトラムを入れると理論は成功しやすい」


---
<!-- _header: わおん -->

$x\in \mathbf{R}$について、$q(x)$を真の分布、$p(x| w)$を確率モデルとする。

定義 (確率モデル): 

---
<!-- _header:  -->
