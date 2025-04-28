## Variable declaration in swift

Variable declared using let and var keywords, key difference between them is that let is immutable (constant) and var is mutable. 
```
let pi = 3.14159
var radius: Double = 5.0
print("pi is \(pi)")
```
pi is implicitly inferred as double with a value of 3.14159.
radius is explicitly declared as a variable with a value of 5.0.
To view the data type of variable, hold option and click on the variable name.
Once a type is declared/inferred, it cannot be changed. It will result in a compile-time error if you try to change it. once a bool always a boolean value.
We can declare a variable without value by defining it's type. (Double, string etc)

```
let x = 5
let y = 2.5
let z = x * y
```
The above will not compile because x and y are of different types. To fix this, we can convert x to a float or y to an integer.
```
let x = 5
let y = 2.5
let z = Double(x) * y
```
OR 
```
let x = 5
let y = 2.5
let z = x * Int(y) //2.5 will turn into 2
```

## Printing values

Use \\() to print value of Variables. It's known as string interpolation. You can evaluate the expression inside the parentheses and print the result. \\(2+3) 

## Types of data Types

Int, Double, Float, Bool, String, Character

## Types of Collections

Array, Dictionary, Set, Tuples

## Reading input

Use the readline() to take input from user. It returns a optional string value, bcz the input can end unexpectedly. It returns nil if the input is empty or if the input is interrupted by a signal. Use optional binding to handle the optional value returned by readline(). 
```
if let input = readline() {
    print("You entered: \(input)")
} else {
    print("No input provided")
}
```
if let input = readline() is used to safely take input, if no input is provided, else statement is executed.
Convert the input to other data types Using Int(), that is data type with (). Thus to take input,
```
if let firstNumber = readLine(), let first = Int(firstNumber) {
    if let secondNumber = readLine(), let second = Int(secondNumber) {
        print("First number: \(first)")
        print("Second number: \(second)")
    } else {
        print("Invalid second input")
    }
} else {
    print("Invalid input")
}