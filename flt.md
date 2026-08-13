# Linear algebra

Mathematics is also about structure. Linear algebra is where we build the
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

- **Addition**: $(A + B)_{ij} = A_{ij} + B_{ij}$
- **Scalar multiplication**: $(cA)_{ij} = c \cdot A_{ij}$
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

