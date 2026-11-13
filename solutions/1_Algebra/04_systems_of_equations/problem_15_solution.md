# Exercise 15. Classifying Three Systems

## Question

For each of the following systems, perform only as much
elimination as necessary to recognize its type.

System 1:

$$
\begin{cases}
x+y=2, \\
x-y=0. \\
\end{cases}
$$

System 2:

$$
\begin{cases}
x+y=2, \\
2x+2y=4. \\
\end{cases}
$$

System 3:

$$
\begin{cases}
x+y=2, \\
2x+2y=5. \\
\end{cases}
$$

For each, justify the classification:
one solution, infinitely many solutions, or no solution.

## Solution

### 1. System 1: exactly one solution

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
1 & -1 & \mid & 0 \\
\end{pmatrix}.
$$

Apply

$$
R_2\leftarrow R_2-R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
\end{pmatrix}.
$$

There is a nonzero pivot for each variable
and no contradictory row.
Therefore, the system has exactly one solution.

No further elimination is needed to classify it.

### 2. System 2: infinitely many solutions

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 4 \\
\end{pmatrix}.
$$

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}.
$$

The zero row represents 0=0.
The system is consistent, but there is only one pivot
for two variables, leaving one free variable.

Therefore, the system has infinitely many solutions.

### 3. System 3: no solution

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 5 \\
\end{pmatrix}.
$$

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}.
$$

The last row represents 0=1, which is impossible.
Therefore, the system is inconsistent and has no solution.

### 4. Summary

| System | Classification | Reason |
|---|---|---|
| 1 | Exactly one solution | A pivot for each variable |
| 2 | Infinitely many solutions | Consistent with one free variable |
| 3 | No solution | Contradictory row |

One elimination operation per system is sufficient
to distinguish the three cases.