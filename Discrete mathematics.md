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

1, 3, 5, 7, 9 (Finished)



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

For $A={1, 2, 3, 4, 5}, B={w, x, y, z}$, let $f A \rarr B$ be given by $f= {(1,w), (2,x), (3,x), (4,y), (5,y)}$.

And then $ A_1={1}, A_2={1, 2}, A_3={1, 2, 3}, A_4={2, 3}$.

We could know that: $f(A_1)=f(1)=w$

$f(A_2)={{f(a) \mid a= 1 or 2}}=w, x$

$f(A_3)=f(a) \mid a = 1, 2, or 3 = w, x$

$f(A_4)=x$



### Example 5.16

(a) Set $g: R \rarr R$ , then $g(R)$ will be __the range__ of $g =[0, \infty)$

(b) Let $g: Z \rarr Z$, hen $g(Z)$ will be __the image__ of $h ={0, 1, 4, 9, 16...}$

 

### Theorem 5.2

Let $f: A \rarr B$. with A~1~, A~2~ $\subseteq$ A

(a) $f(A_1 \cap A_2)$ = $f(A_1) \cup f(A_2)$;

(b) $f(A1 \cap A2) \subseteq f(A1) \cap f(A2)$;

(c) $f(A1 \cap A2) = f(A1) \cap f(A2)$ when $f$ is one-to-one.



### Definition 5.7

If $f: A \rarr B$ and $A_1 \subseteq A$, while $B$ is a set where $A$ comes from at the same time, we call that $f \mid A_1: A_1 \rarr B$ is __the restriction__ of $f$ to $A_1$. Stull, it's the same as original function $A$, but not defined by $A$ any longer. Instead of it, it's defined by a smaller domain $A_1$.



### Definition 5.8

Let $A_1 \subseteq A$, and $f: A_1 \rarr B$. If there's a $g: A \rarr B$ and $g(a) = f(a)$ for all $a \in A_1$, we call that $g$ is an extension of $f$ to A.

 

### Example 5.17

For $A=1, 2, 3, 4, 5$ let $f: A \rarr R$ be defined by $f = {(1,10), (2,13), (3,16), (4,19), (5, 21)}$

Let $g: Q \rarr R \mid g(q)= 3q+7$ and $h: R \rarr R \mid h(r)=3r+7$.



And we could say that:

$g$ is an extension of $f$ from $A$ to $Q$;

$f$ is a restriction of $g$ from $Q$ to $A$;



#### $h$ is a extension of both $f$ and $g$.



### Exercise 5.2

1, 3, 5, 7, 9 (Finished)



## 5.3 Onto Functions: Stirling Numbers of the Second Kind

### Definition 5.9

Onto function, also called surjective function, means that the range of the function cover the whole codomain(all elements included). For all $b \in B$ , there's at least one $a \in A$ with $f(a)=b$.



### Example 5.23

For $A = {w, x, y, z}$ and $B = {1, 2, 3}$, there are 3^4^ functions from $A$ to $B$, why?

We can find $3^4 - \binom 3 2 2^4 + 3 =  \binom{3}{3}3^4 -\binom{3}{2} 2^4+\binom3 11^4=36$.

Which means (all onto)-(all 2 elements)+(minus repeated).

And we get $\sum_k^n(-1)^k\binom {n} {n-k}(n-k)^m$. You can also see it represents 2 things with different containers.

So $\frac 1 {n!}\sum_k^n(-1)^k\binom {n} {n-k}(n-k)^m$ means the originally different $n$ containers are now the same.



### Theorem 5.3

$S(m+1, n)=S(m, n-1)+nS(m,n)$ 

if $m'=1$ or $n=1$, return $1$.

else return$ (S(m'-1,n-1)+nS(m'-1,n))$.

This is what we called recursive algorithm.



Proof:

Put $(m+1)$ objects into $n$ containers.

Let $ A = {a_1, a_2,...,a_m, a_{m+1}}$ (The number of objects,) and there're two cases. One's that $a_{m+1}$ have other objects be in the same container with, while another is that $a_{m+1}$ being distributed into a container alone. So $S(m, n-1)$ means that we take $a_{m+1}$(m+1-1) and one container(n-1) off. And S(m, n) means that __no containers are empty__. We don't need to consider where $a_{m+1}$ is distributed to since we don't need to avoid that specific container now.

So $S(m+1, n)=S(m, n-1)+nS(m,n)$.

Though human brains can not afford to do work like this,  but we could use computers to help us do the work. 



