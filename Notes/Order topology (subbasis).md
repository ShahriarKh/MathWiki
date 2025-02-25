<div class="topSpace"></div>

Date Created: 08/02/2022 12:25:47
Tags: #Type/Proposition #Later/Topology

Proved by: [[Criteria for subbasis to generate existing basis]], [[Half-infinite open rays are open in the order topology]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a set. Then the order topology $\mc{T}\l(<\r)\coloneqq\mc{T}\l(\mc{B}\r)$ on $X$ can be generated by the subbasis
$$\begin{equation}
    \mc{S}\coloneqq\l\{S\in\pow\l(X\r)\mid\l[\ex a\in X:S=\l(a,+\infty\r)\r]\lor\l[\ex b\in X:S=\l(-\infty,b\r)\r]\r\}
\end{equation}$$
containing half-infinite open rays (or bounded open rays, if they exist).

```

<i>Proof.</i> We first need to show that $\mc{S}$ is indeed a subbasis for a topology on $X$. Observe that $\mc{S}\subseteq\pow\l(X\r)$. To see that $\mc{S}$ covers $X$, take $x\in X$.
* If $x$ is not minimal in $X$, then there exists $a\in X$ such that $a<x$. Observe then that $x\in\l(a,+\infty\r)\in\mc{S}$.
* If $x$ is minimal in $X$, then, for all $b\in X$, the open ray $\l(-\infty,b\r)=\l[x,b\r)$; observe that $x\in\l[x,b\r)\in\mc{S}$.

Furthermore, recall that $\mc{S}\subseteq\mc{T}\l(\mc{B}\r)$ since half-infinite open rays are open in the order topology. It remains to show that for any $B\in\mc{B}$, there exists $\mc{R}\subseteq\mc{S}$ such that $0<\l|\mc{R}\r|<\infty$ and $B=\bigcap\mc{R}$, for then the topology generated by $\mc{S}$ is $\mc{T}\l(\mc{S}\r)=\mc{T}\l(\mc{B}\r)=\mc{T}(<
)$. Take $B\in\mc{B}$; we have three cases.
* If $B=\l(a,b\r)$ for some $a,b\in X$ with $a<b$, let $\mc{R}\coloneqq\l\{R_1,R_2\r\}\subseteq\mc{S}$ where $R_1\coloneqq\l(-\infty,b\r)$ and $R_2\coloneqq\l(a,+\infty\r)$. Observe then that $0<\l|\mc{R}\r|=2<\infty$ and that
$$\begin{equation}
    B=\bigcap\mc{R}=R_1\cap R_2=\l(-\infty,b\r)\cap\l(a,+\infty\r)=\l(a,b\r).
\end{equation}$$
Pictorially, this can be seen as:
![[Images/2022-02-09_223333/image.svg|260]]

* If there exists a minimal element $a_0\in X$ and $B=\l[a_0,b\r)$ for some $b\in X$ with $a_0<b$, then $\l[a_0,b\r)=\l(-\infty,b\r)\in\mc{S}$ and $B=\bigcap\l\{\l[a_0,b\r)\r\}$.
* If there exists a maximal element $b_0\in X$ and $B=\l(a,b_0\r]$ for some $a\in X$ with $a<b_0$, then $\l(a,b_0\r]=\l(a,+\infty\r)\in\mc{S}$ and $B=\bigcap\l\{\l(a,b_0\r]\r\}$.<span style="float:right;">$\blacksquare$</span>
