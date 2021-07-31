# Inheritance And Interfaces

### **[Object]**

consist of state and related behavior. An object stores its state in fields, and exposes its behavior through methods.
Methods operate on an object's internal state and serve as the primary mechanism for object-to-object communication.

Bundling code into individual software objects provides a number of benefits, including:

- Modularity.
- Information-hiding.
- Code re-use.
- Pluggability and debugging ease.

### **[Class]**

A class is a user defined blueprint or prototype from which objects are created. It represents the set of properties or methods that are common to all objects of one type.

### **_What Is Inheritance?_**

Object-oriented programming allows classes to inherit commonly used state and behavior from other classes.

**When you want to create a new class and there is already a class that includes some of the code that you want, you can derive your new class from the existing class. In doing this, you can reuse the fields and methods of the existing class without having to write (and debug!) them yourself.**

The syntax for creating a subclass: the beginning of your class declaration, use the extends keyword, followed by the name of the class to inherit from:

```java
class Cats extends Animals {
    // new fields and methods defining
    // a cat would go here
}
```

**Private Members in a Superclass**

A subclass inherits all of the public and protected members of its parent, no matter what package the subclass is in. If the subclass is in the same package as its parent, it also inherits the package-private members of the parent.

> Note: You can make a logical test as to the type of a particular object using the instanceof operator. This can save you from a runtime error owing to an improper cast. For example:

```java
if (obj instanceof MountainBike) {
    MountainBike myBike = (MountainBike)obj;
}
```

**Multiple Inheritance of State**

One significant difference between classes and interfaces is that classes can have fields whereas interfaces cannot. In addition, you can instantiate a class to create an object, which you cannot do with interfaces.

`multiple inheritance of state`, which is the ability to inherit fields from multiple classes.

**Overriding and Hiding Methods**

- Instance Methods: (name, plus the number and the type of its parameters) and return type as an instance method in the superclass overrides the superclass's method.

- Static Methods: If a subclass defines a static method with the same signature as a static method in the superclass, then the method in the subclass hides the one in the superclass.

```java
public class Animal {
    public static void staticMethod() {
        System.out.println("static method in Animal");
    }
    public void instanceMethod() {
        System.out.println("instance method in Animal");
    }
}
```

**Accessing Superclass Members**

If your method overrides one of its superclass's methods, you can invoke the overridden method through the use of the keyword `super`.

### **_What Is an Interface?_**

In its most common form, an interface is a group of related methods with empty bodies.

**Implementing an Interface:**

To implement this interface, the name of your class would change, and you'd use the implements keyword in the class declaration:

```java
class Cats implements Animals {
    int age = 0;
    void changeAge(int newValue) {
         age = newValue;
    }
    void printStates() {
         System.out.println("age:" + age);
    }
}
```

> NOTE: whereas a class can extend only one other class, an interface can extend any number of interfaces

**Using an Interface as a Type**

When you define a new interface, you are defining a new reference data type. You can use interface names anywhere you can use any other data type name. If you define a reference variable whose type is an interface, any object you assign to it must be an instance of a class that implements the interface.

**Default Methods**

Default methods enable you to add new functionality to the interfaces of your libraries and ensure binary compatibility with code written for older versions of those interfaces.

**Extending Interfaces That Contain Default Methods**

To extend an interface that contains a default method:

- Do not mention the default method at all, which lets your extended interface inherit the default method.
- Redeclare the default method, which makes it abstract.
- Redefine the default method, which overrides it.

**Static Methods**

A static method is a method that is associated with the class in which it is defined rather than with any object. Every instance of the class shares its static methods.

### **[Package]**

A package is a namespace that organizes a set of related classes and interfaces. The Java platform provides an enormous class library suitable for use in your own applications. This library is known as the "Application Programming Interface", or "API" for short.

<br>

<hr>
<br>

**Sources**

- Object and Class / Java Documentation.

- Interfaces and Inheritance / Java Documentation.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
