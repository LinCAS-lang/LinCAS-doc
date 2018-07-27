# Symbol

Symbols are used to identify names in the code. They are a substitute of a string in the script, as they are more comfortable to use.

Symbols are usually created with the following sintax:

```Ruby
:name   # This is a symbol without quotes
:"name" # This is a symbol with quotes
:"12.3" # This is a symbol which needs quotes
```

But they can be created using the #to_sym() methods or other ones.

The difference between a symbol and a string is that a symbol is unique through the whole program.

With an example:

```Ruby
module One
{
    sym := :Frog
}

module Two
{
    sym := :Frog
}

sym := :Frog
```

In all the three cases the object is the same, despite of the three different contexts.


