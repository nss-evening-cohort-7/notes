# Jan Sat. 6th - Thurs. 11th <sub><sub><sub>:snowflake: :snowflake: :snowflake:

## How can I talk about what I'm learning?

[.NET can mean a lot of things](https://www.microsoft.com/net/learn/what-is-dotnet). It is a complex ecosystem and you're only going to get experience with a part of it here in class.

[.NET Core & .NET Framework are different](https://docs.microsoft.com/en-us/dotnet/standard/choosing-core-framework-server). _.NET Framework_ requires a Windows (virtual) environment. _.NET Core_ is newer, different, and can run on multiple operating systems, but overlaps some _**core**_ features<sub>*ba dum tss</sub> as well.

All live coding exercises will be using _.NET Framework_ in _Visual Studio for Windows_. If you're adventurous and want to explore _.NET Core_ on Windows, Mac, or Linux, then I highly recommend installing [_Visual Studio Code_](https://code.visualstudio.com/download) and introducing yourself to [some of it's features](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/03_USING_VS_CODE.md). Make sure you add the [C# extension](https://code.visualstudio.com/Docs/languages/csharp) immediately after installation completes.

#### [NuGet](https://www.nuget.org/), newget not nugget

***

## _Serious coders learn the language_ :canada: :alien: :capricorn:

Let's go through [this exercise](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/02_FIRST_EXECUTABLE.md) to get an idea of some of the primary differences between C# and JavaScript, and learn a few extra commands that make our [command line interactive](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/13_CLI_IO.md).

> You can also optionally begin [Koans](https://github.com/NotMyself/DotNetCoreKoans) which are test driven way to understand the language syntax and available data structures. It's best to take your time and make sure you understand each section before progressing. Just making the test pass doesn't mean you learned the lesson. If you reach a section that we haven't covered, feel free to do some preliminary research until class covers that concept.

### Classes
[Classes](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/03_CLASSES.md) are the blueprints for your application. All classes _**must**_ be instantiated with the `new` keyword before any of their properties or methods can be accessed or used, unless they use the `static` keyword.

If you've used classes in JavaScript, then C# is semantically similar; even if JavaScript's implementation is syntactic sugar. You always need to create an instance of a class prior to using it.

> [C# accessibility levels](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/accessibility-levels) are a popular, trivia style, question in interviews.

### Methods
You should already be familiar with [methods](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/04_METHODS.md). They are simply functions attached to an object (or instantiated Class) that perform an action.

> It may be helpful to familiarize yourself with what makes up a [method signature](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/methods).

> [Constructor methods](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/concepts/csharp-language/constructor-methods.md) are used for designing the initial state of your class

### Namespaces
[Namespacing](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/05_NAMESPACING.md) is just a roadmap for the compiler to follow through your code. If you put something in a different namespace, then the compiler in Visual Studio (msbuild) won't be able to find it until you include that new namespace with `using`.
> A `using` statement is semantically equivalent to `require` or `import` in JavaScript.

***

#### Exercises

- A few of your favorite things (Custom Types with behavior)

- Construct some Lego Minifigure Classes
	###### Properties

	Hair/Hat, Head, Torso, Legs, Accessories, etc.

	###### Methods

	If you were working at [Tt Games](http://www.ttgames.com/), your minifigure classes might have actions associated with them in the form of jump, double jump, attack, special attack, look & move methods.
	There might even be certain conditions that must be met to construct (or unlock) a new character or other kind of object.

- [Corporate Class](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/exercises/05_CLASSES.md)

- [Employee Aggregation](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/formatting/orientation/exercises/bangazon/BANGAZON_05.md)

- [Jungle Overloading](https://github.com/nss-evening-cohort-06/bangazon-inc/blob/master/orientation/exercises/bangazon/BANGAZON_03.md)

***

#### Classmate Resources
- Ken
	- [C#: Learn C# in One Day and Learn It Well.](https://www.amazon.com/Beginners-Hands-Project-Coding-Project-ebook/dp/B016Z18MLG/ref=sr_1_fkmr0_1?ie=UTF8&qid=1515544935&sr=8-1-fkmr0&keywords=learn+C%23+in+one+day)
	- [C# Cheat Sheet](https://www.thecodingguys.net/resources/cs-cheat-sheet.pdf)
- Brooke![](http://www.tutorialsteacher.com/Content/images/csharp/csharp-class.png)

***

## _Professionals learn their tools_ :hammer_and_wrench: :crystal_ball: :speech_balloon:
#### Code Navigation
- [Projects & Solutions](https://docs.microsoft.com/en-us/visualstudio/ide/creating-solutions-and-projects)
- [Code Navigation Tools](https://docs.microsoft.com/en-us/visualstudio/ide/navigating-code)

#### [Debugger](https://docs.microsoft.com/en-us/visualstudio/debugger/debugger-feature-tour)
If you're not using the debugger already then **_START NOW_**. It is the single greatest tool a programmer can use. When you want to `console.log(something)`, now you will use a debugger instead. Even [in JavaScript](https://stackoverflow.com/a/66431). **Seriously, I never want to see another `console.log()` again.**
- Yellow arrow is the point of execution. The highlighted line has not been executed.
- Call Stack shows current code path at point of execution.
- Locals, Immediate Window, & Watch.
	> Also, hovering over variables and using the mouse, but why do that when you have [hotkeys](http://visualstudioshortcuts.com/2017/) and search (<kbd>Ctrl</kbd>+<kbd>Q</kbd>)?
- Step Over <kbd>F10</kbd>, Step Into <kbd>F11</kbd>, and Step Out <kbd>Shift</kbd>+<kbd>F11</kbd>
- Run to click
- Run to cursor (<kbd>Ctrl</kbd>+<kbd>F10</kbd>)

#### Intellisense
- Code completion
- Hover text/tooltips as documentation
- Red/Green squiggly underline is referring to the Error List.
- Light bulb - (<kbd>Ctrl</kbd>+<kbd>.</kbd>)

#### Refactor Rename (<kbd>Ctrl</kbd>+<kbd>R,R</kbd>)
- Preview Changes :point_up: , (<kbd>Alt</kbd>+<kbd>P</kbd>)
