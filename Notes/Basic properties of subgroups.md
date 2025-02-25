<div class="topSpace"></div>

Date Created: 08/05/2023 13:17:19
Tags: #Type/Proposition #Topic/Group_Theory

Proved by: [[Basic properties of cosets]], [[Lagrange's Theorem]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $G$ be a group and $H,K\subgrpeq G$. Then the following basic properties hold.
* $HK\subgrpeq G$ iff $HK=KH$.
* If $H\subgrpeq N_G\!\l(K\r)$, then $HK\subgrpeq G$.
* If $H$ and $K$ are finite, then $\l|HK\r|=\l|H\r|\l|K\r|/\l|H\cap K\r|$.

```

<b>Remark.</b> Since $HK\subseteq\gen{H,K}$, we see that $\l|\gen{H,K}\r|\geq\l|H\r|\l|K\r|/\l|H\cap K\r|$.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i>
* If $HK\subgrpeq G$, then, since $H,K\subgrpeq G$, we see that $H,K\subgrpeq HK$. Thus $KH\subseteq HK$ by closure. For the reverse containment, take $hk\in HK$. Thus $hk=x^{-1}$ for some $x\in HK$, say $x=h_1k_1$. Thus $hk=x^{-1}=\l(h_1k_1\r)^{-1}=k_1^{-1}h_1^{-1}\in KH$, as desired. Conversely, suppose $HK=KH$. Clearly $e=ee\in HK$. If $h_1k_1,h_2k_2\in H_K$, then $\l(h_1k_1\r)\l(h_2k_2\r)=h_1\l(k_1h_2\r)k_2=h_1h_2'k_1'k_1\in HK$ for some $h_1'\in H$ and $k_1'\in K$. Lastly, if $hk\in HK$, then $\l(hk\r)^{-1}=k^{-1}h^{-1}=h'k'\in HK$ for some $h'\in H$ and $k'\in K$.
* It suffices to show that $HK=KH$. If $hk\in HK$, then, since $h\in N_G\!\l(K\r)$, we see that $hk=k'h\in KH$ for some $k'\in K$. Similarly if $kh\in KH$.
* First, observe that $HK=\bigcup_{h\in H}hK$ where each $hK$ has cardinality $\l|K\r|$. Thus, since $h_1K\cap h_2K=\em$ for $h_1\neq h_2$, it suffices to find the number of distinct left cosets $hK$ for $h\in H$. Observe that $h_1K=h_2K$ for $h_1,h_2\in H$ iff $h_2^{-1}h_1\in H\cap K$, which occurs iff $h_1\l(H\cap K\r)=h_2\l(H\cap K\r)$. Thus the number of distinct cosets $hK$ in $G$ coincides with that of $h\l(H\cap K\r)$ in $H$. By Lagrange’s Theorem, the latter is $\l[H:H\cap K\r]=\l|H\r|/\l|H\cap K\r|$. Thus $\l|HK\r|$, being $\l|K\r|$ times the number of distinct cosets $hK$ in $G$ for $h\in H$, is $\l|H\r|\l|K\r|/\l|H\cap K\r|$, as desired.<span style="float:right;">$\blacksquare$</span>
