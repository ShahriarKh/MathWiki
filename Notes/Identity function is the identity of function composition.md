---
mathLink: $f\circ\id_X=f=\id_Y\circ f$
---

<div class="topSpace"></div>

Date Created: 27/12/2022 20:23:02
Tags: #Type/Proposition #Topic/Set_Theory

Proved by: [[Criteria for equality of functions]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $f:X\to Y$. Then $f\circ\id_X=f$ and $\id_Y\circ f=f$; in other words, the following diagram commutes.
![[Images/2022-02-09_213021/image.svg|240]]

```

<i>Proof.</i> Observe that
$$\begin{equation}
    \dom f=\dom\l(f\circ\id_X\r)=\dom\l(\id_Y\circ f\r)=X,
\end{equation}$$
so take $x\in X$. Compute
$$\begin{equation}
    \l(f\circ\id_X\r)\l(x\r)=f\l(\id_X\l(x\r)\r)=f\l(x\r)\ \ \ \ \textrm{and}\ \ \ \ \l(\id_Y\circ f\r)\l(x\r)=\id_X\l(f\l(x\r)\r)=f\l(x\r),
\end{equation}$$
so $f\l(x\r)=\l(f\circ\id_X\r)\l(x\r)=\l(\id_Y\circ f\r)\l(x\r)$ for all $x$ in their common domain.<span style="float:right;">$\blacksquare$</span>
