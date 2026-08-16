# Basic Calculus and Complex Analysis


# Linear algebra

Mathematics is not only about numbers, it is also about structure. 
A lot of mathematics is about structures.
Linear algebra is where we build the
foundation of that structure.

## Matrix: Definition

---

- A **matrix** is a rectangular array of scalars from a field $F$.
- An $m \times n$ matrix a has $m$ rows and $n$ columns. The entry in the $i$-th row and $j$-th column is noted $A_{ij}$.

$$
A = \begin{pmatrix}
A_{11} && A_{12} && \dots && A_{1n} \\
\vdots && \vdots && \ddots && \vdots \\
A_{m1} && A_{m2} && \dots && \ A_{mn}
\end{pmatrix}
$$

For now, scalars we can just think of numbers and the field $F$ a number set,
where we take the scalars from. More strictly, it is an algebraic structure where
addition, subtraction, multiplication, and division (for non-zero elements) are defined.

Going forward, $F$ will mostly consider matrices were $F$ is either
$\mathbb{R}$ or $\mathbb{C}$.

### Example 1: a $2$ by $2$ matrix

Example of a $2$ by $2$ matrix, also denoted as $2 \times 2$ matrix,
which has $2$ rows and $2$ columns

$$
\begin{pmatrix}
1 && 2 \\
3 && 4
\end{pmatrix}
$$

### Example 2: a $3$ by $2$ matrix

$$
A = \begin{pmatrix}
1 && 2 && 4 \\
7 && -7 && -6
\end{pmatrix}
$$

So $A_{12} = 2$, $A_{23} = -6$, $A_{13} = 4$. Note that for example $A_{32}$ does not exist!

### Example 3: a matrix over $\mathbf{C}$

$$
A = \begin{pmatrix}
1 + i && -2i \\
i\sqrt{3} && -7
\end{pmatrix}
$$

## Matrix: Operations

---

- **Addition**: 
$$
(A + B)_{ij} = A_{ij} + B_{ij}
$$
- **Scalar multiplication**: 
  
$$(cA)_{ij} = c \cdot A_{ij}$$

- **Matrix multiplication**: If $A$ is $m \times n$ and B is $n \times p$,
  their product $AB$ is an $m \times p$ matrix with entries: 

$$(AB)_{ij} = \sum^n_{k=1}A_{ik}B_{kj}$$

- It is **associative**, $(AB)C = A(BC)$, but not **commutative** in general, $AB\neq BA$

### Example 1: addition

$$
\begin{pmatrix}
2 && 3 \\
4 && 1
\end{pmatrix}
+
\begin{pmatrix}
1 && 2 \\
3 && 4
\end{pmatrix}
=
\begin{pmatrix}
3 && 7 \\
5 && 7
\end{pmatrix}
$$ 

### Example 2: subtraction

$$
\begin{pmatrix}
1 && 3 \\
7 && 4
\end{pmatrix}
-
\begin{pmatrix}
-3 && 2 \\
0 && 7
\end{pmatrix}
=
\begin{pmatrix}
4 && 1 \\
7 && -3
\end{pmatrix}
$$ 

### Example 3: scalar multiplication

$$
(-3) \cdot
\begin{pmatrix}
1 && 2 && 3 \\
4 && 5 && 8
\end{pmatrix}
=
\begin{pmatrix}
-3 && -6 && -9 \\
-12 && -15 && -24
\end{pmatrix}
$$ 

### Example 4: scalar multiplication

$$
(7) \cdot
\begin{pmatrix}
1 && 7 \\
9 && -8
\end{pmatrix}
=
\begin{pmatrix}
7 && 49 \\
63 && -56
\end{pmatrix}
$$ 

### Example 5: matrix multiplication

We take the $i$-th row of $A$ and the $j$-th column of $B$, multiply
the corresponding terms and add them:

$$
\begin{pmatrix}
1 && 2 \\
3 && 4
\end{pmatrix}
\begin{pmatrix}
2 && 4 \\
0 && 3
\end{pmatrix}
=
\begin{pmatrix}
2 && 10 \\
6 && 24
\end{pmatrix}
$$ 

