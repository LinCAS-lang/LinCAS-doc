# Symbolic function

A bit more interesting example is a symbolic function:

```CoffeeScript
function := ${ 2 * x + x * y }
printl "Calculating df/dx of ".concat( function.to_s() )
printl function.diff(${ x })

#=> Calculating df/dx of 2 * x + x * y
#=> 2 + y
```

This example would be clearer after reading all the documentation, but we can understand somethong as well.

* You can define local valiables without the need of declaring their types, and assignments use the convention
  of `:=` 

  ```CoffeeScript
  function := ${ 2 * x + x * y }
  ```
  
* You can create symbolic functions just enclosing them between `${}`
  
  ```CoffeeScript
  ${ 2 * x + x * y }
  ```
  
* You program by invoking methods to objects

  ```CoffeeScript
  printl "Calculating df/dx of ".concat( function.to_s() )
  ...
  printl function.diff(${ x })
  ```
  
* Method calls are identified by the two parenthesis at the end of the name

  ```CoffeeScript
  function.to_s()
  ```
  
  
  
  
