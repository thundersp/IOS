## Operators and Control Flow

### If else
```
let x = 5
if x % 2 == 0 {
    print("x is even")
} else {
    print("x is odd")
}
```
We use if else for control flow, do not use parentheses for conditions. We can create if else ladder for multiple conditions.
```
let x = 2
let y = 3
if x % 2 == 0 && y % 2 == 0 {
    print("Both x and y are even")
} else if x % 2 == 0 {
    print("x is even")
} else if y % 2 == 0 {
    print("y is even")
} else {
    print("Both x and y are odd")
}
```
&& is used for AND and || is used for OR.

### Using switch statements

```
let x = 5
switch x {
case 0:
    print("x is zero")
case 1:
    print("x is one")
case 2:
    print("x is two")
case 3:
    print("x is three")
case 4:
    print("x is four")
default:
    print("x is not zero or one")
}
```

### Boolean Expressions and Type checking

```
let number = 100
let isSmall = number < 10
print("The type of isSmall is \(type(of: isSmall))")
```
In the above, the number < 10 is a boolean expression, which evaluates to either true or false, stores the value in the variable isSmall, and printss its type. Type of variable is accessed by using type(of: variableName).

