Swift provides 3 primary collection types: arrays, sets, and dictionaries.
# Arrays
An array sotres values of the same type in an ordered list.
# Array Type Shorthand Syntax
The type of an array in Swift is written in full as Array<Element> where element is the type of the values stored in the array
# Iterating Over an Array
You can iterate over the entire set of values in an array by using a for-in loop.
```
for item in shoppingList {
  // Some code
}
```
# Sets
A set stores distinct values in an unordered collection
## Hash values for set types
A type must be hashable in order to be stored in a set. All of Swift's primative types are hashable.
## Set Type Syntax
The type of a set in Swift is written as Set<Element> where Element is the type of values stored within the set
## Accessing and modifying a Set
 Use the insert method to add an eleemnt to a set.
 Use the remove method to remove an element from a set.
## Set Operations
- Intersection: Contians only common values shared by two sets
- symmetricDifference: Contains only values that are not shared by both sets
- Union: Contains all emelents in both sets
- Subtraction: Contains the elements in the first set minus the elements that are shared with the second set
## Set membership and Equality
  - is equal (==) is used to see if two sets contain all f the same values
  - isSubset() returns true if a set's values are contained within another set
  - isSuperset returns true if a set contains all values within another set
  - isDisjoint returns true if two sets have no values in common
  - isStrictSubset() & isStrictSuperset() return true if a set is a subset or super set of another and not equal to another set
# Dictionaries
  Stores association between key-value pairs of the same type in a collection with no defined ordering
  ## Type Shorthand
  Dictionary types can be written in full as Dictionary<Key, Value> or shorthand as [Key: Value]
  ## Creating an empty dictionary
  ```
  var myDict: [Int: String] = [:] // Empty Dictionary
  ```
  ## Accessing and Modifying a Dictionary
  - Use the isEmpty() method to determine if a dictionary has no key-value pairs
  - Use subscript syntax (dict[key] = value) to add an element to the dictionary or change a key-value pair
  - updateValue() can be used to set or update the value for a specific key. It returns the old value (or nil) after performing an update.
  - removeValue() can be used to remove a key-value pair from the dictionary
