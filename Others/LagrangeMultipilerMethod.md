# ラグランジュの未定乗数法定理

## 定義

目的関数 $f(x,y,\ldots)$ と制約関数 $g_1(x,y,\ldots),g_2(x,y,\ldots),\ldots$ を考える。

制約条件を

$g_1=g_2=\cdots=0$

とする。

このとき、ラグランジアンを

$L(\lambda,\mu,\ldots,x,y,\ldots)=f-\lambda g_1-\mu g_2-\cdots$

と定義する。

目的関数の極値は、以下の方程式を解くことで求められる。

$\frac{\partial L}{\partial x}=\frac{\partial L}{\partial y}=\cdots=\frac{\partial L}{\partial \lambda}=\frac{\partial L}{\partial \mu}=\cdots=0$

ここで、 $\frac{\partial L}{\partial x}$ は $L$ に対する $x$ についての偏微分である。

偏微分を行う際には、微分する変数以外の変数は定数として扱う。

例えば、

$x^2y+xz+y^2z$

を $x$ について偏微分すると、

$2xy+z$

となる。

このとき、$y,z$ は定数として扱っている。

---

## 具体例

$x+y+z=10$、 $xy+yz+zx=25$ を満たすとき、 $xyz$ の極値を求める。

### 目的関数と制約条件

目的関数を

$f(x,y,z)=xyz$

とする。

制約関数を

$g_1(x,y,z)=x+y+z-10$

$g_2(x,y,z)=xy+yz+zx-25$

とおく。

したがって、ラグランジアンは

$L(\lambda,\mu,x,y,z)=xyz-\lambda(x+y+z-10)-\mu(xy+yz+zx-25)$

となる。

---

## 偏微分

まず、 $x,y,z$ について偏微分する。

$\frac{\partial L}{\partial x}=yz-\lambda-\mu(y+z)=0$

$\frac{\partial L}{\partial y}=zx-\lambda-\mu(x+z)=0$

$\frac{\partial L}{\partial z}=xy-\lambda-\mu(x+y)=0$

また、 $\lambda,\mu$ について偏微分すると、

$\frac{\partial L}{\partial \lambda}=-(x+y+z-10)=0$

$\frac{\partial L}{\partial \mu}=-(xy+yz+zx-25)=0$

となる。

これはもとの制約条件

$x+y+z=10$

$xy+yz+zx=25$

そのものである。

---

## 対称性の利用

ここで、 $x,y,z$ は対称な形で現れている。

そのため、極値を与える点では、2 つの変数が等しくなる場合を考えることができる。

そこで、

$x=y=a,\quad z=b$

とおく。

制約条件から、

$2a+b=10$

$a^2+2ab=25$

を得る。

最初の式から、

$b=10-2a$

である。

これを2つ目の式に代入すると、

$a^2+2a(10-2a)=25$

となる。

整理すると、

$3a^2-20a+25=0$

である。

よって、

$a=\frac{5}{3},\quad 5$

となる。

---

## 5. $b$ の値を求める

$a=\frac{5}{3}$ のとき、

$b=10-2\cdot\frac{5}{3}=\frac{20}{3}$

である。

したがって、

$(x,y,z)=\left(\frac{5}{3},\frac{5}{3},\frac{20}{3}\right)$

が得られる。

一方、 $a=5$ のとき、

$b=10-2\cdot5=0$

なので、

$(x,y,z)=(5,5,0)$

が得られる。

$x,y,z$ は対称なので、これらの値を入れ替えた点も候補となる。

---

$(x,y,z)=\left(\frac{5}{3},\frac{5}{3},\frac{20}{3}\right)$

のとき、

$xyz=\frac{5}{3}\cdot\frac{5}{3}\cdot\frac{20}{3}=\frac{500}{27}$

である。

一方、

$(x,y,z)=(5,5,0)$

のとき、

$xyz=0$

である。

したがって、

$f_{\max}=\frac{500}{27}$

$f_{\min}=0$

となる。

---

特に、目的関数や制約条件に対称性がある場合は、変数のいくつかが等しいと仮定することで計算を大幅に簡略化できる。

今回の例では、 $x,y,z$ の対称性から $x=y=a$ とおくことで、3変数の問題を1変数の二次方程式へ帰着させることができた。

## 注意事項
>
> ラグランジュの未定乗数法は基本的に等式制約を扱う方法である。不等式制約を扱う場合には、KKT 条件などへ拡張する必要がある。