### Example 6: matrix multiplication

$$
\begin{pmatrix}
1 && 2 && 3 \\
4 && 5 && 6\end{pmatrix}
\begin{pmatrix}
3 && 2 \\
4 && -4 \\
-1 && 0
\end{pmatrix}
=
\begin{pmatrix}
8 && -6 \\
26 && -12
\end{pmatrix}
$$ 

### Example 7: associativity of matrix multiplication

$$
\left[
\begin{pmatrix}
1 && 2 \\
3 && 4 
\end{pmatrix}
\begin{pmatrix}
0 && 1 \\
-2 && 3 
\end{pmatrix}
\right]
\begin{pmatrix}
-1 && 1 \\
2 && -2
\end{pmatrix}
=
\begin{pmatrix}
-4 && 7 \\
-8 && 15
\end{pmatrix}
\begin{pmatrix}
-1 && 1 \\
2 && -2
\end{pmatrix}
=
\begin{pmatrix}
-18 && 18 \\
38 && -38
\end{pmatrix}
$$ 

$$
\begin{pmatrix}
1 && 2 \\
3 && 4
\end{pmatrix}
\left[
\begin{pmatrix}
0 && 1 \\
-2 && 3
\end{pmatrix}
\begin{pmatrix}
-1 && 1 \\
2 && -2
\end{pmatrix}
\right]
=
\begin{pmatrix}
1 && 2 \\
2 && -2
\end{pmatrix}
\begin{pmatrix}
2 && -2 \\
8 && -8
\end{pmatrix}
=
\begin{pmatrix}
-18 && 18 \\
38 && -38
\end{pmatrix}
$$ 

## Matrix: Types

---

- **Square Matrix**: A matrix where the number of rows equals the number of columns $m=n$.
- **Zero Matrix ($O$)**: A matrix where all entries are zero. It acts as the additive identity: $A + O = A$.
- **Diagonal Matrix**: A square matrix where all non-diagonal entries are zero.
- **Identity Matrix ($I_n$)**: The $n \times n$ diagoonal matrix with 1s on the diagonal. It acts as a multiplicative identidy: $AI_n = I_n A = A$

### Example 1: square matrices

$$
n \times n,
\begin{pmatrix}
1 && 2 \\
3 && 7
\end{pmatrix},
\begin{pmatrix}
1 && 2 && 0 \\
-7 && 6 && 27 \\
0 && -6 && 1
\end{pmatrix}
$$

### Example 2: $2 \times 3$ zero matrix

$$
\begin{pmatrix}
1 && 5 && -6 \\
0 && 1 && 2
\end{pmatrix}
\begin{pmatrix}
0 && 0 && 0 \\
0 && 0 && 0
\end{pmatrix}
=
\begin{pmatrix}
1 && 5 && -6 \\
0 && 1 && 2
\end{pmatrix}
$$

### Example 3: diagonal matrices

$$
\begin{pmatrix}
1 && 0 \\
0 && 3
\end{pmatrix},
\begin{pmatrix}
1 && 0 && 0 \\
0 && 2 && 0 \\
0 && 0 && 4
\end{pmatrix}
$$

### Example 4: identity matrix

$$
I_2 = 
\begin{pmatrix}
1 && 0 \\
0 && 1
\end{pmatrix}
$$

$$
\begin{pmatrix}
1 && 0 \\
0 && 1
\end{pmatrix}
\begin{pmatrix}
a && b \\
c && d 
\end{pmatrix}
=
\begin{pmatrix}
a && b \\
c && d
\end{pmatrix}
=
\begin{pmatrix}
a && b \\
c && d
\end{pmatrix}
\begin{pmatrix}
1 && 0 \\
0 && 1
\end{pmatrix},
$$

## Matrices and Systems of Linear Equations

---

A system of linear equations can be written as a single matrix equation

