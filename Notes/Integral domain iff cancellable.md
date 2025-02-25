---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 14/11/2022 21:50:14
Tags: #Type/Proposition #Topic/Ring_Theory

Proved by: [[Basic properties of rings]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R$ be a commutative ring with unit $1\neq0$. Then $R$ is an integral domain iff
$$\begin{equation}
    \fa s,t\in R,\fa a\in R\comp\l\{0\r\}:rs=rt\Rightarrow s=t.
\end{equation}$$

```

<i>Proof.</i>
* ($\Rightarrow$): Take $s,t\in R$ and $r\in R\comp\l\{0\r\}$. If $rs=rt$, then $rs-rt=0$ and hence $r\l(s-t\r)=0$. But since $R$ is an integral domain, we see that either $r=0$ or $s-t=0$; the former case is excluded. Thus $s-t=0$, so $s=t$.
* ($\Leftarrow$): Suppose that the cancellation law holds and take $r,s\in R$ such that $rs=0$. If $r\neq0$, write $rs=r0$ so that $r=0$.<span style="float:right;">$\blacksquare$</span>
