# Chapter 1.2

## Basic Notation

1. $\mathbb{Z}$ as integers, that is $\{0,1,-2,2,-2,...\}$.



2. $\mathbb{Q}$ as rational numbers, number form $\frac{m}{n}$, where $m,n\in \mathbb{Z}$ and $n\neq 0$. The space $\mathbb{Q}$ is a highly satisfactory algebraic system in whcih the basic operations addition, multiplication, subtraction and division canbe fully studied. 



3. The set $\mathbb{Q}$ of rational number is a very nice algebraic system until one tries to solve equation like $x^2=2$. That no rational number satisfies this equation. 



4. Definition: A number if called an algebraic number if it satifies a polynomial equation.

$$
c_{n} x^{n}+c_{n-1} x^{n-1}+\cdots+c_{1} x+c_{0}=0
$$

Where the coefficients $c_0,c_1,...,c_n$ are integers, $c_n\neq 0$ and $n\ge 1$. 



### Example 1

(1) $\frac{4}{17}$ is algebraic numbers. Since $\frac{4}{17}$ is a solution of $17x-4=0$.

(2) $\sqrt{3}$ is algebraic numbers. SInce $\sqrt{3}$ is a solution of $x^3-3=0$.



## Rational Zeros Theorem

Suppose $c_0,c_1,...,c_n$ are integers and $r$ is a rational number satisfying the polynomial equation.
$$
c_{n} x^{n}+c_{n-1} x^{n-1}+\cdots+c_{1} x+c_{0}=0
$$
Where $n\ge 1, c_n\neq 0, c_0\neq 0$. Let $r=\frac{c}{d}$ where $c,d$ are integers having no common factors and $d\neq 0$. Then $c$ divides $c_0$ and $d$ divides $c_n$.

In other words, the only rational candidated for solutions of have the form $\frac{c}{d}$ where $c$ divides $c_0$ and $d$ divides $c_n$.



### Proof:

We are given:
$$
c_{n}\left(\frac{c}{d}\right)^{n}+c_{n-1}\left(\frac{c}{d}\right)^{n-1}+\cdots+c_{1}\left(\frac{c}{d}\right)+c_{0}=0 .
$$
We multiply through by $d^n$ and obtain.
$$
c_{n} c^{n}+c_{n-1} c^{n-1} d+c_{n-2} c^{n-2} d^{2}+\cdots+c_{2} c^{2} d^{n-2}+c_{1} c d^{n-1}+c_{0} d^{n}=0
$$
If we solve for $c_0d^n$, we obtain
$$
c_{0} d^{n}=-c\left[c_{n} c^{n-1}+c_{n-1} c^{n-2} d+c_{n-2} c^{n-3} d^{2}+\cdots+c_{2} c d^{n-2}+c_{1} d^{n-1}\right]
$$
It follows that $c$ divides $c_0d^n$. But $c$ and $d^n$ have no common factors, so $c$ divides $c_0$. But $c$ and $d$ have no common factors, so $c$ divides $c_0$. (Theis follow from the basic fact that if an integer $c$ divides a product $ab$ of integers, and if $c$ and $b$ have no common factors, then $c$ divides $a$.)

Similarity, we can use same we to prove for $d$.
$$
c_{n} c^{n}=-d\left[c_{n-1} c^{n-1}+c_{n-2} c^{n-2} d+\cdots+c_{2} c^{2} d^{n-3}+c_{1} c d^{n-2}+c_{0} d^{n-1}\right]
$$
Thus $d$ divides $c_nc^n$. Since $c^n$ and $d$ have no common factors, $d$ divides $c_n$.



## Corollary

Consider the polynomial equation
$$
x^{n}+c_{n-1} x^{n-1}+\cdots+c_{1} x+c_{0}=0
$$
Where the coefficients $c_0,c_1,...,c_{n-1}$ are integers and $c_0\neq 0$. Any rational solution of this equation must be integer that divides $c_0$. 

### Proof:

Clearly, since $x^n$ with coefficient 1, Thus $r$ is an integer and it divides $c_0$.



### Example 2

Prove $\sqrt{2}$ is not a rational number.

Proof: By the corollary, the only rational number that could possible be solutions of $x^2-2=0$ is $\pm1,\pm2$. and $\sqrt{2}$ also a solution of $x^2-2=0$, it cannot be a rational number.



### Example 3

prove $a=\sqrt{2+\sqrt[3]{5}}$ is not a rational number

Proof: The expression $a=\sqrt{2+\sqrt[3]{5}}$ means $a^2=2+\sqrt[3]{5}$ so that $(a^2-2)^3=5$. Therefore we have $a^6-6a^4+12a^2-13=0$. By corollary, the only possible rational solutions are $\pm 1$, $\pm 13$. When $x=1\ or\ -1$, the left hand side of the equation is $-6$ and when $x=13$ or $x=-13$, the left hand side of the equation turns out to equal 4657458. This last computation could be avoided by using a little common sense. Either oberve $a$ is "obviously" bigger than 1 and less than 13, or observe. 
$$
13^{6}-6 \cdot 13^{4}+12 \cdot 13^{2}-13=13\left(13^{5}-6 \cdot 13^{3}+12 \cdot 13-1\right) \neq 0
$$
Since the term in paraenthese cannot be zero: it is one less than some multiple of 13. 