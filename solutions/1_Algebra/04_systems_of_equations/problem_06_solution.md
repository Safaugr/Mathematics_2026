# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Question

Analyze, depending on the parameter a, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4. \\
\end{cases}
$$

Among the three possibilities — exactly one solution,
infinitely many solutions, no solution — determine which
actually occur and for which values of a.
If one type cannot occur, explain why.

## Solution

### Elimination

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}.
$$

Apply

$$
R_2\leftarrow R_2-aR_1.
$$

This operation is valid for every real a and gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}.
$$

The second row represents the condition

$$
0=4-2a.
$$

### Case 1: a=2

The second row becomes 0=0 and adds no restriction.
The system reduces to x+y=2.

Set y=t. All solutions are

$$
(x,y)=(2-t,t),
\qquad t\in\mathbb{R}.
$$

Therefore, there are infinitely many solutions.

### Case 2: a different from 2

If a is not 2, then 4-2a is nonzero.
The second row requires zero to equal a nonzero number,
which is a contradiction.

Therefore, the system has no solution.

### Why a unique solution cannot occur

The second coefficient row is always a times the first.
It can never provide an independent equation.

Consequently, either one free variable remains,
or the equations contradict each other.
Exactly one solution is impossible for every value of a.

### Verification

For a=2 and the proposed solution family,

$$
(2-t)+t=2,
$$

$$
2(2-t)+2t=4.
$$

Both original equations hold for every real t.

For any solution of the first equation, multiplying it by a gives

$$
ax+ay=2a.
$$

The second equation requires this value to be 4,
so consistency is possible only when a=2.

### Conclusion

- For a=2, there are infinitely many solutions.
- For every other real a, there is no solution.
- No value of a gives exactly one solution.