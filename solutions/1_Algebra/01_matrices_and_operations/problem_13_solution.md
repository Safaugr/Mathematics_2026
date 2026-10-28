# Exercise 13. A Recurrence Written in Matrix Form

The given matrix is

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

## 1. Computing successive powers

Using row-by-column multiplication,

$$
F^2=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}.
$$

Next,

$$
F^3=F^2F=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
=\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

Similarly,

$$
F^4=F^3F=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
=\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix},
$$

$$
F^5=F^4F=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
=\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}.
$$

## 2. Connection with the Fibonacci sequence

Define the Fibonacci numbers by

$$
f_0=0,\qquad f_1=1,\qquad f_{n+1}=f_n+f_{n-1}.
$$

This gives the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

The matrix powers contain consecutive Fibonacci numbers.
The observed pattern is

$$
F^n=
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1} \\
\end{pmatrix},
\qquad n\ge1.
$$

For example, F^5 contains $f_6=8$, $f_5=5$, and $f_4=3$.

## 3. One recurrence step

For any numbers a and b,

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
=\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}.
$$

The first component is the sum of the two input numbers.
The second component keeps the previous first component.

If $a=f_{k+1}$ and $b=f_k$, the output is

$$
\begin{pmatrix}
f_{k+2} \\
f_{k+1} \\
\end{pmatrix}.
$$

Thus, multiplying by F advances a pair of consecutive
Fibonacci numbers by one step.

## Verification of the general pattern

For n=1, the proposed formula gives F.

Assume the formula holds for some integer $n\ge1$.
Then

$$
F^{n+1}=F^nF=
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1} \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
=\begin{pmatrix}
f_{n+1}+f_n & f_{n+1} \\
f_n+f_{n-1} & f_n \\
\end{pmatrix}
=\begin{pmatrix}
f_{n+2} & f_{n+1} \\
f_{n+1} & f_n \\
\end{pmatrix}.
$$

This is the same formula for n+1, so the pattern follows
by mathematical induction.