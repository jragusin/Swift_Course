# For-In Loops
Used to iterate over an entire sequence.
# While Loop
Performs a set of statments until a conditional is false
# Repeat-While Loop
Performs a single pass of the Repeat block, then will evaluate the while condition
# If Loops
Executes a code block once if a condition is true. Can also contain else statments and else if statments.
# Switch
Considers a value and compares it to several possible values. The syntax is as follows:
```
switch value {
  case value_1:
    ...
  case value_2:
    ...
  default:
    ...  
}
```
# Control Transfer Statments
- Continue: tells a loop to stop what its doing and start again at the beginning of the next iteration
- Break: ends the execution of a control flow statment. Can be used to end a loop's iteration, or exit a switch statment
- Fallthrough: allows a switch statment to continue its execution after a matching case has been found. Useful is the default option is one that must happen regardless of case
# Labled Statments
Statments can be labled in Swift. This can be used to specify where a break should exit.
Lablenams should be placed before the loop followed by a colon (:)
# Guard
Executed the statments depending on the boolean value of an expression. GUard statments alwasy have an else statment. If the expression is false, the code in the else statment gets executed.
# Checking API Availability
You can use an availability condition in an if or guard statment to execute certain code blocks depending on the APi available. Syntax is as follows:
```
if #available([platform name] [version], ...) ...
```
