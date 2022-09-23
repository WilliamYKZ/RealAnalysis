# Homework 3

## Question 1

Consider $y\in(X\backslash \bar{B}_\varepsilon(x))$. Since $d(x,y)>\varepsilon$, Then $\delta=d(x,y)-\varepsilon>0$. 
$$
\begin{align}
0<\delta-d(y,m)\\&=d(x,y)-\varepsilon -d(y,m)\\&\le d(x,m)-\varepsilon

\end{align}
$$
$\forall m\in B_\delta(y)$ there will have $B_\delta(y\subseteq X\backslash\bar{B}_\varepsilon(x) )$. Then we can know $m\in (X\backslash\bar{B}_\varepsilon(x))$. Then $X\backslash\bar{B}_\varepsilon(x)$ is open. Then $\bar{B}_\varepsilon(x)$ is closed. 

<div style="page-break-after: always;"></div>

## Question 2

Consider $x_{m}\in Lim(x_n)$, we can know there exists $n_j,x_m=Lim_jx_nj$. Since $(x_{nj})$ is convergent subsequence. When $x=\lim _{n \rightarrow \infty} x_{m}$, There exists $m,x=Lim_jx_m$. We can conclude that $x\in Lim(x_n)$. Thus $Lim(x_n)$ is closed.



<div style="page-break-after: always;"></div>

## Question 3

**Idea From Tianyue Cao**

Consider $\left\{\left(x_n, y_n\right)\right\}_1^{\infty}$ be an arbitrary Cauchy sequence that converges to a point $(x,y)$. There will be two cases, when $f(x)<0$ or $g(y)<f(x)$. 

- Case 1:When $f(x)<0$. 

  Consider $\varepsilon=-f(x)>0$. We can know $\lim _{n \rightarrow \infty} f\left(x_n\right)=f(x)$. By definition of limit, There will exists $N$ such that $\forall n >N$.
  $$
  |f(x_n)-f(x)|<\varepsilon\\
  f(x_n)<f(x)+\varepsilon=0
  $$
  Since $(x_n,y_n)\in \{(x, y) \mid 0 \leq f(x) \leq g(y)\}$, we have $f(x_n)\le 0$, which is a contradiction.

- Case 2: When $g(y)<f(x)$.

  Since both $f$ and $g$ are continuous, we can know $\lim _{n \rightarrow \infty} f\left(x_n\right)=f(x)$ and the $\lim _{n \rightarrow \infty} g\left(y_n\right)=g(y)$. By the definiton of limit, 

  - There will exists $N_x$ such that for all $m>N_x$, We can know $\left|f\left(x_m\right)-f(x)\right|<\frac{\epsilon}{2}$. Then we can know $f\left(x_m\right)<f(x)+\frac{\epsilon}{2}$.

  - There will exists $N_y$ such that for all $m> N_y$, We can know $\left|g\left(y_m\right)-g(y)\right|<\frac{\epsilon}{2}$. Then we can know $g\left(y_m\right)>g(y)-\frac{\epsilon}{2}$.

  Then we can know $g\left(y_n\right)>g(y)-\frac{\epsilon}{2}=f(x)+\epsilon-\frac{\epsilon}{2}=f(x)+\frac{\epsilon}{2}>f\left(x_n\right)$. Since $m>max\{N_x,N_y\}$.

  Then there will have a contradiction. Since, $(x_m,y_m)\in \{(x, y) \mid 0 \leq f(x) \leq g(y)\}$, We will have $f(x_n)\le g(x_n)$.

Then we can know $0 \leq f(x) \leq g(y)$ implies that $(x,y)\in \{(x, y) \mid 0 \leq f(x) \leq g(y)\}$ .  We show all cauchy sequences in $\{(x, y) \mid 0 \leq f(x) \leq g(y)\}$ converge to a point in $\{(x, y) \mid 0 \leq f(x) \leq g(y)\}$. Thus it is closed. 





<div style="page-break-after: always;"></div>

## Question 4

($\Rightarrow$) We know that $S$ is oper under $d(x,y)$, Thus it will also open under $d_f(x,y)$. and the $f$ is strictly increasing. Consider $\forall x \in S$, $B_\varepsilon(x)\subseteq S$.
$$
\begin{align}
d(x,y)<\varepsilon &\Rightarrow y\in S\\
x-\varepsilon<y<x+\varepsilon&\Rightarrow y\in S \tag{1}\\
a<b &\Leftrightarrow f(a)<f(b) \tag{2}
\end{align}
$$
Since we know that $S$ is also open under $d_f(x,y)$. we can combine two equation.
$$
f(x-\varepsilon)<f(y)<f(x+\varepsilon) \Rightarrow y\in S
$$
Consider $m=f(x+\varepsilon)-f(x)>0$, and $n=f(x)-f(x-\varepsilon)>0$.
$$
\begin{align}

d_f(x,y)<min\{m,n\} \\
&\Rightarrow -m<f(x)-f(y)<n\\
&\Rightarrow f(x)-f(x+\varepsilon)<f(x)-f(y)<f(x)-f(x-\varepsilon)\\
&\Rightarrow f(x-\varepsilon)<f(y)<f(x+\varepsilon)\\
&\Rightarrow y\in S


\end{align}
$$
($\Leftarrow$): We know $f^{-1}$ is also increasing and continuous. By the prove above we can know $S$ is opern under $d_f(x,y)=|f(x)-f(y)|$, Then $S$ is open under $(d_f)_{f^{-1}}(x,y)=\left|f^{-1}(f(x))-f^{-1}(f(y))\right| = d(x,y)$.

Thus by conclusion, we know the statement is true.





