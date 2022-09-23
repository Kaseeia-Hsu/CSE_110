# Discrete Mathematics

## Week 2

## 5.1 Cartesian Products and Relations

### Definition 5.1

Cartesian product, or cross product, is that sets A and B denoted by A X B.

- $A \times B = {(a,b) | a \in A, b \in B}$

It's a ordered pairs. Let $A$ = {2,3,4}, $B$ = {4,5}. Then,

B^2^ = $B \times B$ = {(4,4) ,(4,5), (5,4), (5,5)}.



### Definition 5.2

E.g. $A$ = {Tom, Brian, Joe}, Then,

$A \times A$ = ${(T,T), (T,J), (T,B), (J,T). (J,J), (J,B), (B,T), (B,J), (B,B)}$

If Brian and Joe are roommates, then (J,B) and (B,J) are the subsets defined by this definition,

And also, you can say that (J,J) and (B,B) correspond to this condition. This is __Relation__.



E.g. $A$ = {a~1~ ~ a~m~}, $B$ = {b~1~ ~ b~n~}, and make a matrix of it, we will find that there're 2^mn^ relations.



## Week 3

### Example 5.6

Relation is also a set, it's actually sets of matching:

E.g $A:R$ = ${(0,0), ({1},{1,2}), ({1},{1})}$



### Example 5.8

$R$ is the subset of $N \times N$ where R = ${(m.n)|n=7m}$,

So it could be $(0,0), (1,7), (11,77)$... It's infinite.

The relation $R$ on $N$ can also be given recursively by:

- $(0,0)$ belongs to $R$: and
- If $(s,t)$ belongs to R, then $(s+1, t+7)$ belongs to $R$.



### Exercise 5.1

1.

3.

5.

7.

9.



## 5.2 Functions: Plain and One-to-One

Functions, or mappings are special cases of Relation(Can only be 1-to-1), and these limits don't exist in Relations. So we define a f: A &rarr; B which means that in function f, __every element of A__ appears __exactly once__ as the first component of an ordered pair in the relation.



$(a,b) \in f$  , b is called the image of a under f, whereas $a$ is preimage of $b$.

And if $(a,b), (a,c) \in f$, it means that $b$ must equals to $c$.



### Definition 5.5

A function $A \rarr B$ is called one-to-one, or injective(one to multiple), but can't be multiple to one.



### Example 5.13

For example, Supposed that there's a $f(x)=3x+7$ , and two values $x_1,  x_2$,

We put these two values into the function, and the result is: $f(x_1)=f(x_2)$;

Which can also be written as $3x_1+7=3x_2+7$. so $x_1=x_2$.

This proved that this is a one-to-one function.



### Example 5.14

Since it's a one-to-one function, and we know there's $n$ elements in $A$, $m$ in $B$. We can say that the there are $n(n-1)(n-2)...(n-m+1)=\frac{n!}{(n-m)!}$ possible ways.



### Definition 5.6

If $f: A \rarr B$  and $A_1 \subseteq A$ , then $f(A_1) = {b \in B \mid b=f(a)}$.

And we say that $f(A_1)$ is the image __under__ $f$.

### Example 5.15



### Example 5.16



### Theorem 5.2

Let $f: A \rarr B$. with A~1~, A~2~ $\subseteq$ A

(a) $f(A_1 \cap A_2)$ = $f(A_1) \cup f(A_2)$;

(b) $f(A1 \cap A2) \subseteq f(A1) \cap f(A2)$;

(c) $f(A1 \cap A2) = f(A1) \cap f(A2)$ when $f$ is one-to-one.



### Definition 5.7



### Definition 5.8



### Example 5.17



### Exercise 5.2

1.

3.

5.

7.

9.



## 5.3 Onto Functions: Stirling Numbers of the Second Kind

### Definition 5.9

Onto function, also called surjective function, means that the range of the function cover the whole codomain(all elements included). For all $b \in B$ , there's at least one $a \in A$ with $f(a)=b$.



### Example 5.23

For $A = {w, x, y, z}$ and $B = {1, 2, 3}$, there are 3^4^ functions from $A$ to $B$, why?

We can find $3^4 - \binom 3 2 2^4 + 3 =  \binom{3}{3}3^4 -\binom{3}{2} 2^4-\binom3 11^4=36$.

Which means (all onto)-(all 2 elements)+(minus repeated).

And we get $\sum_k^n(-1)^k\binom {n} {n-k}(n-k)^m$. You can also see it represents 2 things with different containers.

So $\frac 1 {n!}\sum_k^n(-1)^k\binom {n} {n-k}(n-k)^m$ means the originally different $n$ containers are now the same.



### Theorem 5.3

$S(m+1, n)=S(m, n-1)+nS(m,n)$ 

if $m'=1$ or $n=1$, return $1$.

else return$ (S(m'-1,n-1)+nS(m'-1,n))$.

This is what we called recursive algorithm.



Proof:





 









