# Exercise 8. Row Operations and Their Reversibility

The given matrix is

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}.
$$

## 1. First row operation

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

The new second row is

$$
(2,4,1)-2(1,2,-1)=(0,0,3).
$$

The other rows remain unchanged, giving

$$
A_1=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}.
$$

## 2. Second row operation

Apply to the current matrix

$$
R_3\leftarrow R_3+R_1.
$$

The new third row is

$$
(-1,1,3)+(1,2,-1)=(0,3,2).
$$

Therefore,

$$
A_2=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}.
$$

## 3. Third row operation

Interchange the second and third rows:

$$
R_2\leftrightarrow R_3.
$$

The resulting matrix is

$$
A_3=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}.
$$

## 4. Inverse operations

Each operation can be reversed:

| Original operation | Inverse operation |
|---|---|
| $R_2\leftarrow R_2-2R_1$ | $R_2\leftarrow R_2+2R_1$ |
| $R_3\leftarrow R_3+R_1$ | $R_3\leftarrow R_3-R_1$ |
| $R_2\leftrightarrow R_3$ | $R_2\leftrightarrow R_3$ |

Adding a multiple of another row is reversed by subtracting
the same multiple. Swapping two rows is reversed by swapping
them again.

## Verification

To recover A from the final matrix, undo the operations
in reverse order.

First, swap rows 2 and 3:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}.
$$

Next, subtract row 1 from row 3:

$$
(0,3,2)-(1,2,-1)=(-1,1,3).
$$

Finally, add twice row 1 to row 2:

$$
(0,0,3)+2(1,2,-1)=(2,4,1).
$$

The recovered matrix is

$$
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
=A.
$$

Thus, all three operations are reversible.