Swift is the programming language used for iOS, macOS, watchOS, and tvOS apps.

# Data Types
Swift has its own fundmental types.
- Int - Integer types
- Double and Float - floating-point values
- Bool - Boolean values
- String - Textual Data

# Collection Types
Swift also uses collection types to store collections of values.
- Arrays: Store values in an ordered list. The same value can appear in different spots.
- Sets: Stored distinct values in an unordered collection.
- Dictionaries: Stores an association between key-value pairs in an unordered collection.

# Constants and Variables
Constants and variables must be declared before they can be used. They must be initialized to a value.

Constants can be declared using the 'let' keyword like:
```
let age = 5 // Constant declaration
```

Variables can be declared using the 'var' keyword like:
```
var age = 5 // Variable declaration
```

# Type Annotation
You can provide a type when declaring a constant or variable to be clear about the type the variable can store.
This is done by using a colon followed by the type For example:
```
var age:Int = 5 // Type Annotation
```
# Naming Constants and Variables
Constants and variables can contain almost any unicode character in their name.
They cannot contain any whitespace, mathematical symbols (<, >, etc), or begin with a number.
Their names must be unique if they are declared in the same scope. 
# Printing Constants and Variables
The value of a constant or variable can be printed using the print() function.
Swift uses sting interpolation to include the name of a constant or variable as a placeholder in a longer string. For examlple:
```
var age:Int = 20
print("My age is \(age)") // String interpolation
```
# Integers
Whole numbers with no fractional component. Swift provides signed and unsigned integers in 8, 16,32, and 64 bit forms.
The convention for these types is simlar to C. For example, an unsigned 8-bit integer would be of type UInt8.
## Int Bounds
The size of he Int type depends on the platform's native size:
- On a 32-bit platform, Int is the same size as Int32
- On a 64-bit platform, Int is the same size as Int64
Same goes for unsigned ints

# Type Safety and Type Inference
Swift is type safe. If a type is not declared for a variable upon declaration, Swift will infer the type based on it's initialized value.
# Numeric Literals
- A decimal number has no prefix
- A binary number has 0b as a prefix
- An octal number has 0o as a prefix
- A hexadecial unmber has 0x as a prefix
# Type Aliases
Type aliases define alternative names for an existing type using the typealias keyword. For example:
```
typealias AudioSample = UInt16
var amplitude = AudioSample.min
```

# Tuples
Tuples are groups of multiples values bundles into a single compound value.
Tuples can be created using any premutation of types and as many types as you'd like.

## Decompose a tuple
You can decompose a tuple's contents into separate constants of variables like:
```
let (statusCode, statusMessage) = http404Error
```
## Ignoring tuple values
If you'd like to ignore parts of a tuple, use the underscore (_) to do so.
## Accessing individual tuple parts
Individual tupke parts can be accessed like array elements.
```
let exampleTuple = (404, "Error")
let errorNumber = exampleTuple.0 // 404
let errorMessage = exampleTuple.1 // "Error"
```
You can also lable these parts when a tuple is defined
```
let a = (statusCode: 404, message: "Error")
let code = a.statusCode // 404
let errorMessage = a.message  // "Error"
```
# Optionals
You can use optionals when dealing with values that may be null (nil in Swift). This can be done by adding a question mark (?) to the end of a variables' type.
```
var age:Int? = 5 // Optional Int
```
# Optional Binding
You can use optional binding to check for a value inside of an optional variable. This can be donw as follows:
```
if let [constant name] = [some optional] {
  // Some code ...
}
```
This is a very safe way to check that an optional is not null as the code inside of the let if loop will only be executed if the optional is not null.
# Unwrapped Optionals
It is possible to unwrap optional by force using a (!). Do not do this, as there are not checks to account for nil values
# Error Handling
Very siilar to Java. Functions that throw errors are marked by the 'throws' keyword. The potential errors must be caught by the caller.
Swift used Do-Catch blocks to catch errors. The structure of this is as follows:
```
do {
  try canThrowAnError()
  // The following lines in this block are executed if no error was thrown
} catch {
  // If an error was thrown, the code in this block will be executed
}
```
Do statments create a new containing scope, which allows errors to be propogated through catch clauses.
# Assertions and Preconditions
These are checks done at runtime. These are done to make sure essential checks are donw before any code is executed. If any precondition of assertions is not valid, then the code program will be terminated.
Assertions are only checked in debug builds, while preconditions are checked in debug builds and production.
