# Language Integrated Query (aka [LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/index))
If you like playing with data, you're going to enjoy [LINQ](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/07_LINQ.md)

###### The setup
```cs
public class Student
{
	public string Name { get; set; }
	public bool IsPayingAttention { get; set; }
}

// Just pretend like we constructed some students.

var students = new List<Student> { gib, gina, david, ken };
```

### Method Syntax vs. Query Syntax
There are two ways to use LINQ. They look very different, but accomplish the same goal.

The method syntax looks and acts just like any other method that you would call on any other class. It has a name, parameters, and a return value.

###### Method syntax
```cs
var studentsPayingAttention = students.Where(student => student.IsPayingAttention == true);
```

The query syntax mimics SQL syntax, which we'll be learning about in a couple weeks, but can be different so it's best not to make assumptions about their similarities.

###### Query syntax
```cs
var studentsPayingAttention =
	from student in students
	where student.IsPayingAttention == true
	select student;
```

These two examples above accomplish the exact same thing. As you're learning, it's worth doing everything twice. Use both types of syntax and you'll eventually learn which one you like better. Which one you prefer to use may depend on the situation and complexity of your task.

The return value of all LINQ operations is [IQueryable](https://docs.microsoft.com/en-us/dotnet/api/system.linq.iqueryable). Notice the "I" in the front of the word. That means it's an interface. There's a [rabbit hole here](https://www.google.com/search?q=code+to+interfaces+not+implementations) regarding coding to interfaces if you choose to follow it.

##### Exercises
- [LINQed List](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/exercises/07_LINQ_LIST.md)
- [Advanced LINQ](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/exercises/20_ADVANCED_LINQ.md)


Protip - [Regex](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/formatting/concepts/csharp-language/regular-expressions.md) can be used [inside your LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/how-to-combine-linq-queries-with-regular-expressions)
