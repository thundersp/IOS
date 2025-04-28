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
We dont need to use parentheses for conditions in switch statements, or break statements.
```
let age = 25
switch age {
case 0...10:
    print("age is between 0 and 10")
case 11...20:
    print("age is between 11 and 20")
case 21...30:
    print("age is between 21 and 30")
default:
    print("age is not between 0 and 30")
}
```

We can use 0...10 to define range between which the value will be checked against, inclusive of the two values. 
```
let day = "tuesday"
switch day.lowercased(){
case "monday", "tuesday", "wednesday", "thursday", "friday":
    print("Weekday")
case "saturday", "sunday":
    print("Weekend")
default:
    print("Invalid day")
}
```

We can pass multiple values to a case statement, separated by commas, to check if the value matches any of the values.

### Boolean Expressions and Type checking

```
let number = 100
let isSmall = number < 10
print("The type of isSmall is \(type(of: isSmall))")
```
In the above, the number < 10 is a boolean expression, which evaluates to either true or false, stores the value in the variable isSmall, and printss its type. Type of variable is accessed by using type(of: variableName).

