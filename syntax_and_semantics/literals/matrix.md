# Matrix

A matrix represents a mathematical matrix containing generic values. This allows to make linear operations with matrices containing specific objects representing maths or other scientific datas.

It can be built with a literal in this way

```coffeescript
|"foo"|                     # Creates a 1x1 matrix
|1, 2, 3|                   # Creates a 1x3 matrix
|1, 2, 3; 4, 5, 6|          # Creates a 2x3 matrix
|1, 2, 3; 4, 5, 6; 7, 8, 9| # Creates a 3x3 matrix
```

