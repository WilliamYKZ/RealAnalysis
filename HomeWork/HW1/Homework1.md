# Homework1

## Question 1

From the question we know $T$ is nonempty subset, Suppose $t$ in $T$ and $g,h=t$ . Then $gh^{-1}=tt^{-1}=1$. Which show $1 \in G(T)$.

Suppose $g_1,h_1^{-1}$ in $G(T)$ and ($g_1,h_1 \ in \  T$) and $g_2,h_2^{-1}$ in $G(T)$ and ($g_2,h_2 \ in \  T$). Then we can know $g_1h_1^{-1}g_2h_2^{-1}=g_1g_2h_1^{-1}h_2^{-1}$.

Since $g_1,g_2 \in T$. $h_1^{-1}h_2^{-1} = (h_2h_1)^{-1}$ and $h_1,h_2\in T$. Then we can know $g_1g_2\in T$ and $h_2h_1\in T$. Thus $g_1h_1^{-1}g_2h_2^{-1}=g_1g_2h_1^{-1}h_2^{-1}=g_1g_2(h_2h_1)^{-1}\in G(T)$. Which we show that if $gh\in \ subgroup$.

Thus we can know $G(T)$ is a subgroup of $G$.



## Question 2

Consider $g_1,h_1,g_2,h_2\in T_1$ s.t. $g_1,h_1^{-1}=g_2h_2^{-1}$
$$
\begin{align}
\psi(g_1h_1^{-1})=\phi(g_1)\phi(h_1)^{-1}\tag{1}\\
\psi(g_2h_2^{-1})=\phi(g_2)\phi(h_2)^{-1}\tag{2}\\

\end{align}
$$
Now we need to prove (1) = (2), Since $\phi(g_1),\phi(h_1)^{-1}$ are group element. 
$$
\phi(g_1)\phi(h_1)^{-1}(\phi(g_2)\phi(h_2)^{-1})^{-1}\\
=\phi(g_1)\phi(h_1)^{-1}\phi(h_2)\phi(g_1)^{-1}\\
=\phi(g_1)\phi(h_2)\phi(h_1)^{-1}\phi(g_2)^{-1}\\
=\phi(g_1h_2)\phi(g_2h_1)^{-1}\\
=\phi(g_1h_2)\phi(g_2h_1)^{-1}\\
=1
$$
Thus we can know (1) and (2) have same inverse, thus we can say (1) = (2), and $\psi(gh^{-1})=\phi(g)\phi(h)^{-1}$ is a well-define. 



Let $g$ be an arbitrary element in $T_1$. $\psi(gg^{-1})=\psi(1)=\psi(g)\psi(g)^{-1}=1$. which is $\phi(1)=1$. 

Let $g,h$ be elements in $G(T_1)$. $g=s_1t_1^{-1}$, $h=s_2t_2^{-1}$. $s_1,t_1,s_2,t_2\in T_1$.
$$
\psi(gh)=\psi(s_1t_1^{-1}s_2t_2^{-1})\\
=\psi(s_1s_2(t_2t_1)^{-1})\\
=\phi(s_1s_2)\phi(t_2t_1)^{-1}\\
=\phi(s_1)\phi(s_2)(\phi(t_1)\phi(t_2))^{-1}\\
=\phi(s_1)\phi(s_2)\phi(t_1)^{-1}\phi(t_2)^{-1}\\
=\phi(s_1)\phi(t_1)^{-1}\phi(s_2)\phi(t_2)^{-1}\\
=\psi(s_1t_1^{-1})\psi(s_1t_2^{-1})\\
=\psi(g)\psi(h)
$$
Thus we can know it is a group homomorphism from $G(T_1)$ to $G(T_2)$.





## Question 3

Suppose $g_1,g_2,h_1,h_2\in S$ and $g_1h_2=g_2h_1$, we can find $\phi\left(g_1\right) \phi\left(h_1\right)^{-1}= \phi\left(g_2\right) \phi\left(h_2\right)^{-1} \Rightarrow \psi\left(g_1 h_1^{-1}\right)=\phi\left(g_1\right) \phi\left(h_1\right)^{-1}=\phi\left(g_2\right) \phi\left(h_2\right)^{-1}=\psi\left(g_2 h_2^{-1}\right)$ 

