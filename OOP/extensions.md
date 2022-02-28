#Extensions

Extensions can add functionality to an existing class, struct, enum, or protocol.
Extensions can:
- Add computed instanct properties and computed type properties
- Define instance methods and type methods
- Define subscripts
- Define and use new nested types
- Make an existing type conform to a protocol

## Extension Syntax
'''
extension SomeExtension {
  // new functionality
}
'''

Extensions can also be used to make an existing type conform to multiple protocols. This is done in the following way.
'''
extension SomeExtension: Protocol1, Protocol2 {
  // new functionality
}
'''

Extensions can also add computed type properties to existing types. For example:
'''
extension String {
  func scramble() -> String
    return "xxx\(self)xxx"
}
'''

It is also possible to add initializers to extensions in a similar manner.