## 5.4 Special Functions

### Example 5.10

Any function $f: A \times A \rarr B$ is called a binary operation. Computing elements of two specific domains. and if $B \subseteq A$. This operation is said to be "closed"(on a). 



### Example 5.11

A function $g: A \rarr A$ is called a unary, or monary, operation on A 



### Definition 5.12

Let $f: A \times A \rarr B$; which means $f$ is a binary operation on $A$

1. If $f(a,b) = f(b,a)$ for a; $(a,b) \in A \times A$, $f$ is said to be communicative for all $(a,b) \in A \times A$.
1. When $B \subseteq A$, $f$ is said to be associative if for all $a, b, c \in A. f(f(a,b),c) = f(a,f(b,c))$.



### Definition 5.13

Let $f: A\times A \rarr B$ be a binary operation on $A$. An element $x \in A$ is called an identity for $f$ if $f(a,x)=f(x,a)=a$. for all $a \in A$.



### Theorem 5.4

Identity is unique(only one identity in one binary operation). If $f(a, x_1) = a = f(x_1, a)$ and $f(a, x_2) = a = f(x_2, a)$. We can prove that $f(x_1, x_2) = f(x_1, x_2)$. So consequently: $x_1 = x_2$, and this proves that $f$ has at most 1 identity element.



### Definition 5.14

For sets $A, B$, if $D \subseteq A \times B$, then $\pi_A: D \rarr A$, defined by $\pi_A(a,b)=a$ is called the projection on the first coordinate, and if the function changes to $B$, it's called the projection on the second coordinate.

 

## 5.5 The Pigeonhole Principle

If $m$ pigeons occupy $n$ pigeon holes, and $m>n$,  then at least one pigeonhole has two or more pigeons dwell in it.



### Example 5.47

Assume there are $m+1$ numbers: $ 2^1 - 1, 2^2 - 1,...2^{m+1}-1$. And there're only $m$ possible reminders(from 0 to m-1). So there're $m+1$ different numbers with only $m$ remainders. We set that $2^S - 1 =qm+r$ and $2^t - 1 = pm + r$. Make line one minus line two, and we get that $qm - pm = 2^S - 2^t \rarr 2^t(2^{S-t}-1)$ which could be divided by $m$. $2^t$ is an even, so we now know that $m|(2^{S-t} - 1)$. This result follows $n = S - t$.



## 5.6 Function Composition and Inverse Functions

### Definition 5.15

If $f: A \rarr B$. then $f$ is said to be bijective, or to be one-to-one correspondence if it's both one-to-one and onto.



### Definition 5.16 / 17

Identity function $1_A: A \rarr A$. Defined by $1_A(a)=a$ for all $a \in a$. It's called an identity function for $A$.

If $f, g: A \rarr B$, we say that $f$ and $g$ are equal and write $ f=g$, if $f(a)=g(a)$ for all $a \in A$.



### Definition 5.18

If $ f: A \rarr B,  g: B \rarr C$. We define the composite function, which is denoted $g \circ f: A \rarr C$, by $(g \circ f)(a)=g(f(a))$.



### Theorem 5.5

Let $f: A \rarr B$ and $g: B \rarr C$:

(a) If $f$ and $g$ are one-to-one, then $g \circ f$ will also be one-to-one.

(b) If $f$ and $g$ are onto, then $g \circ f$ will also be onto.



### Theorem 5.6

If $f: A \rarr B$, $g: B \rarr C$, and $h: C \rarr D$, then $(h \circ g) \circ f = h \circ (g \circ f)$.



### Definition 5.19

If $f: A\rarr A$ we define $f^1=f$, and $n \in Z^+$, $f^{n+1}=f \circ (f^n)$. 



### Example 5.56

With $A={1,2,3,4}$ and $f: A \rarr A$ defined by $f={(1,2),(2,2),(3,1),(4,3)}$, we have $f^2 = f \circ f = f(f(x)) = (1,2),(2,2),(3,2),(4,2)$. and for $f^3$ is the same, equals to $f \circ f^2=f(f(f(x)))$, the answer will be: $(1,2),(2,2),(3,2),(4,2)$.



### Definition 5.20

Converse of relation $R$ is defined by $R^c$$$=$${$(b,a)|(a,b) \in R$}.



### Definition 5.21

If $f: A \rarr B$, then it is said to be a invertible function when there's a $g: B \rarr A$ such that $g \circ f = 1_A$ and $f \circ f^c=1_B$.



### Example 5.58

