# Select

A `select` statement is a structure which works a bit like an if statement comparing the given value with the conditions using the `==` method.

The general sintax is

```CoffeeScript
select exp 
{
  case val1, val2, val3 
  {
    # some code
  }
  
  case val4 
  {
    # some code
  }
  
  else 
  {
    # some code
  }
}

# which is the same as


if exp == val1 || exp == val2 || exp == val3 {
  # some code
} elsif exp == val4 {
  # some code
} else {
  # some code
}
```

This structure is more comfortable and readable than an [if]({{ "/If.md" | relative_url }})
















