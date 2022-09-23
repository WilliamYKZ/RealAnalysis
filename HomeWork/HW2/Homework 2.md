# Homework 2

## Question 1

$\mathbb{N}$ is not bounded. 

Consider the $\mathbb{N}$ is bounded, then we can find a supremum $\alpha\in \mathbb{Z}$, and since $\alpha-1<\alpha$. $\alpha -1$ will not be upperbound of $\mathbb{N}$. 

Then we can find
$$
\beta > \alpha -1 \quad \beta\in \mathbb{N}\\
\Rightarrow \beta+1>\alpha
$$
Since $1,\beta \in \mathbb{N}$, $\beta+1\in \mathbb{N}$. Then we find a contradiction. Thus $\mathbb{N}$ is not bounded.



## Question 2

Again, we can prove by contradiction.

Consider that $a>b$. and we know $\mathbb{N}$ is not bounded. We can know there exist $\alpha \in \mathbb{N}\and \alpha >N$ such that 
$$
a\le b +\frac{1}{\alpha}<b+(a-b)=a
$$
Then we find a contradiction. Thus $a\le b$.



## Question 3

Again, we can prove by contradiction.

Since $(x_n)$ is a convergent sequence, consider the it have a limit $x$, where $x>b$. There exists a positive number $\alpha$, where $\alpha=x-b>0$. 

Since, $a\le x_n\le b$, it cannot have $|x_n-x|<\alpha$, where $n\in \mathbb{N}$. Which is a contradiction, and thus $a\le x\le b$.





## Question 4

(The Idea is From Tianyue Cao)

Clearly, all monotone function $f:\mathbb{N}\rightarrow \mathbb{N}$ without upperbound and the fucntion is increasing. So in this question we need to prove there exists a monotone function $g: \mathbb{N}\rightarrow \mathbb{N}$ with $y=lim_{m\rightarrow\infin }x_{g(m)}$.

Consider for all $m\in \mathbb{N}$, there have a $g(m)$, where $|y_m-x_{g(m)}|<|y-y_m|$. Now we will use induction. 

- Base Case: Since $\left\{x_{f_1(n)}\right\}_1^{\infty}$ converges to $y_1$. 

$$
\left|y_1-x_{f_1(n)}\right|<\left|y-y_1\right|
$$

​		Where $N\in \mathbb{N}\and n\ge N$. Thus $g(1)=f_1(N)$.

- Induction Hypothesis: Assume when $\alpha < k$, from $g(1)$ to $g(\alpha)$ is increasing function and all follow $\left|y_m-x_{f_m(n)}\right|<\left|y-y_m\right|$.

- Induction Case:

​		Since $\left\{x_{f_1(n)}\right\}_1^{\infty}$ converges to $y_{k+1}$, There will have
$$
\left|y_{k+1}-x_{f_{k+1}(n)}\right|<\left|y-y_{k+1}\right|
$$
​		Where $N_{new}\in \mathbb{N}\and n\ge N_{new}$. 

​		Since $f_{k+1}$ is monotone increasing and unbounded above, 
$$
f_{k+1}(n)>g(k)+1
$$
​		Where $N_{new2}\in \mathbb{N}\and n>N_{new2}$. 

​		Consider, $g(k+1)=f_{k+1}(N)$, where $N = max\{N_{new1},N_{new2}\}$.
$$
g(k+1)>g(k)
$$
​		Thus we can know the construction $g$ is a monotone increasing.



​		Also, we can know 
$$
\left|y_{k+1}-x_{g(k+1)}\right|<\left|y-y_{k+1}\right|
$$
​		Thus we can know the construction $g$ is also follow $\left|y_m-x_{g(m)}\right|<\left|y-y_m\right|$. 

Now we start to prove,for all $\varepsilon > 0$ $y=\lim _{m\rightarrow \infty} x_{g(m)}$, There exists $N_{new3}\in N$ s.t. $\left|y-y_{N_{new3}}\right|<\frac{\epsilon}{2}$
$$
\left|y-x_{g(N_{new3})}\right| \leq\left|y-y_{N_{new3}}\right|+\left|y_{N_{new3}}-x_{g(N_{new3})}\right| \leq 2\left|y-y_{N_{new3}}\right|
$$
Where is less that $\varepsilon $ . And by conclusion $y=\lim _{m \rightarrow \infty} x_{g(m)}$ for $\varepsilon > 0$.

Thus we can know $y\in Lim(X_n)$.



## Question 5

Consider $s_n$ is a convergent sequence, and $lims_n = s$. Then consider $\varepsilon = 1$. $n>N$ and it implies $|s_n-s|< 1$. By the triangle inequality, we can know $|s_n|-|s|<1 = |s_n|<|s|+1$.

Consider $M=max\{|s|+s,|s_1|,...,|s_N|\}$. we will get $|s_n|\le M$ for all $n\in N$. 

Which implies convergent sequence is bounded. 

