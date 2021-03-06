
# Object-oriented programming(OOP)

**Object-oriented programming (OOP)** is a programming language model organized around object rather  than "actions" and data rather than logic. Historically, a program has been viewed as a logical procedure that takes input data, processes it, and produces output data. It manipulates objects rather than logic in program. Objects can be compared with real world examples. Examples of objects range from human beings (described by name, address, and so forth) to buildings and floors (whose properties can be described and managed) down to the little widgets on a computer desktop (such as buttons and scroll bars).One of the principal advantages of object-oriented programming over procedural programming is that they enable programmers to create modules that do not need to be changed when a new type of object is added. It is difficult to handle large projects in procedural or logical programming but object-oriented programming can handle large project easily. So these days most programming languages( i.e. php, python, ruby, JavaScript etc )  are multi-paradigm programming languages that support object-oriented programming to a greater or lesser degree, typically in combination with imperative, procedural programming.

### Advantages of OOP

* Since a class defines only the data it needs to be concerned with, when an object is run, the code will not be able to accidentally access other program data. This characteristic of data hiding provides greater system security and avoids unintended data corruption.
* It is closer to the real world phenomenon, so it is easier to map the real world problems into a  solution in oop.
* Oop based system are more scalable and relaiable.
* The definition of a class is reusable not only by the program for which it is initially created but also by other object-oriented programs (and, for this reason, can be more easily distributed for use in networks).
* The concept of data classes allows a programmer to create any new data type that is not already defined in the language itself.
* The concept of a data class makes it possible to define subclasses of data objects that share some or all of the main class characteristics. Called inheritance, this property of OOP forces a more thorough data analysis, reduces development time, and ensures more accurate coding.
* OOP provides a good framework for code libraries where supplied software components can be easily adapted and modified by the programmer.

## What Is a Class?

A class is a blueprint or prototype from which objects are created. A class models the state and behavior of a real-world object. It intentionally focuses on the basics, showing how even a simple class can cleanly model state and behavior. Procedures or behavior in object-oriented programming are known as methods; variables or state are also known as fields, members, attributes, or properties. This leads to the following terms:

* Class variables or attributes - belong to the class as a whole; there is only one copy of each one
* Instance variables or attributes - data that belongs to individual objects; every object has its own copy of each one.
* Member variables or attributes - refers to both the class and instance variables that are defined by a particular class.
* Class methods - belong to the class as a whole and have access only to class variables and inputs from the procedure call
* Instance methods - belong to individual objects, and have access to instance variables for the specific object they are called on, inputs, and class variables

## What Is an Object?

An object is a software bundle of related state(variables in some programming languages) and behavior(functions or methods in some programming languages).Objects are created by calling a special type of method in the class known as a constructor(default constructor are automatically generated by the compiler in the absence of any programmer-defined constructors). A program may create many instances of the same class as it runs, which operate independently. When a program is executed, objects interact with each other by sending messages(the process of selecting which implementation of a  method or function to call at run time). Different objects can also interact with each other without knowing the details of their data or code. Methods operate on an object's internal state and serve as the primary mechanism for object-to-object communication. Hiding internal state and requiring all interaction to be performed through an object's methods is known as data encapsulation — a fundamental principle of object-oriented programming. Encapsulation prevents external code from being concerned with the internal workings of an object. This facilitates code refactoring, for example allowing the author of the class to change how objects of that class represent their data internally without changing any external code (as long as "public" method calls work the same way). it isolates a particular code and data from all other codes and data. A well-defined interface controls the access to that particular code and data. The act of placing data and the operations that perform on that data in the same class. The class then becomes the 'capsule' or container for the data and operations. It hides the implementation details. All data members or fields in class should be hidden but can be accessed via properties that is read-only or read-write and no interface members should be hidden.
Bundling code into individual software objects provides a number of benefits, including:

1. *Modularity:* The source code for an object can be written and maintained independently of the source code for other objects. Once created, an object can be easily passed around inside the system.
2. *Information-hiding:* By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.
3. *Code re-use:* If an object already exists (perhaps written by another software developer), you can use that object in your program. This allows specialists to implement/test/debug complex, task-specific objects, which you can then trust to run in your own code.
4. *Pluggable and debugging ease:* If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement. This is similar to fixing mechanical problems in the real world. If a bolt breaks, you replace it, not the entire machine.

