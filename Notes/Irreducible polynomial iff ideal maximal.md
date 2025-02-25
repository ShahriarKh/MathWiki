---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 22/01/2023 23:31:02
Tags: #Type/Proposition #Topic/Ring_Theory #Courses/MATH457

Proved by: [[Basic properties of divisibility and associates]]
References: [[Ideal is maximal iff quotient is a field]], [[Polynomial rings over UFDs are UFDs]], [[Irreducible implies prime (UFD)]]
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $K$ be a field and let $f\in K\l[x\r]$. Then $f$ is irreducible iff the ideal $\sring{f}$ is maximal.

```

<b>Remark.</b> It follows then that $K\l[x\r]/\sring{f}$ is a field iff $f$ is irreducible. Since $K\l[x\r]$ is a UFD, this also holds iff $p$ is prime.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i> Observe that $\sring{f}$ is maximal iff $\sring{f}\not\subset\sring{g}$ for any $\sring{g}\neq R$. But this occurs iff $g\ndivides f$ for any $g\in R\comp R^\times$, iff $f$ is irreducible.<span style="float:right;">$\blacksquare$</span>
