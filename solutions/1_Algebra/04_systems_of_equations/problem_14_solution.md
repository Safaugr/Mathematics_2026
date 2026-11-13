# Exercise 14. A Small Change in the Right-Hand Side

## Question

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3, \\
\end{cases}
$$

and

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1. \\
\end{cases}
$$

Check the consistency of each system and explain
why a small change in one number can change
the type of the system.

## Solution

### 1. Solve the first two equations

Both systems share the equations

$$
x+y=2,\qquad 2x-y=1.
$$

Adding them gives

$$
3x=3,
\qquad x=1.
$$

Substituting into x+y=2 gives y=1.

Thus, any solution of either system must be (1,1).

### 2. First system

The third equation is 3x=3.
At x=1,

$$
3\cdot1=3.
$$

Therefore, the third equation is satisfied.
The first system is consistent and has exactly one solution:

$$
(x,y)=(1,1).
$$

Its third equation is the sum of the first two,
so it adds no new restriction.

### 3. Second system

The third equation now requires 3x=3.1.
But the first two equations already imply 3x=3.

Subtracting the sum of the first two equations
from the third gives

$$
0=3.1-(2+1)=0.1.
$$

This is a contradiction.
Therefore, the second system is inconsistent
and has no solution.

### 4. Confirmation using elimination

For both augmented matrices, apply

$$
R_2\leftarrow R_2-2R_1,
\qquad
R_3\leftarrow R_3-3R_1,
$$

followed by

$$
R_3\leftarrow R_3-R_2.
$$

For the first system, the result is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}.
$$

There are two pivots and no contradiction,
so the solution is unique.

For the second system, the result is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0.1 \\
\end{pmatrix}.
$$

Its final row represents the contradiction 0=0.1.

### 5. Explanation

The first two equations already determine x and y uniquely.
The third equation must agree with that solution.

Changing its right-hand side from 3 to 3.1
breaks this agreement. Exact equations must all hold
simultaneously, even when the discrepancy is small.

### 6. Verification of the first solution

For (x,y)=(1,1),

$$
1+1=2,\qquad 2\cdot1-1=1,\qquad 3\cdot1=3.
$$

All equations of the first system hold.
The third equation of the second system fails,
as expected.