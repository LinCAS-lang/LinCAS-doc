# While

A `while` loop exetutes its block as long as the condition is **truthy**

```coffeescript
[do] while <condition> 
{
  # Some code
}
```

The keyword `do` can be omitted as not really useful.

When a `while` statement is executed, its condition is tested first, and if it is **truthy** the block is executed. This means the code might never be executed.

