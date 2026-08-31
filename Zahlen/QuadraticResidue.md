# 平方剰余

合同式

$x^2\equiv a\pmod p$

が解を持つかどうかについて平方剰余の相互法則を用いる。

---

## 平方剰余

$p$ を奇素数とする。

整数 $a$ が

$x^2\equiv a\pmod p$

を満たす整数 $x$ を持つとき、 $a$ を法 $p$ における平方剰余という。

解を持たないとき、 $a$ を平方非剰余という。

---

## ルジャンドル記号

$p$ を奇素数とし、$p\nmid a$ とする。

このとき、ルジャンドル記号を

$\left(\frac{a}{p}\right)=$　 $1$　 $a$ が法 $p$ の平方剰余

　　　　  $-1$　 $a$ が法 $p$ の平方非剰余

と定義する。

また、 $p\mid a$ の場合は、

$\left(\frac{a}{p}\right)=0$

と定義する。

つまり、

$\left(\frac{a}{p}\right)$

は、 $a$ が法 $p$ で平方になるかを $1,0,-1$ で表したものである。

---

## 乗法性

$\left(\frac{ab}{p}\right)=\left(\frac{a}{p}\right)\left(\frac{b}{p}\right)$

という性質がある。

例えば

$\left(\frac{30}{p}\right)$

を求めたい場合、

$\left(\frac{30}{p}\right)=
\left(\frac{2}{p}\right)
\left(\frac{3}{p}\right)
\left(\frac{5}{p}\right)$

と素因数ごとに分解できる。

---

## オイラーの判定法

$p$ を奇素数とし、 $p\nmid a$ とする。

このとき、

$a^{\frac{p-1}{2}}\equiv\left(\frac{a}{p}\right)\pmod p$

が成立する。

したがって、

$a^{\frac{p-1}{2}}\equiv1\pmod p$

なら $a$ は平方剰余、

$a^{\frac{p-1}{2}}\equiv-1\pmod p$

なら $a$ は平方非剰余である。

---

## 平方剰余の相互法則

$p,q$ を異なる奇素数とする。

このとき、

$\boxed{\left(\frac{p}{q}\right)
\left(\frac{q}{p}\right)=
(-1)^{\frac{(p-1)(q-1)}{4}}
}$

が成立する。

また、$p,q$ のどちらかが $1\pmod4$
なら、

$\left(\frac{p}{q}\right)=
\left(\frac{q}{p}\right)$

である。

一方、 $p\equiv q\equiv3\pmod4$
なら、

$\left(\frac{p}{q}\right)=
-\left(\frac{q}{p}\right)$

となる。

### 例

例えば、

$\left(\frac{3}{13}\right)$

を求める。

$13\equiv1\pmod4$ なので、

$\left(\frac{3}{13}\right)=
\left(\frac{13}{3}\right)$

である。

さらに、 $13\equiv1\pmod3$ 
なので、

$\left(\frac{13}{3}\right)=
\left(\frac{1}{3}\right)=1$

したがって、

$\boxed{\left(\frac{3}{13}\right)=1}$

である。

よって、

$x^2\equiv3\pmod{13}$

は解を持つ。

---

## 補充法則
### 第１補充法則
$\left({\frac {-1}{p}}\right)=(-1)^{\frac {p-1}{2}}$

### 第２補充法則
$\left({\frac {2}{p}}\right)=(-1)^{\frac {p^{2}-1}{8}}$

---

### $-1$ の平方剰余(第１補充法則)

$p$ を奇素数とすると、

$\boxed{
\left(\frac{-1}{p}\right)=
(-1)^{\frac{p-1}{2}}
}$

である。

したがって、
$p\equiv1\pmod4$
なら、

$\left(\frac{-1}{p}\right)=1$

である。

つまり、 $x^2≡-1 (mod p)$ を満たす $$xが存在するためには 

$p\equiv1\pmod4$ を満たす必要がある。

---

### $2$ の平方剰余(第２補充法則)

$p$ を奇素数とすると、

$\boxed{
\left(\frac{2}{p}\right)=
(-1)^{\frac{p^2-1}{8}}
}$

が成立する。

したがって、 $p\equiv1,7\pmod8$
なら、

$\left(\frac{2}{p}\right)=1$

である。

一方、 $p\equiv3,5\pmod8$
なら、

$\left(\frac{2}{p}\right)=-1$

である。

---

## ウィルソンの定理

$p$ を素数とする。

このとき、

$\boxed{(p-1)!\equiv-1\pmod p}$

が成立する。


---

## ウィルソンの定理の応用

$p$ を素数とし、$p\nmid k$ とする。$k$ の逆元を $k^{-1}$ とすると、

$\frac{(p-1)!}{k}\equiv-k^{-1}\pmod p$

となる。

特に $n^2≡-1 (mod p)$を満たすnは 

$n \equiv \pm \left(\frac{p-1}{2}\right)! \pmod p$と表される。
---

## ウィルソンの定理の証明

$p$ を素数とする。

法 $p$ で、 $1,2,\ldots,p-1$
を考える。

各 $a$ は $0$ でないので、逆元 $a^{-1}$ を持つ。

通常、
$a\not\equiv a^{-1}\pmod p$
なら、
$a$
と
$a^{-1}$
を組にすることができる。

すると、
$aa^{-1}\equiv1\pmod p$
である。

つまり、逆元が異なる元はすべて積 $1$ の組に消える。

自分自身が逆元になるのは、

$a\equiv a^{-1}\pmod p$

すなわち、

$a^2\equiv1\pmod p$

の場合である。

したがって、

$(a-1)(a+1)\equiv0\pmod p$

となる。

$p$ は素数なので、

$a\equiv1\pmod p$

または、

$a\equiv-1\pmod p$

である。

よって、$1$ と $p-1$ 以外はすべて逆元との組で消える。

したがって、

$(p-1)!
\equiv1\cdot(-1)
\equiv-1\pmod p$

となる。

