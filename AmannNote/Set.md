# Set

## Elementary Facts

1. If $X$ and $Y$ are set, then $X\subseteq Y$ means $X$ is a **subset** of $Y$, or $X$ is contained in $Y$. That each element of $X$ is also an element of $Y$, that is $\forall x\in X:x\in Y$. 



2. Equality of sets is defined by

$$
X=Y :\Leftrightarrow (X\subseteq Y)\and (Y\subseteq X)
$$

3. The statements 

$$
\begin{align}
X\subseteq X \tag{reflexivity}\\
(X\subseteq Y)\and (Y\subseteq Z)\Rightarrow (X\subseteq Z) \tag{transitivity}

\end{align}
$$

4. If $X\subseteq Y$ and $X\neq Y$, then $X$ is called a proper subset of $Y$. we denote this relationship by $X\subset Y$, and say 'X is properly contained in Y'. 



5. If $X$ is a set and $E$ is a property then $\{x \in X ; E(x)\}$ is the subset of $X$ consisting of all elements $x$ of $X$ such that $E(x)$ is true. The set

$$
\empty x := \{x\in X; x\neq x\}
$$

is the **empty subset** of $X$





## The Power Set

1. If $X$ is a set, then so is its **power set** $\mathcal{P}(x)$. The elements of $\mathcal{P}(X)$ are the subsets of $X$. The following are true:

$$
\begin{aligned}
\emptyset \in \mathcal{P}(X), \quad X & \in \mathcal{P}(X) \\
x \in X \Leftrightarrow\{x\} & \in \mathcal{P}(X) \\
Y \subseteq X \Leftrightarrow Y & \in \mathcal{P}(X)
\end{aligned}
$$

In particular, $\mathcal{P}(X)$ is never empty.



### Example 1

(a): $\mathcal{P}(\emptyset)=\{\emptyset\}, \mathcal{P}(\{\emptyset\})=\{\emptyset,\{\emptyset\}\}$

(b): $\mathcal{P}(\{*, \odot\})=\{\emptyset,\{*\},\{\odot\},\{*, \odot\}\}$





## Complement, Intersection and Union

1. Let $A$ and $B$ be subsets of a set $X$. Then

$$
A \backslash B:=\{x \in X ;(x \in A) \wedge(x \notin B)\}
$$

is the **complement of $B$ in $A$**. When the set $X$ is clear from context, we write also
$$
A^c:= X\backslash A
$$
and call $A^c$ the **complement** of A.



2. The set 

$$
A \cap B:=\{x \in X ;(x \in A) \wedge(x \in B)\}
$$

is called the **intersection ** of $A$ and $B$. If $A \cap B=\empty$, that is, if $A$ and $B$ have no element in common, then $A$ and $B$ are **disjoint**. Clearly, $A \backslash B= A\cap B^c$. The set 
$$
A \cup B:=\{x \in X ;(x \in A) \vee(x \in B)\}
$$
is called the **union** of $A$ and $B$.



3. It is useful to represent graphically the relationships between sets using **Venn diagrams**. 

