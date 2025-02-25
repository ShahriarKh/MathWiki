---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 07/02/2022 16:26:29
Tags: #Type/Definition #Later/Topology

Types: <i>Not Applicable</i>
Examples: <i>Not Applicable</i>
Constructions: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>
Justifications: _Not Appicable_

``` ad-Definition
title: Definition.

Let $\tpl{\N,<}$ be the set of natural numbers equipped with its standard order and consider the lexicographical order $<_L$ on $\N^2$. The <b>lexicographical order topology on $\N^2$</b> is the order topology $\mc{T}\l(<_L\r)\coloneqq\mc{T}\l(\mc{B}\r)$ generated by the basis $\mc{B}\coloneqq\mc{B}_1\cup\mc{B}_2$ where
$$\begin{equation}
    \mc{B}_1\coloneqq\l\{B\in\pow\l(\N^2\r)\mid\ex a,b,c,d\in\N:\tpl{a,b}<_L\tpl{c,d}\land B=\l(\tpl{a,b},\tpl{c,d}\r)\r\}
\end{equation}$$
containing all open intervals in $\tpl{\N^2,<_L}$, and
$$\begin{equation}
    \mc{B_2}\coloneqq\l\{B\in\pow\l(\N^2\r)\mid\ex a,b\in\N:B=\l[\tpl{0,0},\tpl{a,b}\r)\r\}
\end{equation}$$
containing all bounded open rays in $\tpl{\N^2,<_L}$.

```
