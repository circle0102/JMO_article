# 反射原理

反射原理（Reflection Principle）は、格子経路や確率論に現れる非常に強力な数え上げ手法である。

以下二項係数を用いるので簡単な説明

$\binom{n}{r} = {}_n \mathrm{C}_r= \frac{n!}{r!(n-r)!}$
---

## 反射原理

格子点上で

- 右へ $(1,0)$
- 上へ $(0,1)$

のみを用いて

$(0,0)\rightarrow(m,n)$

へ進む経路を考える。

右へ進む回数は $m$ 回、上へ進む回数は $n$ 回なので

$\boxed{\binom{m+n}{n}}$

通り存在する。

途中で初めて

$y=x+1$

となる点を考える。

その点までの経路を

$y=x$

について反射する。

すなわち

$(x,y)\mapsto(y,x)$

と写す。

---

## Ballot問題

$(0,0)$ から $(m,n)$ へ進む経路について

$m\ge n$

とする。

途中で一度も$y>x$とならない経路数は

$\boxed{\frac{m-n+1}{m+1}\binom{m+n}{n}}$

となる。

証明は簡単である。

全経路数は $\boxed{\binom{m+n}{n}}$

一方、

途中で一度でも $y>x$ となる経路は反射原理より
$\binom{m+n}{n-1}$
通りである。

したがって

$\binom{m+n}{n}-\binom{m+n}{n-1}=
\frac{m-n+1}{m+1}
\binom{m+n}{n}$

---

## Catalan数

特に $m=n$
の場合、

最後だけは $y=x$
へ戻ってくる経路となる。

よって

$\boxed{
\frac1{n+1}
\binom{2n}{n}
}$

となる。

これは有名な **Catalan数**

$C_n=
\frac1{n+1}
\binom{2n}{n}$

である。

---

## 上下両方に境界がある場合

今度は $m\le y\le M$
を常に満たす経路を考える。

初期位置 $(0,p)$ から $(p,q)$ への経路の総数を求める。

区間長を $L=M-m+1$
とし

$a=p-m,\qquad
b=q-m$

と置くと

求める経路数は

$\boxed{\sum_{k\in\mathbb Z}\left(\binom{n}{\frac{n+b-a+2kL}{2}}-
\binom{n}{\frac{n+b+a+2+2kL}{2}}
\right)
}$

となる。

実際には二項係数が $0$ となる項がほとんどであり、有限項だけ計算すればよい。
なお、
・添字が整数でない
・ $<0$
・ $>n$
ならその二項係数は0とみなす。

---

## 関連問題

JJMO 2026 7問目など
## 参考記事
https://www.reddit.com/r/statistics/comments/9um1fx/can_someone_explain_to_me_simple_random_walk_and/?tl=ja
