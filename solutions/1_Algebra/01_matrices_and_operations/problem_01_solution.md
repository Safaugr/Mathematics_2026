# Exercise 1. Matrix Size and Entries

## Question

Given

$$
A=
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$.
3. Write the second row of $A$ and the first column of $B$ as vectors.

## Solution

### 1. Matrix sizes

Matrix A has 2 rows and 3 columns, so its size is $2\times3$.
Matrix B has 3 rows and 2 columns, so its size is $3\times2$.

### 2. Matrix entries

The first index indicates the row, and the second indicates the column.

- $a_{12}=-1$: row 1, column 2 of A.
- $a_{23}=5$: row 2, column 3 of A.
- $b_{21}=-2$: row 2, column 1 of B.
- $b_{32}=1$: row 3, column 2 of B.

### 3. Row and column vectors

The second row of A is

$$
\begin{pmatrix}
0 & 4 & 5
\end{pmatrix}.
$$

The first column of B is

$$
\begin{pmatrix}
1 \\
-2 \\
4
\end{pmatrix}.
$$

### Verification

The row vector has 3 entries, matching the number of columns of A.
The column vector has 3 entries, matching the number of rows of B.
Each selected entry matches its stated row and column in the given matrices.