$$
\begin{cases}
a_{11}x_1 + \cdots +A_{1n}x_1 = b_1 \\
\vdots                              \\
a_{m1}x_1 + \cdots +A_{mn}x_n = b_m
\end{cases}
\Longleftrightarrow
\begin{pmatrix}
a_{11} && \cdots && a_{1n} \\
\vdots && \ddots && \vdots \\
a_{m1} && \cdots && a_{mn}
\end{pmatrix}
\begin{pmatrix}
x_1 \\
\vdots \\
x_n
\end{pmatrix} =
\begin{pmatrix}
b_1 \\
\vdots \\
b_m
\end{pmatrix}
$$

That is, $A\bf{x} = \bf{b}$

### Example 1: how it works

$$
\begin{cases}
2x+3y+5z=7 \\
 x+4y+8z=-3 \\
 x+5y+9z=8 
\end{cases}
\Longleftrightarrow
\begin{pmatrix}
2 && 3 && 5 \\
1 && 4 && 8 \\
1 && 5 && -9
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix} =
\begin{pmatrix}
2x+3y+5z \\
x+4y+8z \\
x+5y+9z
\end{pmatrix}=
\begin{pmatrix}
7 \\
-3 \\
8
\end{pmatrix}
$$

This can be written as:

$$
A\vec{x}=\vec{b}
$$

So the natural question is, how do we solve $x$, $y$, and $z$?

If $\vec{x}$ and $\vec{b}$ were just ordinary numbers $x$ and $b$, we would multiply 
both left and right with reciprocal $\dfrac{1}{a}$:

$$
\dfrac{1}{a}ax = \dfrac{1}{a}b \Rightarrow x = \dfrac{b}{a}
$$

So the key value here is $\dfrac{1}{A}$, which gives the identity when multiplied by $A$.
Now the identity for matrices is $I_n$, so we are looking for a matrix $B$ for which

$$
AB=BA=I_n
$$

## Invertible Matrices

---

A square matrix $A$ is **invertible** if an **inverse** matrix $A^{-1}$ exists that satisfies

$$
A A^{-1} = A^{-1} A = I_n
$$

### Example 1: invertible $2 \times 2$ matrix

$$
\text{Let}\ A=
\begin{pmatrix}
2 && 3 \\
1 && 2 
\end{pmatrix},\ \text{then }\ A^{-1}=
\begin{pmatrix}
2 && -3 \\
-1 && 2
\end{pmatrix}
$$

This can easily be verified as follows:

$$
AA^{-1} =
\begin{pmatrix}
2 && 3 \\
1 && 2
\end{pmatrix}
\begin{pmatrix}
2 && -3 \\
-1 && 2
\end{pmatrix}
=
\begin{pmatrix}
1 && 0 \\
0 && 1
\end{pmatrix}
$$

### Example 2: invertible $3 \times 3$ matrix

$$
B = \begin{pmatrix}
1 && 1 && 1 \\
0 && 1 && 1 \\
1 && 0 && 1
\end{pmatrix},\ B^{-1}= 
\begin{pmatrix}
1 && -1 && 0 \\
1 && 0 && -1 \\
-1 && 1 && 1
\end{pmatrix}
\Rightarrow
BB^{-1}=B^{-1}B=I_3
$$

However, not every matrix as an inverse matrix. 

### Example 3: a non-invertible matrix

$$
A =
\begin{pmatrix}
0 && 0 \\
0 && 0
\end{pmatrix}
\Rightarrow
\begin{pmatrix}
0 && 0 \\
0 && 0
\end{pmatrix}
\begin{pmatrix}
a && b \\
c && d
\end{pmatrix}=
\begin{pmatrix}
0 && 0 \\
0 && 0
\end{pmatrix}\neq I_2
$$

So not every matrix as an inverse!

## Invertible matrices

---

A square matrix $A$ is **invertible** if an **inverse** matrix $_{-1}$ exists that satisfies:

$$
AA_{-1} = A_{-1}A = I_n
$$

### Example 1