## Modularity

Modularity is closely tied with encapsulation; think of modularity as a way of mapping encapsulated abstractions into real, physical modules. Modularity is a frequently used term in information technology and computer science. Modularity refers to the concept of making multiple modules first and then linking and combining them to form a complete system. Modularity enables re-usability and minimizes duplication.
Modularity is the degree to which a system’s components are made up of relatively independent components or parts which can be combined.

The C/C++ convention is to create two files for each class: a header file (.h suffix) for the class interface, and an implementation file (.c, .cp, .cpp, .C suffix) for the code of the class.
Booch gives two goals for defining modules. Make a module cohesive (shared data structures, similar classes) with an interface that allows for minimal inter-module coupling.
Other considerations: team work, security, documentation.
Important to remember that the decisions concerning modularity are more physical issues, whereas the encapsulation of abstractions are logical issues of design.
It is possible to "over modularize". This can increase documentation costs and make it hard to find information.

## What Is Inheritance?

Inheritance provides a powerful and natural mechanism for organizing and structuring software. It is the process by which one object acquires the properties of another object. This supports the hierarchical classification. Without the use of hierarchies, each object would need to define all its characteristics explicitly. However, by use of inheritance, an object needs only to define those qualities that make it unique within its class. It can inherit its general attributes from its parent. A new sub-class inherits all of the attributes of all of its ancestors. Subclasses can override the methods defined by super-classes.

Multiple inheritance is allowed in some languages, though this can make resolving overrides complicated. Some languages have special support for mixins, though in any language with multiple inheritance, a mixin is simply a class that does not represent an is-a-type-of relationship. Mixins are typically used to add the same methods to multiple classes. Mixins are sometimes described as being "included" rather than "inherited". Mixins encourage code reuse and can be used to avoid the inheritance ambiguity that multiple inheritance can cause. For example, class UnicodeConversionMixin might provide a method unicode-to-ascii() when included in class FileReader and class WebPageScraper, which don't share a common parent. Abstract classes cannot be instantiated into objects; they exist only for the purpose of inheritance into other "concrete" classes which can be instantiated. In PHP, the final keyword can be used to prevent a class from being subclassed.

### Advantages of inheritance

* Extensibility
* Re-usability
* abstraction
* eliminate redundant code

## What Is an Interface?

An interface is a contract between a class and the outside world. When a class implements an interface, it promises to provide the behavior published by that interface. An interface is a description of the actions that an object can do. For example when you flip a light switch, the light goes on, you don't care how, just that it does. In Object Oriented Programming, an Interface is a description of all functions that an object must have in order to be an "X". Again, as an example, anything that "ACTS LIKE" a light, should have a turn\_on() method and a turn\_off() method. The purpose of interfaces is to allow the computer to enforce these properties and to know that an object of TYPE T (whatever the interface is ) must have functions called X,Y,Z, etc.
An interface is a programming structure/syntax that allows the computer to enforce certain properties on an object (class). For example, say we have a car class and a scooter class and a truck class. Each of these three classes should have a start\_engine() action. How the "engine is started" for each vehicle is left to each particular class, but the fact that they must have a start\_engine action is the domain of the interface.
Interfaces fulfill two goals:

