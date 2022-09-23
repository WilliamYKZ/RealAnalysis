# Fundamentals of Logic



## Basic Notation

1. Symbolic logic is about **statements** which one can meaningfully claim to be true or false. That is, each statement has the truth value "True" or "False". There are no other possibilities, and no statement can be both true and false.



2. Any statement $A$ has a negation $\neg A$ (not A) defined by $\neg A$ is true if $A$ is false, and $\neg A$ is false if $A$ is true. 

![](https://github.com/WilliamYKZ/Picture/raw/main/Picture/Screen%20Shot%202022-08-27%20at%205.28.32%20PM.png)



3. Two statements, $A$ and $B$, can be combined using **conjunction** $\wedge$ and **disjunction** $\vee$ to make new statements. The statement $A\wedge B$ (A and B) and $A \vee B$ (A or B).

![](https://github.com/WilliamYKZ/Picture/raw/main/Picture/Screen%20Shot%202022-08-27%20at%205.35.10%20PM.png)



4. If $E(x)$ is an expression which be comes a statement when $x$ is replaced by an object (member, thing) of a soecified class (collection, universe) of objects, then $E$ is a **property**. The sentece "x has property E" means "E(x) is true". If x belongs to a class $X$, that is, x is an **element** of $X$, then we write $x\in X$, otherwise $x\notin X$. Then 

$$
\{x\in X; E(x)\}
$$

​			is the class of all elements $x$ of the collection $X$ which have property $E$. If $X$ is the class of all readers of this book and $E(x)$ is the statement 'x wear glasses', then $\{x\in X; E(x)\}$ is the class of all reader of this book who wear glasses.



5. $\exists$ denoted quantifier 'there exists'. means there is at least one object $x$ in (the class) $X$ which has property $E$. 

   $\exists ! x\in X: E(x)$ when exactly one such object exists. 



6. $\forall$ for the quantifier "for all". $\forall x \in X: E(x)$ means "Every $x$ in $X$ has the property $E$".





7. $:=$ denoted "is defined by"

$$
a:=b
$$

Means the object a is defined by the object b. 



### Example 1

1. $\neg(A\wedge B )=(\neg A)\vee (\neg B)$
2. $\neg(A\vee B)=(\neg A)\wedge (\neg B)$
3. $\forall x \exists y : E(x,y) $ and $\exists y\forall x: E(x,y)$ are different statements: in the first case, for all x there is some y such that $E(x,y)$ it true. Thus y depends on x, that is, for each x one has to find a possible different y such that $E(x,y)$ is true. In the second case it suffices to find a fixed $y$ such that th statement $E(x,y)$ is true for all $x$. 



## Implication

1. Let $A$ and $B$  be statements. Then one can define a new statement, the **implication** $A\Rightarrow B$ as follow

$$
(A\Rightarrow B):= (\neg A)\vee B
$$

Thus **A $\Rightarrow$ B is false if A is true and B is false, and is true in all other cases**. This is means that a true statement cannot imply a false statement, and also that a false statement implies any statement - true of false. 



It is common to express $A\Rightarrow B$ as "To prove B it sufficies to prove A", or "B is necessary for A to be true.", in other words, A is a sufficient condition for B, and B is a necessary condition for A.



2. The **equivalence** $A\Leftrightarrow B$ of the statements $A$ and $B$ is defined by 

$$
(A\Leftrightarrow B):=(A\Rightarrow B) \wedge (B\Rightarrow A)
$$

 A is a **necessary and sufficient** condition for $B$ (or vice versa). or we can say "A is true if and only if B is true".



3. The fundamental obervation is 

$$
(A\Rightarrow B)\Leftrightarrow (\neg B\Rightarrow \neg A)
$$

The statement $\neg B \Rightarrow \neg A$ is called the **contrapositive** of the statement $A \Rightarrow B$. 



4. To define a statement $A$ so that it is true whenever the statement $B$ is true, we write 

$$
A:\Leftrightarrow B
$$

and say 'A is true, by definition, if B is true.'



5. In mathemtics a true statement is often called a proposition, theorem, lemma or corollary. 



6. For $A\Rightarrow B$. Since the statement is automatically true if $A$ is false, the only interesting case is when $A$ is true. Thus to prove $A\Rightarrow B$ is true, one suppose that $A$ is true and then shows that $B$ is true.



7. The proof can proceed directly or "by contradiction". For a proof by contradiction one suppose that $B$ is false, that is $\neg B$ is true. Then one proves, using also the assumption that $A$ is true, a statement $C$ which is already known to be false. It follows from this 'contradiction' that $\neg B$ cannot be true, and hence that $B$ is true. 