$$
\begin{cases}
2x + 3y = 13 \\
x+2y = 8
\end{cases}
\Longleftrightarrow
\begin{pmatrix}
2 && 3 \\
1 && 2
\end{pmatrix}
\begin{pmatrix}
x \\
y 
\end{pmatrix}=
\begin{pmatrix}
13 \\
8
\end{pmatrix}
$$

Multiplication by the inverse matrix on both sides gives (for the inverse matrix, 
see the first example listed under Invertible Matrices):

$$
\begin{pmatrix}
2 && -3 \\
-1 && 2
\end{pmatrix}
\begin{pmatrix}
2 && 3 \\
1 && 2
\end{pmatrix}
\begin{pmatrix}
x \\
y
\end{pmatrix}=
\begin{pmatrix}
2 && -3 \\
-1 && 2
\end{pmatrix}
\begin{pmatrix}
13 \\
8
\end{pmatrix}
\Rightarrow
\begin{pmatrix}
x \\
y
\end{pmatrix}=
\begin{pmatrix}
2 \\
3
\end{pmatrix}
$$

Now that we learned about inverse matrices, we would like to find the inverse of

$$
\begin{pmatrix}
a && b \\
c && d
\end{pmatrix}
$$

Note that at this point, we don't even know if this matrix _has_ an inverse.

We are looking for an inverse matrix, so we have

$$
\begin{pmatrix}
a && b \\
c && d
\end{pmatrix}
\begin{pmatrix}
x && y \\
z && w
\end{pmatrix}=
\begin{pmatrix}
1 && 0 \\
0 && 1
\end{pmatrix}=
\begin{pmatrix}
ax+bz && ay+bw \\
cx+dz && cy+dw
\end{pmatrix}
$$

From this we infer that

$$
\begin{cases}
ax+bz = 1 \\ 
ay+bw = 0 \\
cx+dz = 0 \\ 
cy+dw = 1
\end{cases} \Rightarrow
\begin{cases}
adx+bdz = d \\
ady+bdw = 0 \\
bcx+bdz = 0 \\
bcy+bdw = b
\end{cases}
$$

Subtraction of the first and the third equations and the second and last respectively results in:

$$
\begin{cases}
x = \dfrac{d}{ad-bc} \\
y = \dfrac{-b}{ad-bc} \\
z = \dfrac{-c}{ad-bc} \\
w = \dfrac{a}{ad-bc}
\end{cases}, ad-bc\neq 0 \Rightarrow
\begin{pmatrix}
x && y \\
z && w
\end{pmatrix}=
\dfrac{1}{ad-bc}
\begin{pmatrix}
d && -b \\
-c && a
\end{pmatrix}
$$

So the matrix has an inverse if and only if $ad-bc\neq 0$. So the $ad-bc$ quantity is key here,
as it determines if the matrix is invertible or not! 
This quantity is called the determinant. It can be generalized to any $n \times n$ matrix.

## The Determinant

---

A **determinant** is a function
$$
\text{det:} M_{n \times n}(F) \rightarrow F
$$
that assigns a scalar to each square matrix.

-
$$
A\ \text{is invertible} \Longleftrightarrow {\text det}(A)\neq 0
$$

-
$$
{\text det}(AB)={\text det}(BA)
$$

- For a $2\times2$ matrix,
$$
{\text det}\begin{pmatrix} a && b \\ c && d\end{pmatrix}=ad-bc
$$

## Matrix Groups: Notation

---

For a field $F$ and a positive integer $n$:
- $Mat_n(F)$: the set of all $n\times n$ matrices with entries in F.
- $GL_n(F)$: the general linear group is the group of all invertible matrices in $Mat_n(F)$.

$$
GL_n(F) = \{A\in Mat_n(F) | \text{det}(A)\neq 0\}.
$$

- $SL_n(F)$: the special linear group is a subgroup of $GL_n(F)$, consisting of matrices with determinant 1.

$$
SL_n(F) = \{A\in GL_n(F) | \text{det}(A)=1\}.
$$

### Example 1: members of $Mat_n(F)$

