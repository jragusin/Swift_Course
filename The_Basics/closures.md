# Closures
Closures are self-contained blocks of functionality that can be passed around and used in different ways. They are basically lambda functions.

## The Sorted Method
Sorted in included in the Swift standard library. This method can accept a closure that takes two arguments of the same type. This closure compares the two items and should return true if the first item should appear before the second item. This can be done either inline or as a separate function entirely.

## Closure Expression Syntax
Closure expressions generally have the following syntax:
```
{ (parameters) -> return type in 
  statments...
}
```
The parameters cannot have a default value.
## Inferred Type from Context
It is always possible to infer the parameter's type when passing a closure as a parameter to a function.
For example, a cllsure can be reduced to the following:
```
array.sorted(by: { s1, s2 in s1 > s2 })
```
## Shorthand Argument Names
Swift provides shorthand argument names for closures. These are denoted as $0, $1, ... etc. This allows closures to be reduced even more. For example, using shorthand notation, we can resuce a closure to the following:
```
array.sorted(by: { $0 > $1 }
```
## Capturing Values in a Closure
A closure can be used to capture and store values from the surrounding context in which it is defined. 
This is done by defining a variable/constant inside of a closure and returning a function that interacts with that vairble/constant from the closure.

## Closures as Reference Type
When you assign a function or closure to a constant or variable, they are used as references to the function or closure. Meaning the function or closure can act as a pointer.