Let $f, g: R \rarr R$, be defined by $f(x)=2x+5, g(x)=\frac{1}{2}(x-5)$. Then $(g\circ f)(x)=g(f(x))=\frac{1}{2}[(2x+5)-5]=x$, and for $(f\circ g)(x)$ is the same, so we call them both invertible function.



### Theorem 5.7 / 8

(a) For a invertible function, another function is always unique.

(b) For a invertible function, another function is always one-to-one and onto.



### Theorem 5.9

If $f: A \rarr B, g:B \rarr C$ are invertible functions, then $g \circ f: A \rarr C$ and $(g \circ f)^{-1}=f^{-1} \circ g^{-1}$.



### Definition 5.22

If $f: A \rarr B$ and $B_1 \subseteq B$, then $f^{-1}(B_1) = {x \in a | f(x) \in B_1}$. The set $f^{-1}(B_1)$ is called the preimage of $B_1$ under $f$.

__And what is f^{-1} actually?__ Let's defined $f: R \rarr R$ by $f=(x,y)|y=mx+b$. And $f^{-1}={(y,x)|y=mx+b}={(x,y)|y=(1/m)(x-b)}$.



### Theorem 5.10

If $f: A \rarr B $ and $B_1, B_2 \subseteq B$, then:

(a) $f^{-1}(B_1 \and B_2)=f^{-1}(B_1)\and f^{-1}(B_2)$.

(b) $f^{-1}(B_1 \or B_2)=f^{-1}(B_1)\or f^{-1}(B_2)$.

(c) $f^{-1}(\overline{B_1})=\overline{f^{-1}(B_2)}$.



### Theorem 5.11

Let $f: A \rarr B$ for finite sets $A$ and $B$, where |A|=|B|. Then the following statement are equivalent: 

$f$ is one-to-one, onto, and invertible at the same time.

 

## 6. Languages: Finite State Machine



## 6.1 Language: The Set Theory of Strings



### Definition 6.1

If $\Sigma$ is an alphabet and $n \in Z^{+}$, we define the powers of $\Sigma$ recursively as follows:

1. $\Sigma^1 = \Sigma$; and
2. $\Sigma^{n+1} = {xy| x \in \Sigma, y \in \Sigma}$, where $xy$ denotes the juxtaposition of x and y



### Definition 6.2

For an alphabet $\Sigma$ we define $\Sigma^0$, where $\lambda$ denotes the empty string–that is, the string consisting of no symbols taken from $\Sigma$. The symbol $\lambda$ will never be an element in $\Sigma$. $\lambda \not\subseteq \Sigma$ and $\lambda \not= 0$ since |$\lambda$| = 1



### Definition 6.3

If $\Sigma $ is an alphabet, then,

(a) $\Sigma^+=\or^{\infin}_{n=1}\Sigma_{n\in Z^+}$. The plus sign means that it start from $n=1$, so $\lambda$ won't appear in $\Sigma^+$.

(b) $\Sigma^{*}=\or^{\infin}_{n=0}$. And it includes $\lambda$.



### Example 6.2

For $\Sigma={0,1}$, the set $\Sigma^{*}$ consists of all finite strings of $0^{*}$'s and $1^{*}$'s together with the empty string $\lambda$.



### Definition 6.4

If $w_1, w_2 \in \Sigma^+$, then we may write that $w_1=x_1x_2...x_m$ and $w_2=y_1y_2...y_n$. We could say that string $w_1$ and $w_2$ are equal, and $w_1=w_2$, if $m=n$ and $x_i=y_i$ for all $1\leq i \leq m$.



### Definition 6.5

The length of a string $w$ is denoted by $||w||$, but for the case of $\lambda$, $||\lambda||=0$.

 

### Definition 6.6

The concatenation of $x$ and $y$ is the string $x_1x_2x_3...y_1y_2y_3...$, as for $\lambda$, the concatenation of $\lambda$ and $x$ will be $\lambda x_1x_2x_3...$. In the opposite position, it will be $x_1x_2x_3...\lambda$. And finally, the concatenation of two $\lambda$ is $\lambda\lambda=\lambda$.

 

### Definition 6.7

For each $x \in \Sigma^{*}$, we define that the power of $x$ by $x^0=\lambda$, $x^1=x$, $x^2=xx$…



### Definition 6.8

If $x, y \in \Sigma^{*}$, and $w=xy$, we say the string $x$ is called the prefix of $w$(x could be a bunch of alphabets, numbers, or symbols like: x=6hdsf3). And if $y$ is not a empty string, we call $x$ a proper prefix; vice versa, $y$ is called a suffix or proper suffix.



