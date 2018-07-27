# If

An `if` statement is used to optionally execute a set of instructions.
It executes the given branch only if the condition has a **truthy** value, otherwise it executes the `else` branch if given.

The general sintax is:

```
if <condition> [then] {

  # code
  
} else {

  # code
  
}
```

The keyword `then` is optional and can be omitted as it's redundant.

The `else` branch can be omitted if it is not needed.

An example:

```CoffeeScript
a := 2

if a >= 2 {
  a *= 10
} else {
  a += 1
}

#=> 20

b := 1
if b > 2 {
  b := "bigger"
} else {
  b := "smaller equal"
}

#=> smaller equal
```









