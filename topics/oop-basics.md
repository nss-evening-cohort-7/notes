# Object Oriented Programming (OOP) Basics

### Classes
[Classes](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/03_CLASSES.md) are the blueprints for your application. All classes _**must**_ be instantiated with the `new` keyword before any of their properties or methods can be accessed or used, unless they use the `static` keyword.

If you've used classes in JavaScript, then C# is semantically similar; even if JavaScript's implementation is syntactic sugar. You always need to create an instance of a class prior to using it.

> [C# accessibility levels](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/accessibility-levels) are a popular, trivia style, question in interviews.

### Properties and Fields
[Properties](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/properties) & [Fields](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/fields) are provided as a way to store the state of your class. Idiomatic C# states that fields should be prefixed with an underscore (`_myPrivateField`) and properties are named using Camel Caps (`MyPublicProperty { get; set; }`).

There is a special version of Properties called _**Auto Properties**_ that include the default getter and setter for the property.
```cs
public string HomeAddress { get; set; }
```
You can also customize the accessibility of the getter or setter.
```cs
public SocialSecurityNumber { get; private set; }
```

Fields and Properties can be functionally equivalent, but idiomatically speaking, Fields are intended for the internal state of the class and Properties are used to expose values to other areas of the application.

### Methods
You should already be familiar with [methods](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/04_METHODS.md). They are simply functions attached to an object (or instantiated Class) that perform an action.

> It may be helpful to familiarize yourself with what makes up a [method signature](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/methods).

> [Constructor methods](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/concepts/csharp-language/constructor-methods.md) are used for designing the initial state of your class

### Namespaces
[Namespacing](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/05_NAMESPACING.md) is just a roadmap for the compiler to follow through your code. If you put something in a different namespace, then the compiler in Visual Studio (msbuild) won't be able to find it until you include that new namespace with `using`.
> A `using` statement is semantically equivalent to `require` or `import` in JavaScript.

##### Exercises

- Your favorite things
  - Create at least four classes, each representing one of your favorite things.
  - Give each of these things two or more properties (attributes).
  - Give each of these things two or more methods (behavior).
  - Create at least one instance in your `Main` method of each of these classes.
  - Loop over each of your instantiated favorite things and print the attributes and behaviors to the console.

- Construct some Lego Minifigure Classes
	###### Properties

	Hair/Hat, Head, Torso, Legs, Accessories, etc.

	###### Methods

	If you were working at [Tt Games](http://www.ttgames.com/), your minifigure classes might have actions associated with them in the form of jump, double jump, attack, special attack, look & move methods.
	There might even be certain conditions that must be met to construct (or unlock) a new character or other kind of object.

- Bangazon
	- [Corporate Class](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/exercises/05_CLASSES.md)

- [Jungle Overloading](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/exercises/bangazon/BANGAZON_03.md)

- [Syntactic Sugar in C# 6](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/exercises/06_%20EXPRESSION_FN_MEMBERS.md)
