# Interfaces

An [Interface](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/10_INTERFACES.md) functions as a [contract for a class](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/interfaces/) to implement properties and methods. Unlike abstract classes, they cannot have a defined implementation. They will only contain properties(not initialized) and method signatures.

One of the benefits of using an interface is that a single class can implement multiple interfaces.
```cs
public class Amphicar : IGroundVehicle, IAquaticVehicle
{
	// An amphibious automobile
}
```

##### Exercises

- [SOLID Vehicles](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/master/orientation/exercises/11_INTERFACES.md) :blue_car: :racing_car: :police_car: :tractor: :articulated_lorry: :car:
- Bangazon
	- [Architecture](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/formatting/orientation/exercises/bangazon/BANGAZON_01.md)
	- [Polymorphism](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/formatting/orientation/exercises/bangazon/BANGAZON_02.md)
	- [Interfaces](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/formatting/orientation/exercises/bangazon/BANGAZON_04.md)
	- [Employee Aggregation](https://github.com/nss-evening-cohort-7/bangazon-inc/blob/formatting/orientation/exercises/bangazon/BANGAZON_05.md)
