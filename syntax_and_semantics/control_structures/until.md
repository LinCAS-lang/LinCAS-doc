# Until

An `until` loop executes its body as long as the condition is **falsey**.

```coffeescript
do
  # some code
until <condition>
```

The main difference with a `while` loop is the block of code is first execuded, then the condition is checked. This means the code is executed at least once.

As you can see it is not necessary to enclose the code between braces as it is surrounded by the keywords `do` and `until`

