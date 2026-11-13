# Exercise 1. From a System to a Matrix

## Question

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7. \\
\end{cases}
$$

in the form Ax=b.

Identify the coefficient matrix, the vector of unknowns,
and the right-hand side vector. Explain how each row
of the matrix corresponds to one equation.

## Solution

### 1. Fix the order of the unknowns

Use the order x, y, z consistently.

The vector of unknowns is

$$
\mathbf{x}=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}.
$$

### 2. Construct the coefficient matrix

Each row contains the coefficients of x, y, and z
in the corresponding equation:

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}.
$$

The first row comes from 2x-y+z.
The second row comes from x+3y-2z.
The third row comes from 3x+y+z.

### 3. Construct the right-hand side vector

The constants on the right-hand sides give

$$
b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}.
$$

Therefore, the matrix equation is

$$
A\mathbf{x}=b,
$$

or explicitly,

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
=\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}.
$$

### 4. Verification

Expanding the matrix-vector product gives

$$
A\mathbf{x}=
\begin{pmatrix}
2x-y+z \\
x+3y-2z \\
3x+y+z \\
\end{pmatrix}.
$$

Equating this vector to b reproduces all three
original equations in the same order.

The dimensions are also consistent:
a 3-by-3 matrix times a 3-by-1 vector
produces a 3-by-1 vector.