# For

A `for` loop executes its body a fixed number of times and provides a counter automatically increased every cycle.

```CofeeScript
for i : 1 to 10 
{
  # some code
}

# The above code is the same as

i := 1
while i <= 10
{
  # some code
  i += 1
}
```

This kind of loop is very useful on arrays, matrices and all those container objects we know the size in advance.

For instance: 

```CofeeScript
a := [1,2,3,4,5]
for i : 1 to a.size()
{
  a[i - 1] += 3
}

#=> [4,5,6,7,8]
```

There also is the possibility of an inverse loop, that is from n to m having n > m. The counter is automatically decreased.

```CoffeeScript
for i : 10 downto 1
{
  # some code
}

# Same as

i := 10
while i >= 1
{
  # some code
  i -= 1
}
```









 
