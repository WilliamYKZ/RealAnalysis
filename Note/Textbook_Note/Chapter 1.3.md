# Chapter 1.3

1. The basic algebraic operations in $\mathbb{Q}$ are addition and multiplication. Given a pair $a,b$ of rational number, **the sum $a+b$ and the product $ab$ also represent rational number**. Moreover, the following properties hold. 

   - $a+(b+c)=(a+b)+c$ for all $a, b, c$ (Associative) 
   - $a+b=b+a$ for all $a, b$ (commutative) 
   - $a+0=a$ for all $a$
   - For each $a$, there is an element $-a$ such that $a+(-a)=0$.

   

   - $a(b c)=(a b) c$ for all $a, b, c$ (Associative) 

   - $a b=b a$ for all $a, b$ (commutative) 

   - $a \cdot 1=a$ for all $a$

   - For each $a\neq 0$, there is an element $a^{-1}$ such that $aa^{-1}=1$.

     

   - $a(b+c)=a b+a c$ for all $a, b, c$  (distributive) 



2. A system that has more than one element and satisfies these nine properties is called a **field. **





3. The set $\mathbb{Q}$ also has an order structure $\le $ satisfying
   - Given $a$ and $b$, either $a\le b\ or \ b\le a$
   - If $a\le b$ and $b\le a$, then $a=b$.
   - If $a \leq b$ and $b \leq c$, then $a \leq c$
   - If $a \leq b$, then $a+c \leq b+c$
   - If $a \leq b$ and $0 \leq c$, then $a c \leq b c$



4. A field with an ordering satisfying properties )1 through )5 is called an **ordered firld**.



## Theorem of field

The following are consequence of the field properties:

1. $a+c=b+c$ implies $a=b$
2. $a\cdot 0 = 0 $ for all $a$
3. $(-a)b=-ab$ for all $a,b$
4. $(-a)(-b)=a b$ for all $a, b$
5. $a c=b c$ and $c \neq 0$ imply $a=b$
6. $ab=0$ implies either $a=0$ or $b=0$; for $a,b,c\in \mathbb{R}$



## Theorem of ordered field

The following are consequences of the properties of an ordered field:

1. If $a \leq b$, then $-b \leq-a$
2. If $a \leq b$ and $c \leq 0$, then $b c \leq a c$
3. If $0 \leq a$ and $0 \leq b$, then $0 \leq a b$
4. $0 \leq a^{2}$ for all $a$
5. $0<1$
6. If $0< a$, then $0< a^{-1}$
7. If $0<a<b$ then $0<b^{-1}<a^{-1}$. For $a,b,c\in \mathbb{R}$



## Two Definition 

1. We define

   $|a|=a \quad$ if $\quad a \geq 0 \quad$ and $\quad|a|=-a \quad$ if $\quad a \leq 0$

​		$|a|$ is called the absolute value of $a$.

The absolute value of a represent the distance between 0 and $a$, but in fact we will define the idea of "distance" in term of the "absolute value", which in turn was define in terms of ordering.



2. For numbers $a$ and $b$ we define $dist(a,b)=|a-b|$; $dist(a,b)$ represents the **distance between a and b**.





## Theorem of absolute value

1. $|a|\ge 0$ for all $a\in \mathbb{R}$
2. $|ab|=|a|\cdot|b|$ for all $a,b\in \mathbb{R}$
3. $|a+b|\le |a|+|b|$ for all $a,b\in\mathbb{R}$



## Corollary

$dist(a,c)\le dist(a,b)+dist(b,c)$ for all $a,b,c\in \mathbb{R}$



## Triangle Inequality

$|a+b|\le |a|+|b|$ for all $a,b$. 

