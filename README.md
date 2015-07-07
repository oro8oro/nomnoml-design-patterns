# Nomnoml Design Patterns

In this project we present the well-known OOP design patterns from the [GoF Book]( https://en.wikipedia.org/wiki/Design_Patterns) in [Nomnoml](http://www.nomnoml.com)

For the Javascript implementation see: [js-design-patterns](http://loredanacirstea.github.io/js-design-patterns)

Images were generated by [Nomnoml](http://www.nomnoml.com) from the .uml file. Also by sequence diagrams .seq file.

Everyone is welcome to improve on this and provide implementation in various programming languages.

* [Creational Patterns](#creational-patterns)
	* [Abstract Factory](#abstract-factory)
	* [Builder](#builder)
	* [Factory Method](#factory-method)
	* [Prototype](#prototype)
	* [Singleton](#singleton)

* [Structural Patterns](#structural-patterns)
	* [Adapter](#adapter)
	* [Bridge](#bridge)
	* [Composite](#composite)
	* [Decorator](#decorator)
	* [Façade](#façade)
	* [Flyweight](#flyweight)
	* [Proxy](#proxy)

* [Behavioral Patterns](#behavioral-patterns)
	* [Chain of Responsibility](#chain-of-responsibility)
	* [Command](#command)
	* [Interpreter](#interpreter)
	* [Iterator](#iterator)
	* [Mediator](#mediator)
	* [Memento](#memento)
	* [Observer](#observer)
	* [State](#state)
	* [Strategy](#strategy)
	* [Template Method](#template-method)
	* [Visitor](#visitor)



## Creational Patterns
### Abstract Factory

![Abstract Factory](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/creational/abstract_factory/abstract_factory.png)

```
[<abstract>AbstractFactory
	|
	| +createProductA()
	 +createProductB()
]

[AbstractFactory]<:-[ConcreteFactory1
	|
	| +createProductA()
	 +createProductB()
]

[AbstractFactory]<:-[ConcreteFactory2
	|
	| +createProductA()
	 +createProductB()
]

[AbstractFactory]<-[Client
	(from design_patterns)
	|
	| 
]

[Client]->[<abstract>AbstractProductA
	|
	| 
]

[AbstractProductA]<:-[ProductA1
	|
	|

]

[AbstractProductA]<:-[ProductA2
	|
	|

]

[<abstract>AbstractProductB
	|
	| 
]

[AbstractProductB]<:-[ProductB1
	|
	|

]

[AbstractProductB]<:-[ProductB2
	|
	|

]

[ConcreteFactory1]-->[ProductA1]
[ConcreteFactory1]-->[ProductB1]
[ConcreteFactory2]-->[ProductA2]
[ConcreteFactory2]-->[ProductB2]
```


### Builder

![Builder](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/creational/builder/builder.png)

![Builder](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/creational/builder/builder_seq.png)

### Factory Method

![Factory Method](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/creational/factory/factory.png)

### Prototype

![Prototype](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/creational/prototype/prototype.png)

### Singleton

![Singleton](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/creational/singleton/singleton.png)

## Structural Patterns
### Adapter

![Adapter MultiInheritance](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/structural/adapter/adapter.png)

### Bridge

![Bridge](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/structural/bridge/bridge.png)

### Composite

![Composite](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/structural/composite/composite.png)

### Decorator

![Decorator](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/structural/decorator/decorator.png)

### Façade


![Façade](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/structural/facade/facade.png)


```

[<package>Subsystem Classes |
	
    [Class1]
    [Class2]
    [Class3]
    [Class4]
    [Class5]
    [Class6]
    [Class7]
]

[<abstract>Facade
	|
	| 
]

[Class2]-->[Class1]
[Facade]->[Class2]
[Facade]->[Class3]
[Facade]->[Class4]
[Facade]->[Class6]
[Facade]->[Class7]

[Class5]<:-[Class6]
[Class5]<:-[Class7]
[Class1]<:-[Class3]

```


### Flyweight

![Flyweight](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/structural/flyweight/flyweight.png)

### Proxy 

![Proxy](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/structural/proxy/proxy.png)

## Behavioral Patterns
### Chain of Responsibility

![Chain of Responsibility](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/chain_of_responsibility/chain_of_responsibility.png)

### Command

![Command](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/command/command.png)

![Command Sequence](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/command/command_seq.png)

### Interpreter

![Interpreter](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/interpreter/interpreter.png)

### Iterator

![Iterator](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/iterator/iterator.png)

### Mediator

![Mediator](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/mediator/mediator.png)

### Memento

![Memento](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/memento/memento.png)

![Memento](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/memento/memento_seq.png)

### Observer

![Observer](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/observer/observer.png)

![Observer Sequence](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/observer/observer_seq.png)

### State

![State](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/state/state.png)

### Strategy

![Strategy](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/strategy/strategy.png)

### Template Method

![Template Method](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/template_method/template_method.png)

### Visitor

![Visitor](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/visitor/visitor.png)

![Visitor](https://raw.githubusercontent.com/oro8oro/nomnoml-design-patterns/master/generated/Model/loretek/design_patterns/behavioral/visitor/visitor_seq.png)