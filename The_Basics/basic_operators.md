# Basic Operators
Operators are special symbols used to check, change, or combine values.
- Unary Operators: Operate on a single target
- Binary Operators: Operate on two targets and appear between their two targets
- Ternary Opertors: OPerate on 3 targets. Swift only has one ternary operator, the ternary conditional operator (a ? b : c)

# Assignment Operator (=)
Used to assign or update the value of a variable or constant.

# Arithmetic Operators (+, -, *, /)
The four standard arithmetic operators for all number types. In Swft, operators do not allow values to overflow by default.

# Remainder (Modulus) Operator (%)
Used to find the remainder of dividing two numbers.
```
var remainder = 15 % 4 // remaainder = 3
```
# Unary Minus Operator (-)
Toggles the sign of a numeric value

# Unary Plus Operator (+)
Returns the value it operates on without any change. Not sure why this exists.

# Nil-Coalescing Operator (a ?? b)
Used to unwrap an optional is it is not nil. It is the same as the following:
```
a != nul ? a!: b
```
# Range Operators
## Closed Range Operator (a...b)
Defines a rnage that runs from a to b inclusive
## Half-Open Range Operator (a..<b)
Defines a range tht runs from a to b without including b
## One-Sided Ranges (a...), (...<a)
Defines a range starting at a and continuing as long as possible. Can also be used to start at 0 and go until a by using the second syntax.


