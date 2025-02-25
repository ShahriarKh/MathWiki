<div class="topSpace"></div>

Date Created: 15/11/2022 14:07:45
Tags: #Type/Proposition #Topic/Ring_Theory

Proved by: [[Basic properties of group homomorphisms]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R_1$ and $R_2$ be rings and consider a homomorphism $\phi:R_1\to R_2$. Let $S_1\subseteq R_1$ and $S_2\subseteq R_2$ be subrings. Then the following properties hold.
* (Preserves identity): If $R_1$ and $R_2$ have units, and $\phi$ is surjective, then $\phi\l(1_1\r)=1_2$.
* (Image preserve subrings): $\im_\phi\!\l(S_1\r)\subseteq R_2$ is a subring.
* (Image preserve commutativity): If $S_1$ is commutative, then $\im_\phi\!\l(S_1\r)\subseteq R_2$ is commutative.
* (Image preserve field): If $S_1$ is a field, then $\im_\phi\!\l(S_1\r)\subseteq R_2$ is either $\l\{0\r\}$ or a field.
* (Preimage preserve subrings): $\preim_\phi\!\l(S_2\r)\subseteq R_1$ is a subring.
* (Preimage preserve ideals): If $S_2\subseteq R_2$ is an ideal, then $\preim_\phi\!\l(S_2\r)\subseteq R_1$ is an ideal.

```

<b>Remark.</b>
* For the multiplicative identity, surjectivity is a necessary condition for the ring homomorphism $\phi:r\mapsto0$ does not map $1$ to $1$.
* In particular, $\im\phi\subseteq R_2$ and $\ker\phi\subseteq R_1$ are subrings, and that $\ker\phi$ is an ideal in $R_1$.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i>
* (Preserves identity): Since $\phi$ is surjective, there exists some $x\in R$ such that $\phi\l(x\r)=1_2$. Then, since $\phi$ is a ring homomorphism, we have
$$\begin{equation}
    \phi\l(x\r)=\phi\l(x\cdot1_1\r)=\phi\l(x\r)\cdot\phi\l(1_1\r)=1_2\cdot\phi\l(1_1\r)=\phi\l(1_1\r),
\end{equation}$$
so $\phi\l(1_1\r)=\phi\l(1_2\r)$.

* (Image preserve subrings): We use the Subring Test. Indeed, it suffices to show that multiplication closes in $\im_\phi\!\l(S_1\r)$, so take $r_2,r_2'\in\im_\phi\!\l(S_1\r)$. Then there exist $r_1,r_1'\in S_1$ such that $r_2=\phi\l(r_1\r)$ and $r_2'=\phi\l(r_1'\r)$, so
$$\begin{equation}
    r_2\cdot r_2'=\phi\l(r_1\r)\phi\l(r_1'\r)=\phi\l(r_1\cdot r_1'\r)\in\im_\phi\!\l(S_1\r).
\end{equation}$$
* (Image preserve commutativity): Take $r_2,r_2'\in\im_\phi\!\l(S_1\r)$, so there exist $r_1,r_1'\in S_1$ such that $r_2=\phi\l(r_1\r)$ and $r_2'=\phi\l(r_1'\r)$. Observe then that
$$\begin{equation}
    r_2\cdot r_2'=\phi\l(r_1\r)\cdot\phi\l(r_1'\r)=\phi\l(r_1\cdot r_1'\r)=\phi\l(r_1'\cdot r_1\r)=\phi\l(r_1'\r)\cdot\phi\l(r_1\r)=r_2'\cdot r_2.
\end{equation}$$
* (Image preserve field): Observe that $\im_\phi\!\l(S_1\r)$ is a commutative ring, and since $S_1$ is a field, it has a multiplicative identity $1_1\in S_1$. Observe that
$$\begin{equation}
    \phi\l(1_1\r)\cdot\phi\l(r\r)=\phi\l(1_1\cdot r\r)=\phi\l(r\r)
\end{equation}$$
for all $r\in S_1$, so $\phi\l(1_1\r)$ is the multiplicative identity of $\im_\phi\!\l(S_1\r)$. Now, take some non-zero $\phi\l(r\r)\in\im_\phi\!\l(S_1\r)$. Then, since $\phi$ is a group homomorphism, we see that $r\neq0$, lest $\phi\l(r\r)=0$. Hence it has an inverse $r^{-1}\in S_1$; we claim that $\phi\l(r\r)^{-1}=\phi\l(r^{-1}\r)$. Indeed, since $\im_\phi\!\l(S_1\r)$ is a commutative ring, the computation
$$\begin{equation}
    \phi\l(r^{-1}\r)\cdot\phi\l(r\r)=\phi\l(r^{-1}\cdot r\r)=\phi\l(1_1\r)
\end{equation}$$
suffices.
* (Preimage preserve subrings): We use the Subring Test. Indeed, it suffices to show that multiplication closes in $\preim_\phi\!\l(S_2\r)$, so take $r_1,r_1'\in\preim_\phi\!\l(S_2\r)$. Then $\phi\l(r_1\r)\in S_2$ and $\phi\l(r_1'\r)\in S_2$, so
$$\begin{equation}
    \phi\l(r_1\cdot r_1'\r)=\phi\l(r_1\r)\cdot\phi\l(r_1'\r)\in S_2.
\end{equation}$$
* (Preimage preserve ideals): Take $p\in\preim_\phi\!\l(S_2\r)$ and $r\in R_1$, so $\phi\l(p\r)\in S_2$ and hence $r_2\cdot\phi\l(p\r),\phi\l(p\r)\cdot r_2\in S_2$ for all $r_2\in R_2$. It suffices to show that $r\cdot p,p\cdot r\in\preim_\phi\!\l(S_2\r)$. Indeed, observe that
$$\begin{equation}
    \phi\l(r\cdot p\r)=\phi\l(r\r)\cdot\phi\l(p\r)\in S_2\ \ \ \ \ \ \ \ \textrm{and}\ \ \ \ \ \ \ \ \phi\l(p\cdot r\r)=\phi\l(p\r)\cdot\phi\l(r\r)\in S_2.\qedin
\end{equation}$$
