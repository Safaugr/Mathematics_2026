# Exercise 3. When Can Matrices Be Multiplied?

The given matrix sizes are:

- A: $2\times3$
- B: $3\times4$
- C: $4\times2$
- D: $2\times2$

## Rule

A matrix product is defined when the number of columns
of the first matrix equals the number of rows of the second.

If the sizes are $(m\times n)(n\times p)$,
the product has size $m\times p$.

## Results

| Product | Sizes | Compatibility | Result |
|---|---|---|---|
| AB | $(2\times3)(3\times4)$ | $3=3$ | Defined: $2\times4$ |
| BA | $(3\times4)(2\times3)$ | $4\ne2$ | Not defined |
| BC | $(3\times4)(4\times2)$ | $4=4$ | Defined: $3\times2$ |
| CB | $(4\times2)(3\times4)$ | $2\ne3$ | Not defined |
| AC | $(2\times3)(4\times2)$ | $3\ne4$ | Not defined |
| CA | $(4\times2)(2\times3)$ | $2=2$ | Defined: $4\times3$ |
| AD | $(2\times3)(2\times2)$ | $3\ne2$ | Not defined |
| DA | $(2\times2)(2\times3)$ | $2=2$ | Defined: $2\times3$ |

## Explanation and Verification

Each entry of a product is the dot product of a row
of the first matrix and a column of the second.
These vectors must have the same number of entries.

For AB, both vectors have 3 entries, so multiplication
is possible. The result has 2 rows from A and 4 columns from B.

For BA, a row of B has 4 entries but a column of A has 2,
so the required dot product cannot be formed.

The same compatibility check is shown for every product
in the table. In each defined product, the result keeps
the row count of the first matrix and the column count
of the second.