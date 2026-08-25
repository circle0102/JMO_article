# ベクトル

## 1. ベクトルの基本

原点を $O$ とし、各点の位置ベクトルを

$\overrightarrow{OA}=\mathbf{a},\quad \overrightarrow{OB}=\mathbf{b},\quad \overrightarrow{OC}=\mathbf{c}$

とする。

### 点の差

$\overrightarrow{AB}=\mathbf{b}-\mathbf{a}$

### 長さ

$|\overrightarrow{AB}|^2=|\mathbf{b}-\mathbf{a}|^2$

### 内積

ベクトル $\mathbf{u},\mathbf{v}$ のなす角を $\theta$ とすると、

$\mathbf{u}\cdot\mathbf{v}=|\mathbf{u}||\mathbf{v}|\cos\theta$

$\mathbf{u}=(a_1,a_2), \mathbf{v}=(b_1,b_2)$とした時、

$\mathbf{u}\cdot\mathbf{v}=a_1b_1+a_2b_2$

したがって、

- 直交： $\mathbf{u}\cdot\mathbf{v}=0$
- 鋭角： $\mathbf{u}\cdot\mathbf{v}>0$
- 鈍角： $\mathbf{u}\cdot\mathbf{v}<0$
- 平行： $\mathbf{u}=k\mathbf{v}$

### 余弦定理

$|\mathbf{a}-\mathbf{b}|^2=|\mathbf{a}|^2+|\mathbf{b}|^2-2\mathbf{a}\cdot\mathbf{b}$

### コーシー・シュワルツの不等式

$(\mathbf{a}\cdot\mathbf{b})^2\leq|\mathbf{a}|^2|\mathbf{b}|^2$

### 射影

$\mathbf{a}$ を $\mathbf{b}$ の方向へ射影したベクトルを $\mathbf{p}$ とすると、

$\mathbf{p}=\frac{\mathbf{a}\cdot\mathbf{b}}{|\mathbf{b}|^2}\mathbf{b}$

となる。

---

## 2. 距離・位置ベクトル

### 点と直線の距離

点 $P$ から直線上の点 $H$ までの距離を考える。

直線の法線ベクトルを $\mathbf{n}$ とすると、点 $P$ と直線の距離は

$\frac{|(\mathbf{p}-\mathbf{h})\cdot\mathbf{n}|}{|\mathbf{n}|}$

である。

### 中点

$M$ が $AB$ の中点であるとき、

$\mathbf{m}=\frac{\mathbf{a}+\mathbf{b}}{2}$

となる。

### 内分点

$AP:PB=m:n$ のとき、

$\mathbf{p}=\frac{n\mathbf{a}+m\mathbf{b}}{m+n}$

となる。

### 外分点

$AP:PB=m:n$ のとき、

$\mathbf{p}=\frac{-n\mathbf{a}+m\mathbf{b}}{m-n}$

となる。

---

## 3. 三角形

### 重心

三角形 $ABC$ の重心を $G$ とすると、

$\mathbf{g}=\frac{\mathbf{a}+\mathbf{b}+\mathbf{c}}{3}$

となる。

### 面積

三角形 $ABC$ の面積を $S$ とする。

$\angle BAC=\theta$ とすると、

$S=\frac{1}{2}|AB||AC|\sin\theta$

である。

また、内積を利用すると、

$S^2=\frac{1}{4}\left(|AB|^2|AC|^2-(\overrightarrow{AB}\cdot\overrightarrow{AC})^2\right)$

となる。

---

## 4. 円

中心を $C$、半径を $r$ とする円上の点を $X$ とすると、

$|X-C|=r$

である。

---

## 5. 垂直二等分線

点 $P$ が線分 $AB$ の垂直二等分線上にあることと、

$|PA|=|PB|$

は同値である。

---

## 6. 共線条件

3 点 $A,B,C$ が一直線上にあるための条件は、

$\overrightarrow{AC}=k\overrightarrow{AB}$

を満たす実数 $k$ が存在することである。

位置ベクトルを用いれば、

$\mathbf{c}-\mathbf{a}=k(\mathbf{b}-\mathbf{a})$

となる。

---

## 7. 平行四辺形

四角形 $ABCD$ が平行四辺形であるとき、

$\mathbf{a}+\mathbf{c}=\mathbf{b}+\mathbf{d}$

が成立する。

これは、対角線の中点が一致することから得られる。

---

## 8. 垂心

三角形 $ABC$ の垂心を $H$ とする。

$AH\perp BC$ より、

$(\mathbf{h}-\mathbf{a})\cdot(\mathbf{c}-\mathbf{b})=0$

となる。

同様に、

$(\mathbf{h}-\mathbf{b})\cdot(\mathbf{a}-\mathbf{c})=0$

となる。

したがって、これらの連立方程式から垂心の位置ベクトルを求めることができる。

---

## 9. 外心

三角形 $ABC$ の外心を $P$ とする。

$PA=PB$ より、

$|\mathbf{p}-\mathbf{a}|^2=|\mathbf{p}-\mathbf{b}|^2$

である。

これを整理すると、

$2\mathbf{p}\cdot(\mathbf{b}-\mathbf{a})=|\mathbf{b}|^2-|\mathbf{a}|^2$

となる。

同様に、$PA=PC$ より、

$2\mathbf{p}\cdot(\mathbf{c}-\mathbf{a})=|\mathbf{c}|^2-|\mathbf{a}|^2$

となる。

---

## 10. 内心

三角形 $ABC$ の内心を $I$ とする。

辺の長さを

$x=|BC|,\quad y=|CA|,\quad z=|AB|$

とおく。

このとき、内心の位置ベクトルは

$\mathbf{i}=\frac{x\mathbf{a}+y\mathbf{b}+z\mathbf{c}}{x+y+z}$

で与えられる。

つまり、内心は各頂点の位置ベクトルを、対辺の長さを重みとして加重平均した点である。