$$
Mat_2(\mathbb{R}):\ \begin{pmatrix} 2 && 3 \\ -1 && \sqrt{7}\end{pmatrix},\ \begin{pmatrix} \pi && 3+\sqrt{2} \\ -7 && \dfrac{3}{4}\end{pmatrix}
$$

### Example 2: members of $GL_n(F)$

$$
GL_2(\mathbb{R}):\ \begin{pmatrix} 1 && 2 \\ 3 && 4\end{pmatrix} \Rightarrow \text{det}=-2
$$

However, the following matrix is _not_ a member of $GL_2(\mathbb{R})$, as it is a non-invertible matrix:

$$
\begin{pmatrix} 2 && 4 \\ 5 && 10\end{pmatrix} \Rightarrow \text{det}=-0
$$

### Example 3: members of $SL_n(F)$

$$
\begin{pmatrix} 3 && 2 \\ 7 && 5\end{pmatrix} \in SL_2(\mathbb{R})
$$

But

$$
\begin{pmatrix} 4 && 6 \\ 0 && 1\end{pmatrix} \notin SL_2(\mathbb{R})
$$

We stated earlier that mathematics is not only about numbers, 
it is also about structure. A vector space is one of the most important
examples of such a structure.

## Vector Space: Axioms

---

A **vector space** $V$ over a field $F$ is a set with addition ($+, V\times V \rightarrow V$) 
and scalar multiplication ($\cdot, V\times F \rightarrow V$)
satisfying these axioms for all $x,y,z\in V$ and $a, b\in F$:

Here we intentionally want to generalize the concept of a vector!

**VS 1**: $x + y = y + x$ (addition: commutativity)

**VS 2**: $(x + y) + z = x + (y + z)$ (addition: associativity)

**VS 3**: $\exists {\bf 0} \in V\ \text{s.t.}\ x + {\bf 0}= x$ (addition: zero vector)

**VS 4**: $\forall x\in V, \exists(-x) \in V\ \text{s.t.}\ x + (-x) = {\bf 0}$ (addition: inverse)

**VS 5**: $1 \cdot x = x$ (scalar multiplication: identity)

**VS 6**: $1 (ab)\cdot x = a\cdot(b\cdot x)$ (scalar multiplication: associativity)

**VS 7**: $a\cdot(x + y) = a\cdot x + a\cdot y$ (scalar multiplication: distributive law)

**VS 8**: $(a + b)\cdot x = a\cdot x + b\cdot x$ (scalar multiplication: distributive law)

Note that addition is also a generalized concept here, an operation which name
happens to be addition, hence we cannot
automatically assume that $x + y = y + x$ always holds.

For example, assume $V=\mathbb{R}$ and we define $a + b := a^b + e^ab^{72}\in \mathbb{R}$
This definition of addition does _not_ statisfy **VS 1** and **VS 2**!

### Example vector spaces

$\mathbb{R}$, $\mathbb{C}$, and the cartesian product $\mathbb{R}^n$.

For the first two, we define addition and multiplication in the familiar way.
For the last one, we define addition as follows:

$$
(x_1, x_2, \dots, x_n) + (y_1, y_2, \dots, y_n) = (x_1+y_1, x_2+y_2, \dots, x_n+y_n)
$$

and scalar multiplication

$$
a (x_1, x_2, \dots, x_n) = (ax_1, ax_2, \dots, ax_n)
$$

Another example is $\mathbb{R}[x]$, the set of all polynomials with real coefficients.
So how do we know that $\mathbb{R}[x]$ is a vector space? We check if all axioms hold!
For example, if we add two polynomials and change the order under addition, do we get
the same result back? Yes, we do!

$$
(1 + x) + (3 + x^2) = (3 + x^2) + (1 + x)
$$

Similarly, we can check that all other axioms hold.

Also, the set of al continuous functions $C_0(\mathbb{R})$ is a vector space, as is $Mat_2(\mathbb{R})$.

However, $\matbb{N}$ is _not_ a vector space, as 0 is not in the set. Also, if we pick any natural number,
the negative is _not_ in the set.
