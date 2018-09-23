# Array

Arrays are generic auto-resizing containers of elements, and they are usually created with literals

```ruby
[]                     # Creates an empty array
[1,3,2]                # Creates an array with three elements of integer type
["foo",:bar,123,12.6]  # Creates an array with four elements of generic type
["foo"] << 12          #=> ["foo",12]  /* it auto-resizes the length of the array from 1 to 2 */
```

The maximum size of an array is set to 10,000.

Users must be careful with method aliases: this type has methods which modify the content of an array, and others which return a new one. The first ones usually end with `!`, but there are some exceptions like `Array#[]=`

