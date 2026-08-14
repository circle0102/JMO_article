# LTEの補題
---
$p$で $n$が何回われるかを $\nu_p(n)$とする。

任意の整数 $x,y$ 及び正整数 $n,x,y$ の素因数でない素数 $p$ について

**一般的に $\nu_p(x^n-y^n)=\nu_p(x-y)+\nu_p(n)$が成り立つ**

---
## 厳密には
任意の整数 $x,y$ 及び正整数 $n,x,y$ の素因数でない素数 $p$ について、次の主張が成立する。

$p$ が奇素数であるとき、

$x-y\equiv 0\pmod{p}$ であれば
　 $\nu_p(x^n-y^n)=\nu_p(x-y)+\nu_p(n).$

$x+y\equiv 0\pmod{p}$ かつ $n$ が奇数ならば
　 $\nu_p(x^n+y^n)=\nu_p(x+y)+\nu_p(n).$

$x+y\equiv 0\pmod{p}$ かつ $n$ が偶数ならば
　 $\nu_p(x^n+y^n)=0.$

$p$ が偶数の素数、つまり $2$ であるとき、

$x-y\equiv 0\pmod{2}$ かつ $n$ が偶数ならば
　 $\nu_2(x^n-y^n)=\nu_2(x-y)+\nu_2(x+y)+\nu_2(n)-1
=\nu_2\left(\frac{x^2-y^2}{2}\right)+\nu_2(n).$

$x-y\equiv 0\pmod{2}$ かつ $n$ が奇数ならば
　 $\nu_2(x^n-y^n)=\nu_2(x-y).$

任意の $p$ について、

$x-y\equiv 0\pmod{p}$ かつ、$n$ が $p$ で割り切れないならば
　 $\nu_p(x^n-y^n)=\nu_p(x-y).$

$x+y\equiv 0\pmod{p}$ かつ、$n$ が $p$ で割り切れないかつ、$n$ が奇数ならば
　 $\nu_p(x^n+y^n)=\nu_p(x+y).$

$p=2$ の場合の系には以下の様なものがある。

$x-y\equiv 0\pmod{4}$ で、$x,y$ がともに奇数ならば、 $ \nu_2(x+y)=1$ で、
$\nu_2(x^n-y^n)=\nu_2(x-y)+\nu_2(n).$

$x+y\equiv 0\pmod{2}$ かつ $n$ が偶数のとき、
　 $\nu_2(x^n+y^n)=1.$
  
$x+y\equiv 0\pmod{2}$ かつ $n$ が奇数のとき、
　 $\nu_2(x^n+y^n)=\nu_2(x+y).$
