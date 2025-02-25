---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 08/03/2022 14:37:40
Tags: #Type/Proposition #Topic/Set_Theory

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $f:X\to Y$ and $g:Y\to Z$ and fix subsets $S\subseteq X$ and $T\subseteq Z$. Then
$$\begin{equation}
    \im_{g\circ f}\l(S\r)=\im_g\l(\im_f\l(S\r)\r)\ \ \ \ \ \ \ \ \mathit{and}\ \ \ \ \ \ \ \ \preim_{g\circ f}\l(T\r)=\preim_f\l(\preim_g\l(T\r)\r).
\end{equation}$$

```

<i>Proof.</i> Take $z\in\im_{g\circ f}\l(S\r)$. The result follows from the following chain of equivalences:
$$\begin{equation}
    \begin{aligned}
        z\in\im_{g\circ f}\l(S\r)&\Leftrightarrow z\in Z\land\ex x\in S:z=\l(g\circ f\r)\l(x\r) && \textrm{Definition of image} \\
        &\Leftrightarrow z\in Z\land\ex x\in S:z=g\l(f\l(x\r)\r) && \textrm{Definition of composition} \\
        &\Leftrightarrow z\in Z\land\ex y\in\im_f\l(S\r):z=g\l(y\r) && \textrm{Set }y\coloneqq f\l(x\r) \\
        &\Leftrightarrow z\in\im_g\l(\im_f\l(S\r)\r). && \textrm{Definition of image}       
    \end{aligned}
\end{equation}$$
Similarly, take $x\in\preim_{g\circ f}\l(T\r)$. The result follows from the following chain of equivalences:
$$\begin{align}
    x\in\preim_{g\circ f}\l(T\r)&\Leftrightarrow x\in X\land\l(g\circ f\r)\l(x\r)\in T && \textrm{Definition of preimage} \\
    &\Leftrightarrow x\in X\land g\l(f\l(x\r)\r)\in T && \textrm{Definition of composition} \\
    &\Leftrightarrow x\in X\land f\l(x\r)\in\preim_g\l(T\r) && \textrm{Definition of preimage} \\
    &\Leftrightarrow x\in\preim_f\l(\preim_f\l(T\r)\r) && \textrm{Definition of preimage}\qedin
\end{align}$$
