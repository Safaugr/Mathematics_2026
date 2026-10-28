# Exercise 14. Rotation Matrices

The matrix for a rotation through an angle theta is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

## 1. Multiplying the rotation matrices

Using row-by-column multiplication,

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha \\
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta \\
\end{pmatrix}
=\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta \\
\end{pmatrix}.
$$

## 2. Applying the angle-sum formulas

The trigonometric identities are

$$
\cos(\alpha+\beta)
=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
$$

$$
\sin(\alpha+\beta)
=\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

Substituting these expressions into the product gives

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}
=R(\alpha+\beta).
$$

## 3. Geometric interpretation

In the product R(alpha)R(beta), the rightmost matrix acts first.

A vector is first rotated through beta and then through alpha,
both about the origin. Its total change in direction is alpha+beta,
while its length remains unchanged.

Therefore, the composition is a rotation through alpha+beta.

## Verification with a numerical example

Take

$$
\alpha=\beta=\frac{\pi}{2}.
$$

Then

$$
R\left(\frac{\pi}{2}\right)=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

Multiplying gives

$$
R\left(\frac{\pi}{2}\right)
R\left(\frac{\pi}{2}\right)=
\begin{pmatrix}
-1 & 0 \\
0 & -1 \\
\end{pmatrix}
=R(\pi).
$$

Thus, two consecutive 90-degree rotations give a 180-degree
rotation, consistent with the general formula.