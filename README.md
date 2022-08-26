# Driver Class

## Learning Goals

- Discuss what a Driver class is in Java

## What is a Driver?

Sometimes in Java, when we want to bring multiple classes together to
instantiate and call actions, we will create a **driver** or **runner** class.
A driver class is often just a class with a `main()` method so that it can be
made runnable in Java. We can import numerous classes to instantiate and execute
various methods to "drive" or "run" the program.

In the Inheritance lesson, we used a class `Main` to demonstrate how the `Cat`
and the `Parrot` classes were children of the `Animal` class, like so:

```java
package com.flatiron.animal;

public class Main {
   public static void main(String[] args) {
      Cat tom = new Cat();
      tom.setName("Tom");
      System.out.println("Hello! My name is " + tom.getName());
      tom.eat();
      tom.useLitter();

      Parrot polly = new Parrot();
      System.out.println("I'm a parrot and my name is " + polly.getName());
      polly.eat();
      polly.startFlying();
   }
}
```

Notice how the only purpose of the `Main` class was to instantiate our `Cat`
and `Parrot` instances and call on their methods. This is an example of a
driver class.
