A simple math interpreter designed to solve basic linear equations with one variable.

## Syntax
### Addition
* **Example:** `1 + 1/x`
* **Commutative Property:** `x + 1`
* **Associative Property:** `1 + (2 + 3)x`

### Subtraction
* **Example:** `100 - 5x`
* **Non-Commutative:** `x - 12` (Order of operands matters)

### Multiplication
* **Example:** `(1 / x)x`
* **Commutative Property:** `1 * (2 + 3) * 4`
* **Associative Property:** `(1/x) * (1/(1/x))`
* **Distributive Property:** `3 * (k - 2)` or `5 * (2 * p + 1)`

### Division
* **Example:** `20 / 5`
* **Complex Division:** `2 / ((x + 5) / (x + 10))`

### Unary Operators & Nested Parentheses
* **Unary:** `--+456.789`
* **Nested:** `( ( (100 - 5*2) / 10 ) + --1 )`

## Equations
### Basic Linear Solving
* `x + 1 = 5` → **x = 4**
* `7y = 49` → **y = 7**

### Multi-variable / Polynomial Error
The system only supports linear equations with one variable. Multiplying variables or using different variable names will trigger an error.
* `x * x = 4` → **Error: Nonlinear equations (polynomials) not supported**
* `x + y = 10` → **Error: Multiple variables not supported**

### Infinite Solutions (Identity)
Occurs when both sides of the equation are identical after simplification.
* `2 * (3 * m + 5) = 6 * m + 10` → **Infinite Solutions**

### No Solution (Contradiction)
Occurs when the equation leads to an impossible statement.
* `4 * (a + 1) + 2 = 4 * a + 7` → **No Solution**
