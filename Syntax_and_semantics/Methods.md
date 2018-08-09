# Methods

A method is a piece of code which can be called multiple times whenever it is needed.

The sintax is:

```coffee
let method_name(<arguments>) {
  # Body
}
```

Where: 
  * `method_name` can be replaced with the preferred one. It is recommended to choose a name which shortly describes what the method does. Underscore names are
    preferred to camel case ones.
  * <arguments> can be empty, or filled with a list of comma-separated arguments the method takes when invoked.
  
## Mandatory arguments

Unless it is specified, all arguments a method takes are mandatory:

```coffee
let sum(a,b) {
  return a + b
}

sum(5,8) #=> 13
sum(5)   #=> ArgumentError: Wrong number of arguments (1 instead of 2)
```

## Optional arguments

Optional arguments are the ones a default value has been provided. If another value is passed when calling a method, the default one is overwritten.

```coffee
let sum(a, b := 1) {
  return a + b
}

sum(5)   #=> 6
sum(5,8) #=> 13
```

# Calling methods

The interpreter operates a method call everytime a name is followed by an opened and a closed parethesi (with possible arguments between them).

```coffee
my_method() #=> calls method 'my_method'
```

A method call accepts an arbitrary number of arguments, but only the needed ones are taken. If the number is unsatisfactory, an error is raised.

```coffee
let sum(a,b) { return a +b }

sum(3,4)        #=> 7
sum(3,4,12,6,7) #=> 7
sum(8)          #=> ArgumentError: Wrong number of arguments (1 instead of 2)
```

# Method receiver

In LinCAS every method has a receiver, that is the object the method is invoked on:

```coffee
# here the receiver is '10'
10.zero? () #=> false 
```

If a method is just called without an explicit receiver, this last one is taken from the current scope:

```coffee
# This method is declared in the main scope (or program)
let foo() {
  puts self
}

foo() #=> <Object:@0x7fff5c02bad0>
```

Other details will be explained later

# Return values

A method always returns the values of the last executed expression. However an explicit `return` is supported

```coffee
# Method with no explicit return
let foo() { "Foo" }
foo() #=> Foo

# Method with explicit return
let baz() { return "Bazz" }
baz() #=> Bazz
``` 





