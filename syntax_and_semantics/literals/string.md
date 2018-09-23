# String

A string is a sequence of UTF-8 characters enclosed betweend double quotes.

Up to now no special characters have been introduced \(like '\n' or similar\) nor particular string options like string interpolation, but they're planned to be implemented in future.

Users must be careful with method aliases: this type has methods which modify the content of a sring, and others which return a new one. The first ones usually end with `!`, but there are some exceptions like `String#[]=`

The main way to create a string is:

```coffeescript
"Hello, world"
```

A string can span multiple lines:

```coffeescript
"This 
  string 
spans across multiple 
lines"

#=> This
      string
    spans across multiple
    lines
```