![](https://github.com/WilliamYKZ/Picture/raw/main/Picture/Screen%20Shot%202022-09-04%20at%208.08.17%20PM.png)



4. Proposition: Let $X$, $Y$ and $Z$ be sinsets of a set.

$$
\text { (i) } X \cup Y=Y \cup X, \quad X \cap Y=Y \cap X \text {. (commutativity) }\\
\text { (ii) } X \cup(Y \cup Z)=(X \cup Y) \cup Z, \quad X \cap(Y \cap Z)=(X \cap Y) \cap Z \text {. (associativity) }\\
\text { (iii) } \begin{aligned}
X \cup(Y \cap Z) &=(X \cup Y) \cap(X \cup Z) \\
X \cap(Y \cup Z) &=(X \cap Y) \cup(X \cap Z)
\end{aligned}\\
\text { (iv) } X \subseteq Y \Leftrightarrow X \cup Y=Y \Leftrightarrow X \cap Y=X
$$



## Products

1. From two objects $a$ and $b$ we can form a new object, the ordered pair $(a, b)$. Equality of two ordered pairs $(a, b)$ and $\left(a^{\prime}, b^{\prime}\right)$ is defined by

$$
(a, b)=\left(a^{\prime}, b^{\prime}\right): \Leftrightarrow\left(a=a^{\prime}\right) \wedge\left(b=b^{\prime}\right)
$$

The bject $a$ and $b$ are called the first and second **components** of the ordered pair $(a,b)$. For $x=(a,b)$, we also define 
$$
\operatorname{pr}_1(x):=a, \quad \operatorname{pr}_2(x):=b
$$
and, for $j=1,2$ (that is, for $j\in \{1,2\}$), we call $\operatorname{pr}_j(x)$ the $j^{\text {th }}$ **projection** of $x$.



2. If $X$ and $Y$ are sets, then the **Cartesian Product** $X\times Y$ of $X$ and $Y$ is the set of all ordered pairs $(x,y)$ with $x\in X$ and $y\in Y$.



### Example

For $X:=\{a, b\}$ and $Y:=\{*, \odot, \square\}$ we have
$$
X \times Y=\{(a, *),(b, *),(a, \odot),(b, \odot),(a, \square),(b, \square)\}
$$


3. Proposition: Let $X$ and $Y$ be sets

(i) $X \times Y=\emptyset \Leftrightarrow(X=\emptyset) \vee(Y=\emptyset)$.
(ii) In general: $X \times Y \neq Y \times X$.





3. The product of three sets $X$, $Y$ and $Z$ is defined by 

$$
X \times Y \times Z:=(X \times Y) \times Z
$$

This construction can be repeated to define the product of $n$ sets:
$$
X_1 \times \cdots \times X_n:=\left(X_1 \times \cdots \times X_{n-1}\right) \times X_n
$$
For $x$ in $X_1 \times \cdots \times X_n$ we write $\left(x_1, \ldots, x_n\right)$ instead of $\left(\cdots\left(\left(x_1, x_2\right), x_3\right), \ldots, x_n\right)$ and call $x_j$ the $j^{\text {th }}$ component of $x$ for $1 \leq j \leq n$. The element $x_j$ is also $\operatorname{pr}_j(x)$, the jth **projection** of $x$. Instead of $X_1 \times \cdots \times X_n$ we can also write
$$
\prod_{j=1}^n X_j
$$
If all the factors in this product are the same, that is, $X_j=X$ for $j=1, \ldots, n$, then the product is written $X^n$.





## Families of Sets

Let $A$ be a nonempty set and, for each $\alpha \in A$, let $A_{\alpha}$ be a set.  Then $\{A_{\alpha}; \alpha \in A\}$ is called a **family of set** and $A$ is an index set for this family. Family of sets is never empty.

let $X$ be a set, and $\mathcal{A}:=\left\{A_\alpha ; \alpha \in A\right\}$ a family of subsets of $X$. Generalizing the above concepts we define the **intersection**. and the **union** of this family by.
$$
\begin{aligned}
&\bigcap_\alpha A_\alpha:=\left\{x \in X ; \forall \alpha \in \mathrm{A}: x \in A_\alpha\right\} \\
&\bigcup_\alpha A_\alpha:=\left\{x \in X ; \exists \alpha \in \mathrm{A}: x \in A_\alpha\right\}
\end{aligned}
$$
Note that $\bigcap_\alpha A_\alpha$ and $\bigcup_\alpha A_\alpha$ are subsets of $X$.



1. Proposition: 

$$
\begin{aligned}
&\left(\bigcap_\alpha A_\alpha\right) \cap\left(\bigcap_\beta B_\beta\right)=\bigcap_{(\alpha, \beta)} A_\alpha \cap B_\beta \\
&\left(\bigcup_\alpha A_\alpha\right) \cup\left(\bigcup_\beta B_\beta\right)=\bigcup_{(\alpha, \beta)} A_\alpha \cup B_\beta \\\\\\
&\left(\bigcap_\alpha A_\alpha\right) \cup\left(\bigcap_\beta B_\beta\right)=\bigcap_{(\alpha, \beta)} A_\alpha \cup B_\beta \\
&\left(\bigcup_\alpha A_\alpha\right) \cap\left(\bigcup_\beta B_\beta\right)=\bigcup_{(\alpha, \beta)} A_\alpha \cap B_\beta \\\\\\
&\left(\bigcap_\alpha A_\alpha\right)^c=\bigcup_\alpha A_\alpha^c \cdot  \\
&\left(\bigcup_\alpha A_\alpha\right)^c=\bigcap_\alpha A_\alpha^c 
\end{aligned}
$$
