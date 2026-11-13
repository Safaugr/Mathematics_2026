# Exercise 7. Choosing a Method Deliberately

## Question

Do not solve all of the following systems completely.
For each situation, choose the method that best uses
its structure and justify your choice:

1. One system with a triangular coefficient matrix:

$$
\begin{cases}
2x-y=3, \\
4y=8. \\
\end{cases}
$$

2. Three systems Ax=b_i with the same invertible matrix A,
   when the inverse of A is already known.
3. One 3-by-3 system for which the inverse matrix is not given
   and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely.
For cases 2 and 3, describe the plan and indicate which part
of the computation would be reusable or unnecessary.

Do not judge a method by its name alone:
refer to the number of right-hand sides
and the structure of the matrix.

## Solution

### 1. Triangular system: back-substitution

The system is already upper triangular,
so no elimination or inverse calculation is needed.

The second equation gives

$$
4y=8,
\qquad
y=2.
$$

Substitute into the first equation:

$$
2x-2=3,
\qquad
x=\frac52.
$$

Therefore,

$$
(x,y)=\left(\frac52,2\right).
$$

Verification in the original equations gives

$$
2\left(\frac52\right)-2=3,
\qquad
4\cdot2=8.
$$

Both equations are satisfied.

### 2. Three right-hand sides: reuse the known inverse

Since the inverse of A is already available,
compute the three solution vectors using

$$
x_i=A^{-1}b_i,
\qquad i=1,2,3.
$$

The same inverse is reused for all three right-hand sides.
Each system requires only a matrix-vector multiplication.

There is no need to calculate the inverse again
or independently repeat elimination for each system.

Each result can be checked by computing Ax_i
and comparing it with the corresponding b_i.

### 3. One 3-by-3 system: Gaussian elimination

Form the augmented matrix with the coefficient matrix
and the single right-hand side.

Use elementary row operations to obtain row echelon form,
then back-substitute if there is a unique solution.

If elimination produces a contradiction, report no solution.
If it leaves free variables without a contradiction,
choose their values to obtain a solution vector.

Computing the entire inverse is unnecessary:
the goal is only one solution vector for one right-hand side.
Elimination works directly on that right-hand side
and also reveals whether the system is consistent.

Check any resulting vector by substituting it
into the original system.

If additional right-hand sides were introduced later,
the recorded elimination operations on A could be reused.
Here, however, only one right-hand side is required.