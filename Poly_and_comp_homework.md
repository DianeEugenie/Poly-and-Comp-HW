## Polymorphism

#### What does the word 'polymorphism' mean?
**Poly** means *many* and **morph** means *form* or *change*. *Polymorphism* is the ability of an object to take many forms.

#### What does it mean when we apply polymorphism to OO design? Give a simple Java example.

When we apply *polymorphism* to an OO design, we can give variables, functions or objects the ability to take on many forms. For example, we can use one parent class which is abstract as a blue print for all the child classes. This enables us if we wish to add a *motorbike* to an `ArrayList` for `<Vehicle>` and a *speedboat* to the same `<Vehicle>`. Both extend the abstract class of `Vehicle` and are therefore *morphs* or *different forms of* `Vehicle`. Essentially, an instance of a class as if it was a different class but a different type.

#### What can we use to implement polymorphism in Java?

We can use either **interfaces** or **abstract classes** (**inheritance**) to implement polymorphism. Interfaces can be implemented by classes and abstract classes can be extended by concrete classes. Anything with a parent class or extends an abstract class.

*Same method different implementations*
 *Method overloading add(int num1, int num2), add(double num1, double2 num2) can exist in the same file even though they have the same name.*

#### How many 'forms' can an object take when using polymorphism?

Infinite amount. With regards to the `Vehicle`, we can create many different vehicle types that extend the properties and functionalities of the `Vehicle`. But a concrete class can **only extend one** abstract class or parent class. But the same concrete class would be able to **implement many interfaces**.

#### Give an example of when you could use polymorphism.
When you are coding and realise that many of the components have similar functions and properties, that would be an ideal case to use polymorphism. Gathering different types into one collection `ArrayList<Vehicle>`. Bear belly, Salmon -> only can eat salmon, different classes with an `IEat` interface and belly an array of edible things. So bear can eat anything that implements `IEat`.

## Composition

#### What do we mean by 'composition' in reference to object-oriented programming?

By **composition** in OOP, we see objects as being made of or **composed** of other objects. For example, a Car has an engine and has wheels and so does a motorbike.

Composition refers to a HAS-A relationship in the way that a car has an engine and a motorbike has an engine. But in the same way when the car has the engine, the ownership of that engine is handed over to the car.

#### When would you use composition? Provide a simple example in Java.

You would use composition if you would like an object to use behaviours of other classes. Composition also makes it possible for that behaviour to change at runtime.

For example, a car is composed of an engine, of doors, of a gearbox. These components could have their own functionalities and by adding these to the car, the car will have access to the functionalities of the components.

*Composition over inheritance* means that we should compose our classes from other classes that carry out behaviours we need. Instead of having objects inherit from other objects and them inheriting from others etc.

*Identify the objects - does it have its own properties, does it need its own methods - YES? create new object as component and use composition.*


#### What is/are the advantage(s) of using composition?

Composition is *flexible*. An object can be composed of many interfaces, but an object can only inherit once. Java only allows one inheritance but multiple compositions (interfaces). Can swap out any kind of engine in a vehicle for example.

Composition allows you to stick to *Encapsulation*. One object is in charge of all of its behaviours.

Composition allows you to *reuse existing code* by giving an object behaviours that have already been written. Without having to rely on inheritance,

Composition allows you to *change an implementation* of a behaviour *without adapting any external classes* that use that behaviour. e.g. the interface `ISecurity` in the theme park, where different attractions and stall had different security measures with regards to the height and the age of the visitor.

#### When an object is destroyed, what happens to all the objects it is composed of?

Because an object is composed of other behaviours owns those behaviours, as soon as we destroy an object, the behaviours of this object are also destroyed.


*Garbage collection in Java goes through memory and removes all that has been destroyed.*