### Example 6.4

There's no length limit for proper prefixes and proper suffixes, for example, consider the string $w=abbccc$, the prefix could be a, ab, or even abbccc. The same for the suffix, it could be c, bbccc, or abbccc.



### Definition 6.9

Substring is a string between prefix and suffix, and if there exist one prefix or suffix($\not=\lambda$), this substring is called proper substring. In some cases, we can say that the prefix or suffix is a substring, too. For example, 12111110, $x=12, y=11110, z=\lambda$, we could say that $y$ is both the substring and the suffix at the same time.



### Definition 6.10

For a given alphabet $\Sigma$, any subset of $\Sigma^{*}$ is called a language over $\Sigma$. This includes $\emptyset$, which is called an empty language.



### Example 6.8

With $\Sigma = {0,1}$ the set $A={0, 01, 001...}$ are examples of language over $\Sigma$.(subset of $\Sigma^*$.)



### Definition 6.11

For an alphabet $\Sigma$ and language $A, B \subseteq \Sigma^{*}$, the concatenation of A and B, denoted AB, is ${ab|a \in A, b \in B}$.



### Example 6.10

Repetition only appears once, or it's meaningless. For $\Sigma$=${x,y,z}$, and let $A, B$ be the finite language $A={x, xy, z}$, $B={\lambda, y}$. Then $AB ={x, xy, z, xyy, zy}$ and $BA={x, xy, z, yx, yxy, yz}$. So,

1. $|AB|=5 \not= 6=|BA|$, (not communicative); and
2. $|AB|=5\not=6=3\times2=|A||B|$, (not associative)



### Theorem 6.1

(a) $A{\lambda}={\lambda}A=A$	(b) $(AB)C=A(BC)$

(c)$A(B\or C)=AB\or AC$	(d)$(B \or C)A=BA \or CA$

(e)$A(B \and C) \subseteq AB \and AC$	(e)$(B \and C) A \subseteq BA \and CA$



### Definition 6.12

(a) $A^0=\lambda$

(b) $A^{+}=\or_{n\in Z^+}A^n$, called the positive closure of A.

(c) $A^{*}=A^{+}\or\lambda$, called the Kleene closure.

 

### Example 6.11

For $A=x$, $A^0=\lambda, A^n=x^n, A^{+}=x^n|n\geq1$; and $A^{*}=x^n|n\geq0$.



### Example 6.12

Let $\Sigma=x,y$

(a) If $A=xx,xy,yx,yy=\Sigma^2$, then $A^{*}$ is the language of all even length strings $w$ in $\Sigma^{*}$.

(b) For there's another $B=x,y$, $BA^{*}$ contains all the strings in $\Sigma^{*}$ in odd length.

(c) It tells how the prefix, suffix, and substring work in this example, fairly easy.

(d) ${[x,y]^{*}}$ contains every possible strings of x and y, hence $[x]^{*}[y]^{*}\subset[x,y]^{*}$



### Example 6.13

It shows us that when we removed a specific string from $A$, $A^2=B^2=B$ still, but $A\not=B$.



### Lemma 6.1

It demonstrates that once $A,B \subseteq \Sigma^{*}$, $A^n\subseteq B^n$, but it doesn't establish that $A^+ \subseteq B^+$ nor $A^{*} \subseteq B^{*.}$ 



### Theorem 6.2

For $A, B \subseteq \Sigma^{*}$,

(a) $A\subseteq AB^{*}$	(b) $A\subseteq BA^{*}$

(c) $A \subseteq B \rarr A^+ \subseteq B^+$	(d) $A \subseteq B \rarr A^{*} \subseteq B^{*}$

(e) $AA^{*}=A^{*}A=A^+$	(f) $A^{*}A^{*}=A^{*}=(A^{*})^{*}=(A^{*})^+=(A^+)^{*}$

(g) $(A\or B)^{*}=(A^{*}\or B^{*})^{*}=(A^{*}B^{*})^{*}$



### Example 6.16

The reversal of a string, for example, $x=x_1x_2x_3...x_n$, becomes $x^R=x_nx_{n-1}x^{n-2}...x_1$. And $\lambda^R=\lambda$, still.

Let $x_1,x_2 \in \Sigma^{*}$, $(x_1x_2)^R={x_2}^R{x_1}^R$.



## 6.2 Finite State Machine: A First Encounter

__The notes of this chapter are all in paper form due to the needed of visualization.__
