# Object Oriented Design

### SOLID:The First 5 Principles of Object Oriented Design

SOLID stands for:

- S - Single-responsiblity Principle.
- O - Open-closed Principle.
- L - Liskov Substitution Principle.
- I - Interface Segregation Principle.
- D - Dependency Inversion Principle.

### [Single-Responsibility Principle]

A class should have only one job.

For example if have a class with the name of `Shape`, that inherit Circle Class and Square Class.

the Circle has a radius but the Square has length. if I need to calculate the area from shape, i should determinate type of the Shape.

**Real-life example**: Nobody wants to live in a resort, it's nice and good for a particular vacation but it's impractical for everyday life..

### [Open-Closed Principle]

which mean that the Objects should be open for extension but closed for modification.

**class should be extendable without modifying the class itself.**

Back to `Shape` class its better to remove the area method out of the super class method and attach it to each shape’s class.

```java
// Square
    public int area() {
        return area(thi.length, 2);
    }
// Circle
    public int area() {
        return pi() * area(thi.length, 2);
    }
```

> To know that the object passed into the area() is actually a shape or if the shape has a method named area, we can use **interface** which is an integral part of SOLID.

```java
public interface ShapeInterface {
    public double area();
}
```

**Real-life example**: you can extend the phone's capabilities to allow you to manage more applications via the app store.

### [Liskov Substitution Principle]

Means that every subclass or derived class should be substitutable for their base or parent class.

**Real-life example**: if you're anything, you'd only put things in there that were edible because you would want to eat the stew without picking through each bite, asking yourself repeatedly, "is this edible?"

### [Interface Segregation Principle]

A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.

if I want to support the new three-dimensional shapes of, I will need to calculate volume.

for example :

```java
public interface ShapeInterface {
    public double area();
    public double volume(); // X shapes like Circle doesn't have volume you could create another interface to solve this
}
```

**Real-life example**: In the restaurant menu. there is all of the normal menu mainstays, and then something that's just called "soup of the day. because the soup changes a lot and there's no sense reprinting the menus every day.

### [Dependency Inversion Principle]

Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.

**Real-life example**: when you pay with a credit card. the clerk doesn't examine your card and gets out the "visa machine" after seeing that your card is a visa. he just takes your card, whatever it is, and swipes it.

<hr>
<br>

**Sources**

- SOLID: The First 5 Principles of Object Oriented Design / Samuel Oloruntoba.

- The SOLID Principles in Real Life / Erik Dietrich.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
