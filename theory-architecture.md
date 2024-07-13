# Index

- [Behavioral Design Patterns](#behavioral-design-patterns)
  - [Chain of Responsibility](#chain-of-responsibility)
  - [Command](#command)
  - [Iterator](#iterator)
  - [Mediator](#mediator)
  - [Memento](#memento)
  - [Observer](#observer)
  - [State](#state)
  - [Strategy](#strategy)
  - [Template Method](#template-method)
  - [Visitor](#visitor)
- [Structural Design Patterns](#structural-design-patterns)
  - [Adapter](#adapter)
  - [Bridge](#bridge)
  - [Composite](#composite)
  - [Decorator](#decorator)
  - [Facade](#facade)
  - [Flyweight](#flyweight)
  - [Proxy](#proxy)
- [Creational Design Patterns](#creational-design-patterns)
  - [Factory Method](#factory-method)
  - [Abstract Factory](#abstract-factory)
  - [Builder](#builder)
  - [Prototype](#prototype)
  - [Singleton](#singleton)

## Behavioral Design Patterns

Behavioral design patterns are concerned with algorithms and the assignment of responsibilities between objects.
[Link to details](https://refactoring.guru/design-patterns/behavioral-patterns)

### Chain of Responsibility

**Chain of Responsibility** lets you pass requests along a chain of handlers. Upon receiving a request, each handler decides either to process the request or to pass it to the next handler in the chain.

[Back To Index](#index)

### Command

**Command** turns a request into a stand-alone object that contains all information about the request. This transformation lets you pass requests as a method arguments, delay or queue a request's execution, and support undoable operations.

[Back To Index](#index)

### Iterator

**Iterator** lets you traverse elements of a collection without exposing its underlying representation (list, stack, tree, etc.).

[Back To Index](#index)

### Mediator

**Mediator** lets you reduce chaotic dependencies between objects. The pattern restricts direct communications between the objects and forces them to collaborate only via a mediator object.

[Back To Index](#index)

### Memento

**Memento** lets you save and restore the previous state of an object without revealing the details of its implementation.

[Back To Index](#index)

### Observer

**Observer** lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they're observing.

[Back To Index](#index)

### State

**State** lets an object alter its behavior when its internal state changes. It appears as if the object changed its class.

[Back To Index](#index)

### Strategy

**Strategy** lets you define a family of algorithms, put each of them into a separate class, and make their objects interchangeable.

[Back To Index](#index)

### Template Method

**Template Method** defines the skeleton of an algorithm in the superclass but lets subclasses override specific steps of the algorithm without changing its structure.

[Back To Index](#index)

### Visitor

**Visitor** lets you separate algorithms from the objects on which they operate.

[Back To Index](#index)

## Structural Design Patterns

Structural design patterns explain how to assemble objects and classes into larger structures, while keeping these structures flexible and efficient.
[Link to details](https://refactoring.guru/design-patterns/structural-patterns)

### Adapter

**Adapter** allows objects with incompatible interfaces to collaborate.

[Back To Index](#index)

### Bridge

**Bridge** lets you split a large class or a set of closely related classes into two separate hierarchies—abstraction and implementation—which can be developed independently of each other.

[Back To Index](#index)

### Composite

**Composite** lets you compose objects into tree structures and then work with these structures as if they were individual objects.

[Back To Index](#index)

### Decorator

**Decorator** lets you attach new behaviors to objects by placing these objects inside special wrapper objects that contain the behaviors.

[Back To Index](#index)

### Facade

**Facade** provides a simplified interface to a library, a framework, or any other complex set of classes.

[Back To Index](#index)

### Flyweight

**Flyweight** lets you fit more objects into the available amount of RAM by sharing common parts of state between multiple objects instead of keeping all of the data in each object.

[Back To Index](#index)

### Proxy

**Proxy** lets you provide a substitute or placeholder for another object. A proxy controls access to the original object, allowing you to perform something either before or after the request gets through to the original object.

[Back To Index](#index)

## Creational Design Patterns

Creational design patterns provide various object creation mechanisms, which increase flexibility and reuse of existing code.
[Link to details](https://refactoring.guru/design-patterns/creational-patterns)

### Factory Method

**Factory Method** provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created.

[Back To Index](#index)

### Abstract Factory

**Abstract Factory** lets you produce families of related objects without specifying their concrete classes.

[Back To Index](#index)

### Builder

**Builder** lets you construct complex objects step by step. The pattern allows you to produce different types and representations of an object using the same construction code.

[Back To Index](#index)

### Prototype

**Prototype** lets you copy existing objects without making your code dependent on their classes.

[Back To Index](#index)

### Singleton

**Singleton** lets you ensure that a class has only one instance, while providing a global access point to this instance.

[Back To Index](#index)
