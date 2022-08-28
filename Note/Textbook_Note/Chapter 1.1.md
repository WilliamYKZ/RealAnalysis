# Chapter 1.1

## The Set $\mathbb{N}$ of Natural Numbers

1. we denote the set $\{1,2,3,...\}$ of all **positive integers** by $\mathbb{N}$. Each positive integer $n$ has a **successor**, namely $n+1$. Thus the successor of 2 is 3. 

   

2. **Peano Axioms**: most familiar properties of $\mathbb{N}$ can be proved based on these five axioms.

   - **N1:**  1 belong to $\mathbb{N}$
   - **N2:** if $n$ belongs to $\mathbb{N}$, then its successor $n+1$ belongs to $\mathbb{N}$.
   - **N3:** 1 is not the successor of any element in $\mathbb{N}$.
   - **N4:** if $n$ and $m$ in $\mathbb{N}$ have the same successor, then $n=m$.
   - **N5:** A subset of $\mathbb{N}$ which contains 1, and which contains $n+1$ whenever it contains $n$, must equal $\mathbb{N}$.

Now let us prove **N5**. First we assume axiom N5 is false. Then $\mathbb{N}$ contains a set $S$ such that

(i) $1 \in S$

(ii) if $n\in S$, then $n+1\in S$

Since $S\neq \mathbb{N}$. Consider the smallest member of the set $\{n\in \mathbb{N}: n\notin S\},$ call it $n_0$. Since (i) holds, it is clear $n_0 \neq 1$. So $n_0$ is a successor to some number in $\mathbb{N}$, namely $n_0-1$. We have $n_0-1 \in S$, since $n_0$ is the smallest member of $\{n\in \mathbb{N}: n\notin S\}.$ By the (ii), the successor of $n_0-1$, namely $n_0$ is also in $S$, which is a contradiction.



3. Mathematical induction
   - $P_1$ is true.
   - $P_{n+1}$ is true whenever $P_n$ is true.

### Example 1

Prove $1+2+...+n=\frac{1}{2}n(n+1)$ for positive integers $n.$

Solution: Base Case 

$P_1$ asserts since $1= \frac{1}{2}\cdot 1(1+1)$. 

Induction Step: Suppose $P_n$ is true, and we know $1+2+...+n=\frac{1}{2}n(n+1)$, and now we want to prove $P_{n+1}$ is true.
$$
\begin{align}
1+2+...+n+(n+1)&= \frac{1}{2}n(n+1)+(n+1)\\
&=\frac{1}{2}[n(n+1)+2(n+1)]\\
&=\frac{1}{2}(n+1)(n+2)\\
&=\frac{1}{2}(n+1)((n+1)+1)
\end{align}
$$
Thus $P_{n+1}$ holds if $P_n$ holds. By the induction, we conclude $P_n$ is true for all $n$.



### Example 2

All number of the form $5^n-4n-1$ are divisible by 16.

Solution: Base Case

When $P_1$, since $5^1-4\cdot1-1=0$. it is clearly true. 

Induction Step: Suppose $P_n$ is true. now we need to verify $P_{n+1}$, is true.
$$
5^{n+1}-4(n+1)-1=5\left(5^{n}-4 n-1\right)+16 n
$$
Since $\left(5^{n}-4 n-1\right)$ is a multiple of 16 by the induction hypothesis. thus  $5^{n+1}-4(n+1)-1$ is also multiple of 16. Thus we prooved the statement. 



