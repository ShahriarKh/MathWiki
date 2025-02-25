---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 08/01/2023 22:36:26
Tags: #Type/Theorem #Topic/Ring_Theory #Courses/MATH457

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Theorem
title: Theorem (Hilbert’s Basis Theorem).

Let $R$ be a commutative ring. If $R$ is Noetherian, then $R\l[x\r]$ is also Noetherian.

```

<i>Proof.</i> Suppose, for sake of contradiction, that there exists an ideal $I$ of $R\l[x\r]$ that is not finitely-generated. Clearly $I\neq\sring{0}$, so choose $0\neq f_0\in I$ of minimal degree. Since $I$ is not finitely-generated, we can inductively choose $f_n\in I\comp\sring{f_0,\dots,f_{n-1}}$ of minimal degree. Note that $\deg f_0\leq\deg f_1\leq\cdots$. Set $d_n\coloneqq\deg f_n$ and let $a_n$ be the leading coefficient of $f_n$. Since $R$ is Noetherian, the chain $\sring{a_0}\subseteq\sring{a_0,a_1}\subseteq\cdots$ stabilizes, so there exists some $n\in\N$ such that $a_{n+1}\in\sring{a_0,\dots,a_n}$ and hence $a_{n+1}=\sum_{i=0}^{n}r_ia_i$ for some $r_0,\dots,r_n\in R$. Consider the polynomial
$$\begin{equation}
    g\l(x\r)\coloneqq f_{n+1}\l(x\r)-\sum_{j=0}^{n}r_jx^{d_{n+1}-d_k}f_j\l(x\r).
\end{equation}$$
Since $f_{n+1}\neq\sring{f_0,\dots,f_n}$, we see that $g\not\in\sring{f_0,\dots,f_n}$. However, observe that
$$\begin{equation}
    g\l(x\r)=\underbrace{a_{n+1}x^{d_{n+1}}+\cdots}_{\mathclap{f_{n+1}}}-\sum_{j=0}^{n}r_jx^{d_{n+1}-d_j}\underbrace{\l(a_jx^{d_j}+\cdots\r)}_{\mathclap{f_j}}=\l(a_{n-1}-\sum_{j=0}^{n}r_ja_j\r)x^{d_{n+1}}+\cdots=0x^{d_{n+1}}+\cdots,
\end{equation}$$
so $\deg g<\deg f_{n+1}$. This contradicts the minimality of $\deg f_{n+1}$.<span style="float:right;">$\blacksquare$</span>
