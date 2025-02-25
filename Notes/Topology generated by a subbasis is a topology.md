<div class="topSpace"></div>

Date Created: 24/01/2022 21:00:06
Tags: #Type/Proposition #Later/Topology

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a set and $\mc{S}$ be a subbasis for a topology on $X$. Then the topology generated by $\mc{S}$, $\mc{T}\l(\mc{S}\r)=\mc{T}\l(\mc{B}\r)$ where
$$\begin{equation}
    \mc{B}=\l\{B\in\pow\l(X\r)\mid\ex\mc{R}\subseteq\mc{S}:0<\l|\mc{R}\r|<\infty\land B=\bigcap\mc{R}\r\},
\end{equation}$$
is a topology on $X$.

```

<i>Proof.</i> It suffices to show that $\mc{B}$ is, in fact, a basis for a topology on $X$.
* ($\axibasis[1]$): Take $x\in X$ so, because $\mc{S}$ covers $X$, there exists $S\in\mc{S}$ such that $x\in S$. Set $\mc{R}\coloneqq\l\{S\r\}$, so there exists $B\in\mc{B}$ such that $B=\bigcap\l\{S\r\}=S$. Thus $X\subseteq\bigcup\mc{B}$, so $\mc{B}$ covers $X$.

* ($\axibasis[2]$): Now let $B_1=\bigcap\mc{R}_1$ and $B_2=\bigcap\mc{R}_2$. Take
$$\begin{equation}
    x\in\bigcap\mc{R}_1\cap\bigcap\mc{R}_2=\bigcap\l(\mc{R}_1\cup\mc{R}_2\r),
\end{equation}$$
and since the union of finite sets is finite, set $B_3\coloneqq\bigcap\l(\mc{R}_1\cup\mc{R}_2\r)\in\mc{B}$.<span style="float:right;">$\blacksquare$</span>
