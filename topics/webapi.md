# WebAPI

### Part of the .NET Framework
Because the .NET framework is **SOOO** massive, Microsoft has separated it into several sections. One of the most commonly used sections for web developers is [MVC](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions-1/overview/asp-net-mvc-overview). This section of the framework is *very creatively* :roll_eyes: named after the more general architectural pattern known as [Model-View-Controller](https://www.wikiwand.com/en/Model%E2%80%93view%E2%80%93controller) (MVC).

Inside the MVC section of .NET is a section called **_WebAPI_**. This is the section that we'll be working with for right now. The View of a WebAPI is considered to be the JSON that is returned to the client.

## Controllers
Controllers, in a general sense, are classes that have the specific purpose of processing an incoming request, calling any additional logic, and returning a response to that request.

You can think of Controllers as an "orchestration layer" that will be responsible for accessing code in other parts of your application and handling the result of that code.

## Models
Models are a representation of your data in C#. Functionally, they are just classes with nothing but properties in them.

For instance, if your application was tracking doctors in a hospital, then one of your models might look something like this.
```cs
public class Doctor
{
    public int Id { get; set; }
    public string Name { get; set; }
    public string Specialty { get; set; }
    public string Gender { get; set; }
    public int Rating { get; set; }
    public string Department { get; set; }
}
```

## Attributes
Attributes are a feature can be used anywhere in C#, but we'll be discussing them in the [context of WebAPI](https://docs.microsoft.com/en-us/aspnet/web-api/overview/web-api-routing-and-actions/create-a-rest-api-with-attribute-routing#add-route-attributes). They are denoted by the square brackets directly above the method signature of a controller.
```cs
[HttpGet] //<-- attribute
public IEnumerable<User> GetUsers()
{
    // get all the users
}
```
Attributes can also be used at the class level.
```cs
[Route("api/[controller]")]
[ApiController]
public class UsersController : ControllerBase
{
    // get User methods
}
```
Attributes can also be used directly inside a parameter list
```cs
[HttpPost]
public IActionResult CreateUser([FromBody] User newUser)
{
    // save a new user
}
```

## What exactly is ActionResult?
(Coming Soon)