Thus $\psi$ is well define. 
$$
\begin{align}
\psi\left(g_1 h_1^{-1} g_2 h_2^{-1}\right)=\psi\left(\left(g_1 g_2\right)\left(h_1 h_2\right)^{-1}\right)&=\phi\left(g_1 g_2\right) \phi\left(h_1 h_2\right)\\&=\phi\left(g_1\right) \phi\left(g_2\right) \phi\left(h_1\right)^{-1} \phi\left(h_2\right)^{-1}\\
&=\psi\left(g_1 h_1^{-1}\right) \psi\left(g_2 h_2^{-1}\right)\\
&= \psi(1)=\psi\left(g g^{-1}\right)=\phi(g) \phi(g)^{-1}

\end{align}
$$
Which is equal to 1. and from
$$
\psi(s)=\psi(s \cdot 1)\\=\phi(s) \phi(1)\\=\phi(s)
$$
We can know that for all $s\in S$, $\psi(s)=\phi(s)$. Thus it is also homomorphism. 

## Question 4

Consider $g,h$ in $G(\phi_1(S))$. There exists $s_1,s_2,s_3,s_4\in S$. s.t. $g=\phi_1(s_1)\phi(s_2)^{-1}$,$h=\phi_1(s_3)\phi_1(s_4)^{-1}$. Define $\psi(\phi_1(s_1)\phi_1(s_2)^{-1})=\phi_2(s_1)\phi_2(s_2)^{-1}$. By the question 2 we know it is well define and homomorphism. 

Surjective is clearly, since each $\phi_2(s_1)\phi_2(s_2)^{-1}$ in $G(\phi_2(S))$ we can find $\psi(\phi_1(s_1)\phi_1(s_2)^{-1})$ in $G(\phi_1)(S)$
$$
\psi(\phi_1(s_1)\phi_1(s_2)^{-1}) = \psi(\phi_1(s_3)\phi_1(s_4)^{-1})
$$
We times $\psi(\phi_1(s_3)\phi_1(s_4)^{-1})^{-1}$
$$
\psi(\phi_1(s_1)\phi_1(s_2)^{-1}\phi_1(s_4)\phi_1(s_3)^{-1}=1\\
\phi_1(s_1)\phi_1(s_2)^{-1}\phi_1(s_4)\phi_1(s_3)^{-1}=1
$$

$$
\phi_1(s_1)\phi_1(s_2)^{-1}=\phi_1(s_3)\phi_1(s_4)^{-1}
$$

Thus we can know it also injective. Thus it is bijective. Since it is also homomorphism, so it is isomorphism. 





## Question 5 

Consider function $f(z):Z \rightarrow G(N)$ where 
$$
f(0 )=1\\
f(n)=\phi(n) \ for \ all \ n \ in \ N\\
f(-n) = \phi(n)^{-1} \ for \ all \ n \ in \ N
$$
$f$ is a bijection, $f(a)f(b)=f(a+b)$. For all $a,b\in Z$, $f(a+b)=f(a)+f(b)$ closure for all $a,b,c\in Z$.

$(f(a) f(b)) f(c)=f(a+b) f(c)=f(a+b+c)=f(a) f(b+c)=f(a)(f(b) f(c))$ thus we know it is closure.



$(a, b) \cdot(0,0)=(a, b)$ and $(0,0) \cdot(a, b)=(a, b)$, we can know it have indentity which is $(0,0)$. 



From $(a, b) \cdot(c, d)=(a+c, b+d)=(c+a, d+b)=(c, d)+(a, b)$, we can know that it have commutative. 



From $((a, b) \cdot(c, d)) \cdot(e, f)=(a+c, b+d) \cdot(e, f)=(a+c+e, b+d+f)=(a, b)+((c, d)+(e, f))$. we can know it also have associative. 

Since $f(a)+f(-1)=f(0)=1$, Thus $\phi(a)$ and $\phi(-a)$ is inverse.

$f(a)f(b)=f(a+b)=f(b+a)=f(b)f(a)$, thus it also follow abelian property. 

Thus we can know the right hand side can be made into an abelian group. Thus we prove that it is a disjoint decomposition.  