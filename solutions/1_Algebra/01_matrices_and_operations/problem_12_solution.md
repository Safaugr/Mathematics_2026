# Exercise 12. Formula for a Matrix Power

The given matrix is

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

## 1. Computing successive powers

Using matrix multiplication,

$$
A^2=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}.
$$

Next,

$$
A^3=A^2A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix}.
$$

Similarly,

$$
A^4=A^3A=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}.
$$

## 2. Conjecture

The diagonal entries remain 1, and the lower-left entry
remains 0. The upper-right entry increases by 1 each time.

This suggests that, for every integer $n\ge1$,

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

## 3. Proof by mathematical induction

### Base case

For $n=1$, the formula gives

$$
A^1=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
=A.
$$

Thus, the formula holds for n=1.

### Induction step

Assume the formula holds for some integer $n\ge1$:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

Multiplying by A gives

$$
A^{n+1}=A^nA=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 1+n \\
0 & 1 \\
\end{pmatrix}.
$$

This is exactly the proposed formula with n replaced by n+1.
Therefore, the formula holds for every integer $n\ge1$.

## Verification at n=0

The same formula also gives the identity matrix at n=0:

$$
A^0=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$