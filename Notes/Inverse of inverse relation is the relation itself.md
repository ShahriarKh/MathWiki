<div class="topSpace"></div>

Date Created: 22/01/2022 09:43:31
Tags: #Type/Proposition #Later/Set_Theory

Proved by: [[Inverse of a relation is a relation]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R$ be a binary relation. Then $\l(R^{-1}\r)^{-1}=R$.

```

<i>Proof.</i> By definition, we have $R^{-1}=\l\{\tpl{y,x}\mid xRy\r\}$. Taking the inverse again, we have

$\begin{alignat}{2}
    \l(R^{-1}\r)^{-1}&=\l\{\tpl{x,y}\mid yR^{-1}x\r\}\\
    &=\l\{\tpl{x,y}\mid xRy\r\}\\
    &=R.\qedin
\end{alignat}$
