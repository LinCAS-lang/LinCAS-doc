# Constants

LinCAS provides two ways to create constants; The first one involves the keyword `const`

```coffeescript
const MyConst := 12
```

Names of constants can begin with lowcase or capital letters, but the suggested convention is to use the capital letter: this in order not to confuse them with local variables.

The second way to create a constant uses the character `&`, but it is not recommended as it makes the code less clear

```coffeescript
&MyConst := 12
```

This second way has been introduced to avoid possible collisions between constants and local variable names. LinCAS allows these elements to have the same name, since they're treated differently. When a name is searched and it can be referred to both a constant or a variable in a scope, the interpreter first looks in the local variables scope, and if no variable is found, a constant is searched.

But if we want to force the interpreter to look for a constant \(as we are sure it exists\) we put the `&` character before the name

```coffeescript
const var := 12
var := "foo"

var  #=> "foo"
&var #=> 12
```

Constants can never be reassigned. An exception is raised if done.

