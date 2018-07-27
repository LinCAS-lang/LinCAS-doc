# Hash

A hash represents a table of keys with an associated value.

Users must be careful with method aliases: this type has methods which modify the content of a hash, and others which return a new one. The first ones usually end with `!`, but there are some exceptions like `Hash#[]=`

To create a hash with a literal, just use the following sintax:

```Ruby
{}                       # Creates an empty hash
{:foo => 1, :bar => 2}   # Creates a hash table with two two keys
{1 => "foo", 2 => "bar"} # Creates a hash table with integers as keys
```

Keys and values are generic types.

If a key is added or deleted, the size of the hash is automatically resized. 
