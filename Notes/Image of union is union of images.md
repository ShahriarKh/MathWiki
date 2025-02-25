<div class="topSpace"></div>

Date Created: 28/01/2022 13:28:47
Tags: #Type/Proposition #Topic/Set_Theory

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R$ be a binary relation and fix $\mc{A}\subseteq\pow\l(\dom R\r)$; that is, fix a collection of subsets of $\dom R$. Then
$$\begin{equation}
    \im_R\l(\bigcup\mc{A}\r)=\bigcup\l\{\im_R\l(A\r)\mid A\in\mc{A}\r\}.
\end{equation}$$

```

<b>Remark.</b> If $\mc{A}=\l\{A,B\r\}$, then the above reads $\im_R\!\l(A\cup B\r)=\im_R\!\l(A\r)\cup\im_R\!\l(B\r)$.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i> Take $y\in\im_R\l(\bigcup\mc{A}\r)$. The result follows from the following chain of equivalences:

$\begin{alignat}{2}
    y\in\im_R\l(\bigcup\mc{A}\r)&\Leftrightarrow y\in\ran\l(R\rest\bigcup\mc{A}\r)&&\textrm{Definition of image}\\
    &\Leftrightarrow\ex x:\tpl{x,y}\in R\rest\l(\bigcup\mc{A}\r)&&\textrm{Definition of range}\\
    &\Leftrightarrow\ex x:\tpl{x,y}\in R\land x\in\bigcup\mc{A}&&\textrm{Definition of restriction}\\
    &\Leftrightarrow\ex x:\tpl{x,y}\in R\land\l(\ex A\in\mc{A}:x\in A\r)\ \ \ \ \ \ \ \ &&\textrm{Definition of union}\\
    &\Leftrightarrow\ex x,\ex A\in\mc{A}:\tpl{x,y}\in R\land x\in A&&A\textrm{ not free in }\tpl{x,y}\in R\\
    &\Leftrightarrow\ex A\in\mc{A},\ex x:\tpl{x,y}\in R\land x\in A&&\textrm{Like quantifiers commute}\\
    &\Leftrightarrow\ex A\in\mc{A},\ex x:\tpl{x,y}\in R\rest A&&\textrm{Definition of restriction}\\
    &\Leftrightarrow\ex A\in\mc{A}:y\in\ran\l(R\rest A\r)&&\textrm{Definition of range}\\
    &\Leftrightarrow\ex A\in\mc{A}:y\in\im_R\l(A\r)&&\textrm{Definition of image}\\
    &\Leftrightarrow y\in\bigcup\l\{\im_R\l(A\r)\mid A\in\mc{A}\r\}.&&\textrm{Definition of union}\qedin
\end{alignat}$
