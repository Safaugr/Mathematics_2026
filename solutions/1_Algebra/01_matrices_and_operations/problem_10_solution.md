# Exercise 10. Columns of a Matrix Product

The given matrices are

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

A has size $2\times3$ and B has size $3\times2$,
so AB is defined and has size $2\times2$.

## 1. Identifying the columns of B

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix},
\qquad
b_2=
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}.
$$

## 2. Computing the two matrix-vector products

Multiply each row of A by the first column:

$$
Ab_1=
\begin{pmatrix}
1\cdot1+2(-1)+0\cdot3 \\
0\cdot1+1(-1)+1\cdot3 \\
\end{pmatrix}
=\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}.
$$

For the second column:

$$
Ab_2=
\begin{pmatrix}
1\cdot2+2\cdot0+0\cdot1 \\
0\cdot2+1\cdot0+1\cdot1 \\
\end{pmatrix}
=\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}.
$$

## 3. Computing AB directly

$$
AB=
\begin{pmatrix}
1\cdot1+2(-1)+0\cdot3 & 1\cdot2+2\cdot0+0\cdot1 \\
0\cdot1+1(-1)+1\cdot3 & 0\cdot2+1\cdot0+1\cdot1 \\
\end{pmatrix}
=\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

## 4. Comparison and explanation

The first column of AB equals Ab_1,
and the second column equals Ab_2:

$$
AB=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

This follows from the row-by-column rule.
To calculate column j of AB, every row of A is multiplied
by column j of B. These are exactly the calculations
that define the vector Ab_j.

Therefore, multiplying A by B applies A separately
to every column of B.

## Verification

Let

$$
u=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}.
$$

Then

$$
Bu=b_1+b_2=
\begin{pmatrix}
3 \\
-1 \\
4 \\
\end{pmatrix}.
$$

Applying A gives

$$
A(Bu)=
\begin{pmatrix}
3-2 \\
-1+4 \\
\end{pmatrix}
=\begin{pmatrix}
1 \\
3 \\
\end{pmatrix}.
$$

Using the computed product gives the same result:

$$
(AB)u=
\begin{pmatrix}
-1+2 \\
2+1 \\
\end{pmatrix}
=\begin{pmatrix}
1 \\
3 \\
\end{pmatrix}.
$$

Also, Ab_1+Ab_2=(1,3), consistent with both calculations.