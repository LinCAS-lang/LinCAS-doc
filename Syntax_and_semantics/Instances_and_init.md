# Instances and initialization

You create instances of a class through the keyword `new`:

```CofeeScript
dog := new Dog()
```

Parenthesis after the class names are mandatory.

Now we have an instance of class `Dog`.

Since an object respons to some method, as said in its definition, we can add some as we wand our dog to have some behavour. For instance when we create an object `Dog` we want to give it a name, and we can store in in an instance variable which is prefixed with the symbol `@`. And of course we want to retrive its name a a later moment.

To give our dog a name when we create the object, we can use the `init` method that is called everytime a class is instantiated. It is also called constructor of a class and it is used just to *initialize* the object state (eg. its instance variables)

```CoffeeScript
class Dog
{
    let init(name) {
        @name := name
    }
    
    let name() {
        @name
    }
}
``` 

Now our class is ready enough to create dogs in this way:

```CoffeeScript
bobby := new Dog("Bobby")
lexi  := new Dog("Lexi")

bobby.name() #=> Bobby
lexi.name()  #=> Lexi
```

When we created `Dog` instances, we never actually called 'init'. This is because the interpreter does it for us passing the arguments we put between parenthesis (after the class name) to the method itself.

























