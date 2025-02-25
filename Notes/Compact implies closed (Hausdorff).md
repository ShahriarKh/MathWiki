---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 28/12/2022 20:34:09
Tags: #Type/Proposition #Topic/Topology

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a Hausdorff space and consider a subspace $Y\subseteq X$. If $Y$ is compact, then it is closed.

```

<i>Proof.</i> If $Y=X$, we are done. Otherwise, let $p\in X\comp Y$; we shall show that $X\comp Y$ is open by finding some open neighborhood $U$ of $p$ such that $U\subseteq X\comp Y$.
* Indeed, for all $q\in Y$, let $U_q$ and $V_q$ be disjoint neighborhoods of $p$ and $q$, respectively.

Observe then that $Y\subseteq\bigcup_{q\in Y}V_q$, and since $Y$ is compact, there exist finitely-many points $q_i$ such that $Y\subseteq\bigcup_{i=1}^nV_{q_i}$. But since each $U_{q_i}\cap V_{q_i}=\em$, the intersection $U\coloneqq\bigcap_{i=1}^nU_{q_i}$ is disjoint from each $V_{q_i}$, and is hence disjoint from $Y$. Thus $U\subseteq X\comp Y$ is a neighborhood of $p$, so we are done.<span style="float:right;">$\blacksquare$</span>