1. They allow the programmer to be more abstract when referencing objects (for example, var vehicle : Vehicle, can reference any car, truck, etc... anything that is a vehicle (and not care what type it is.) This occurs at "program time".
When the vehicle.start\_engine() function is invoked, the correct function associated with the real object is actually used. This occurs at "run time".
2. They require the programmer to create specific functions that are expected in an implementing class when it implements an Interface.

Again, this allows all objects in a "set" of like objects to be treated based on the "high level" type of the set, rather than on the specific type of the individual object.
Take a look at your television when it is off. Its interface are the buttons it has an and the various plugs and the screen. Its semantics and behavior are that it takes inputs (e.g., cable programming) and has outputs (display on the screen, sound, etc.). However, when you look at a TV that is not plugged in, you are projecting your expected semantics into an interface. For all you know, the TV could just explode when you plug it in. However, based on its "interface" you can assume that it won't make any coffee since it doesn't have a water intake.
In object oriented programming, an interface generally defines the set of methods (or messages) that an instance of a class that has that interface could respond to.
An interface is most certainly not a blueprint for a class. A blueprint, by one definition is a "detailed plan of action". An interface promises nothing about an action! The source of the confusion is that in most languages, if you have an interface type that defines a set of methods, the class that implements it "repeats" the same methods (but provides definition), so the interface looks like a skeleton or an outline of the class

## Access specifier in oop
The main purpose of using access specifiers is to provide security to the applications. The availability (scope) of the member objects of a class may be controlled using access specifiers. Access specifiers are a specific part of programming language syntax used to facilitate the encapsulation of components.
C++ uses the three modifiers called public, protected, and private. C# has the modifiers public, protected ,internal, private, and protected internal. Java has public, package, protected, and private. The access modifier package is the default and used, if any other access modifier keyword is missing. The meaning of these modifiers may differ from one language to another. A comparison of the keywords, ordered from the most restrictive to the most open, and their meaning in these three languages follows. Their visibility ranges from the same class to the package where the class is defined to a general access permission. Below, the maximal access is written into the table.

*PUBLIC:* As the name specifies, it can be accessed from anywhere. If a member of a class is defined as public then it can be accessed anywhere in the class as well as outside the class. This means that objects can access and modify public fields, properties, methods.

*PRIVATE:* As the name suggests, it can't be accessed outside the class. Its the private property of the class and can be accessed only by the members of the class.

*FRIEND/INTERNAL:* Friend & Internal mean the same. Friend is used in VB.NET. Internal is used in C#. Friends can be accessed by all classes within an assembly but not from outside the assembly.

*PROTECTED:* Protected variables can be used within the class as well as the classes that inherites this class.

*PROTECTED FRIEND/PROTECTED INTERNAL:* The Protected Friend can be accessed by Members of the Assembly or the inheriting class, and of-course, within the class itself.

*DEFAULT:* A Default property is a single property of a class that can be set as the default. This allows developers that use your class to work more easily with your default property because they do not need to make a direct reference to the property. Default properties cannot be initialized as Shared/Static or Private and all must be accepted at least on argument or parameter. Default properties do not promote good code readability, so use this option sparingly.

## Namespace

Often, one assembly has only one name-space and is used by one program. But it can span over several name-spaces. Also, one name-space can spread over several assemblies. In large designs, an assembly may consist of multiple files that are held together by a manifest (i.e. a table of contents).
In C#, an assembly is the smallest deployment unit used.
a name-space is a set of symbols that are used to organize objects of various kinds, so that these objects may be referred to by name

## What Is a Package?

A package is a name-space for organizing classes and interfaces in a logical manner. Placing your code into packages makes large software projects easier to manage. A package, also known as a name-space, contains its own variables and subroutines. It's a way of segregating different parts of your program. You create the package and put your code into it.

## What Is a Polymorphism?

In programming languages and type theory, polymorphism ( polys means "many, much" and morphē means "form, shape") is the provision of a single interface to entities of different types. It is a feature that allows one interface to be used for a general class of actions. The specific action is determined by the exact nature of the situation. In general, polymorphism means "one interface, multiple methods", This means that it is possible to design a generic interface to a group of related activities. This helps reduce complexity by allowing the same interface to be used to specify a general class of action. It is the compiler's job to select the specific action (that is, method) as it applies to each situation.

In the programming world, polymorphism is used to make applications more modular and extensible. Instead of messy conditional statements describing different courses of action, you create interchangeable objects that you select based on your needs. That is the basic goal of polymorphism. The ability of different objects to respond, each in its own way, to identical messages is called polymorphism.

Method names are part of an object’s interface. When a message is sent requesting that an object do something, the message names the method the object should perform. Because different objects can have methods with the same name, the meaning of a message must be understood relative to the particular object that receives the message. The same message sent to two different objects can invoke two distinct methods.

The main benefit of polymorphism is that it simplifies the programming interface. It permits conventions to be established that can be reused in class after class. Instead of inventing a new name for each new function you add to a program, the same names can be reused. The programming interface can be described as a set of abstract behaviors, quite apart from the classes that implement them.

It is the ability of assigning different meaning to entities such as variable, methods or objects so that these can be made to exhibit more than one form. In class we have functions and these functions when accessed from objects can come from base class or derived class and user don't always stick to it override. Abstract operation is possible due to polymorphism. It is used to pass more specific object to a method and to declare a more generic field which is initialized and specialized. It ensures the appropriate method of the sub class that is called. Exact method to be called is determined at runtime.

## What Is Abstraction?

Abstraction (from the Latin abs, meaning away from and trahere, meaning to draw) is the process of taking away or removing characteristics from something in order to reduce it to a set of essential characteristics. In object-oriented programming, abstraction is one of three central principles (along with encapsulation and inheritance). Through the process of abstraction, a programmer hides all but the relevant data about an object in order to reduce complexity and increase efficiency. In the same way that abstraction sometimes works in art, the object that remains is a representation of the original, with unwanted detail omitted. The resulting object itself can be referred to as an abstraction, meaning a named entity made up of selected attributes and behavior specific to a particular usage of the originating entity. Abstraction represents complex reality in terms of simplified model. Abstraction is related to both encapsulation and data hiding. The programmer works with an idealized interface (usually well defined) and can add additional levels of functionality that would otherwise be too complex to handle. For example, a programmer writing code that involves numerical operations may not be interested in the way numbers are represented in the underlying hardware ( e.g. whether they're 16 bit or 32 bit integers), and where those details have been suppressed it can be said that they were abstracted away, leaving simply numbers with which the programmer can work. The advantages of abstraction are that we can have an eye to future reuse and managing complexity. looking at object, we see things that have meaning to us we abstract their property and keep only what we need e.g. students get "name" not "color of eye".

## Association, Aggregation, and Composition
*Association* is a 'has-a' relationship between two classes where there is no particular ownership in place. It is just the connectivity between the two classes. When you define a variable of one class in another class, you enable first to associate functions and properties of the second class. Then again  both Aggregation and Composition are types of Association.

*Aggregation* is a weak type of Association with partial ownership. For an Aggregation relationship, we use the term 'uses' to imply a weak 'has-a' relationship. This is weak compared to Composition. Then again, weak meaning the linked components of the aggregator may survive the aggregations life-cycle without the existence of their parent objects. For example, a school department *uses* teachers. Any teacher may belong to more than one department. And so, if a department ceases to exist, the teacher will still exist.

On the other hand, *Composition* is a strong type of Association with full ownership. This is strong compared to the weak Aggregation. For a Composition relationship, we use the term 'owns' to imply a strong 'has-a' relationship. For example, a department 'owns' courses, which means that the any course's life-cycle depends on the department's life-cycle. Hence, if a department ceases to exist, the underlying courses will cease to exist as well.

Whenever there is no ownership in place, we regard such a relationship as just an Association and we simply use the 'has-a' term, or sometimes the verb describing the relationship. For example, a teacher 'has-a' or 'teaches' a student. There is no ownership between the teacher and the student, and each has their own life-cycle.

## Typing
According to the theories of abstract data type, a type is a characterization of a set of elements. In OOP, a class is visualized as a type having properties distinct from any other types. Typing is the enforcement of the notion that an object is an instance of a single class or type. It also enforces that objects of different types may not be generally interchanged; and can be interchanged only in a very restricted manner if absolutely required to do so.
The two types of typing are:

* Strong Typing : Here, the operation on an object is checked at the time of compilation, as in the programming language Eiffel.
* Weak Typing : Here, messages may be sent to any class. The operation is checked only at the time of execution, as in the programming language Smalltalk.

## Concurrency

Concurrency in operating systems allows performing multiple tasks or processes simultaneously. When a single process exists in a system, it is said that there is a single thread of control. However, most systems have multiple threads, some active, some waiting for CPU, some suspended, and some terminated. Systems with multiple CPUs inherently permit concurrent threads of control; but systems running on a single CPU use appropriate algorithms to give equitable CPU time to the threads so as to enable concurrency.
In an object-oriented environment, there are active and inactive objects. The active objects have independent threads of control that can execute concurrently with threads of other objects. The active objects synchronize with one another as well as with purely sequential objects.

## Persistence

An object occupies a memory space and exists for a particular period of time. In traditional programming, the lifespan of an object was typically the lifespan of the execution of the program that created it. In files or databases, the object lifespan is longer than the duration of the process creating the object. This property by which an object continues to exist even after its creator ceases to exist is known as persistence.
