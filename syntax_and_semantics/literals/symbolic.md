# Symbolic

A symbolic is a representation of numbers, variables and other mathematics elements for symbolic computation.

Every element can be built through its specific class or as a literal:

```coffeescript
${ 1 }         # Returns a symbolic number
${ x }         # Returns a symbolic representation of a variable 
${ 2 * x + 1 } # Returns a symbolic function
```

