# Static methods

A static method is a kind of method that can be called without the object is created as it doesn't depend on the instance.
It is the same concept of class (or singleton) methods in other languages such as Ruby and Crystal.

To define a static method, you have to put the keyword `slef` (or the class name) before its name

```coffee
class Foo
{
    let self.bar() {
        printl "I am a class method"
    }
    
    let Foo.baz() {
        printl "Bazz"
    }
}

Foo.bar() #=> I am a class method
Foo.baz() #=> Bazz
```

In other words these are methods whose receiver is the class itself. In fact they are not accessible from the instances.
