# Exercise 11. When Do Matrices Commute?

The given matrices are

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

## 1. Computing AB

Using the row-by-column multiplication rule,

$$
AB=
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix}.
$$

## 2. Computing BA

$$
BA=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}.
$$

## 3. Comparing corresponding entries

Two matrices are equal if and only if all corresponding
entries are equal. Therefore, AB=BA requires

$$
\begin{cases}
a+c=a, \\
b+d=a+b, \\
c=c, \\
d=c+d. \\
\end{cases}
$$

The first and fourth equations give $c=0$.
The second equation gives $d=a$.
The third equation is always satisfied.

Thus, the necessary conditions are

$$
c=0,\qquad d=a.
$$

There is no restriction on a or b.

## 4. General form and verification

Every possible matrix B must have the form

$$
B=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix},
\qquad a,b\in\mathbb{R}.
$$

Substituting this form into both products gives

$$
AB=
\begin{pmatrix}
a & b+a \\
0 & a \\
\end{pmatrix},
\qquad
BA=
\begin{pmatrix}
a & a+b \\
0 & a \\
\end{pmatrix}.
$$

Since $a+b=b+a$, these products are equal.

Therefore, the conditions $c=0$ and $d=a$ are both
necessary and sufficient for B to commute with A.