---
mathLink: $I$ prime $\Leftrightarrow$ $R/I$ integral domain
---

<div class="topSpace"></div>

Date Created: 22/11/2022 19:23:49
Tags: #Type/Proposition #Topic/Ring_Theory

Proved by: [[Basic properties of cosets]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R$ be a commutative ring with unit and let $I\subset R$ be a proper ideal. Then $I$ is prime iff $R/I$ is an integral domain.

```

<i>Proof.</i> Since $R$ is a commutative ring with unit, we see that $R/I$ is also a commutative ring with unit.
* ($\Rightarrow$): Take $r+I,s+I\in R/I$ such that $\l(r+I\r)\l(s+I\r)=0+I$. Then $rs+I=0+I$, so $rs\in I$. But $I$ is prime, so either $r\in I$ or $s\in I$. Thus either $r+I=0+I$ or $s+I=0+I$.

* ($\Leftarrow$) Take $r,s\in I$ such that $rs\in I$. Then $rs+I=0+I$, so $\l(r+I\r)\l(s+I\r)=0+I$. But $R/I$ is an integral domain, so either $r+I=0+I$ or $s+I=0+I$. Thus either $r\in I$ or $s\in I$.<span style="float:right;">$\blacksquare$</span>
