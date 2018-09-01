## Inheritance :family_man_woman_girl_boy:

In Javascript, every array you ever created has methods like `.map()`, `.filter()`, & `.forEach()`, but you didn't write those methods so how are they part of every array? The answer is inheritance. Javascript has a kind of inheritance called prototypal inheritance ([check out Steve's keynote slide deck](https://stevebrownlee.keybase.pub/OLOO/assets/player/KeynoteDHTMLPlayer.html#0)). [Classical Inheritance](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/inheritance) :classical_building: in C# looks and acts different, but has a very similar effect to how it acts in Javascript.

If not, it might be a good idea to familiarize yourself with [JavaScript inheritance](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain).
These [first 4 articles](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics) look helpful and in depth.

### Other types of relationships
There are a [couple other ways](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/inheritance) that C# can define relationships between Classes. Remember that a good way to tell the difference between when to use these different types of relationships is to ask yourself if the relationship between the things can be described best as "Thing 1 _**is a**_ Thing 2" or "Thing 1 _**has a**_ Thing 2"

### Abstract classes
[Abstract classes](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/abstract) can only be inherited from and cannot be instantiated. They are meant to serve as a base class to a series of related things that may want to share functionality.

You can also add the `abstract` keyword to methods inside of an abstract class if you only want to define the method signature, but you don't want to define any functionality at that time.

##### Exercises

- Refactor your favorite things
	- Create 3 variations of each of your favorite things
		- Ex. If one of your favorite things is a Truck, then other variations would be a Car, SUV, etc.
	- Inevitably, you'll have some shared functionality and properties between these different things. Create a base class that these variations can inherit from in order to share the functionality and properties between them.
