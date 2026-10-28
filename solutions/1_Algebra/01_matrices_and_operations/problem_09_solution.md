# Exercise 9. Composing Transformations

The given matrices and vector are

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},
\qquad
R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix},
\qquad
x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}.
$$

S doubles the horizontal coordinate and preserves the vertical coordinate.
R rotates a vector through 90 degrees counterclockwise.

In a product acting on a vector, the rightmost transformation
is applied first.

## 1. Computing RSx

First apply S:

$$
Sx=
\begin{pmatrix}
2\cdot1+0\cdot2 \\
0\cdot1+1\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}.
$$

Then apply R:

$$
RSx=R(Sx)=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
=\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}.
$$

## 2. Computing SRx

First apply R:

$$
Rx=
\begin{pmatrix}
0\cdot1-1\cdot2 \\
1\cdot1+0\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}.
$$

Then apply S:

$$
SRx=S(Rx)=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
=\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

## 3. Geometric comparison

Scaling first sends $(1,2)$ to $(2,2)$.
Rotating this vector then gives $(-2,2)$.

Rotating first sends $(1,2)$ to $(-2,1)$.
Scaling then doubles its horizontal coordinate, giving $(-4,1)$.

The results differ because S scales only the horizontal direction.
Rotation changes which component lies in that direction,
so changing the order changes the result.

Thus,

$$
RSx\ne SRx.
$$

## Verification using matrix products

Direct multiplication gives

$$
RS=
\begin{pmatrix}
0 & -1 \\
2 & 0 \\
\end{pmatrix},
\qquad
SR=
\begin{pmatrix}
0 & -2 \\
1 & 0 \\
\end{pmatrix}.
$$

Applying these matrices to x gives

$$
(RS)x=
\begin{pmatrix}
0\cdot1-1\cdot2 \\
2\cdot1+0\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix},
$$

$$
(SR)x=
\begin{pmatrix}
0\cdot1-2\cdot2 \\
1\cdot1+0\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

These agree with the successive transformations calculated above.