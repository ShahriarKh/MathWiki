<div class="topSpace"></div>

Date Created: 09/02/2022 09:43:00
Tags: #Type/Proposition #Topic/Set_Theory

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X_1,X_2,Y_1,Y_2$ be sets. Then
$$\begin{equation}
    \l(X_1\cap X_2\r)\times\l(Y_1\cap Y_2\r)=\l(X_1\times Y_1\r)\cap\l(X_2\times Y_2\r).
\end{equation}$$

```

<i>Proof.</i> Take $p\in\l(X_1\cap X_2\r)\times\l(Y_1\cap Y_2\r)$. The result follows from the following chain of equivalences:

$\begin{alignat}{2}
    p\in\l(X_1\cap X_2\r)\times\l(Y_1\cap Y_2\r)&\Leftrightarrow\ex x\in X_1\cap X_2,\ex y\in Y_1\cap Y_2:p=\tpl{x,y}&&\textrm{Definition of Cartesian product}\\
    &\Leftrightarrow\l(\ex x:x\in X_1\land x\in X_2\r)\land\l(\ex y:y\in Y_1\land y\in Y_2\r)\land p=\tpl{x,y}&&\textrm{Definition of intersection}\\
    &\Leftrightarrow\l(\ex x\in X_1,\ex y\in Y_1:p=\tpl{x,y}\r)\land\l(\ex x\in X_1,\ex y\in Y_2:p=\tpl{x,y}\r)\ \ \ \ \ \ \ \ &&\textrm{Idempotence and associativity of conjunction}\\
    &\Leftrightarrow p\in X_1\times Y_1\land p\in X_2\times X_y&&\textrm{Definition of Cartesian product}\\
    &\Leftrightarrow p\in\l(X_1\times Y_1\r)\cap\l(X_2\times Y_2\r).\qedin&&\textrm{Definition of intersection}
\end{alignat}$
