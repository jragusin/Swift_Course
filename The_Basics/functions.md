# Functions
Functions are self-contained chunks of code that perform a specific task
# Defining and Calling Functions
Syntax for defining functions is as follows:
```
func functionName([external label] [internal label] [parameterName]: Type, ...) -> returnType {
  // Some code
}
```
Syntax for coalling a function is as follows
```
functionName(paramName: parameter, ...)
```
Parameters must have their label in the function call is required.
Note that return values for functions can be ignored.

# Optional Tuple
A tuple that has the potential to have no value for the entire tuple.

# Implicit Return
Any function that is just one line can omit the return keyword. For example, these next two functions return the exact same thing
```
func greeting() -> String {
  return "Hello world!"
}

func greeting2() -> String {
  "Hello world!"
}
```
# Function Argument Labels
Each parameter has both an argument name and a paramter name.
## Omitting parameter names
Use an underscore (_) as a parameter name to omit it when makng a function call

## Default parameter values
You can include a default parameter value by assigning a parameter to a value in the function signature. If a value for the parameter is not passed in, it will be assigned the default value.

## Variadic Parameters
A variadic paramteter accepts zero or more vales of a specified type. You can use these to allow users to submit a varying number of input values. A variatic parameter will be passed into the function as an array of an appropriate type.

## In-Out Parameters
Use the inout keyword to pass a parameter by reference instead of value. This means that any changes done to the parameter inside of the function will change the original parameter itself.
Passing parameters into functions with an ampersand (&) in front of the parameter as an argument to an inout parameter.

## Functions as Return Types
It is possible to pass in a function as a parameter to another function. You can do this by writing a complete function after the arrow (->) 
