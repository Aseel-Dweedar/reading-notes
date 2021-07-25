# A Guide to Java Loops

looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to **_false_**.

types of loops in Java:

**1. For Loop** :

allows us to repeat certain operations by incrementing and evaluating a loop counter.

```java
for (int i = 0; i < 10; i++) {
    System.out.println("Hello world!");
}
```

**2. While Loop** :

It repeats a statement or a block of statements while its controlling Boolean-expression is true.

```java
int counter = 0.4;
int total = Math.random();
while (counter != total) {
    total = Math.random();
    System.out.println("Hello world!");
}
```

**3. Do-While Loop** :

The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.

```java
int counter = Math.random();
do
{
   System.out.println("Hello world!");
}
while (counter < 0.5);
```

# Packages and Import

A package name is the same as the directory (folder) name which contains the .java files. You declare packages when you define your Java program, and you name the packages you want to use from other libraries in an import statement.

### **[Package declaration]**

you can have import statements, which allow you to specify classes from other packages that can be referenced without qualifying them with their package.

It's possible to omit the package declaration. For small programs it's common to omit it, in which case Java creates what it calls a **_default package_**.

> Note : It's recommends that you do not use default packages.

<br>

### **[Package declaration syntax]**

<br>

```java
/* Package statement (optional). */
Package package_Name;

/* Imports (optional). */
import java.util.Scanner;

/* Class or interface definitions. */
public class Scan {
    . . .
}
```

### **[Imports: three options]**

The wildcard character (\*) is used to specify that all classes with that package are available to your program. This is the most common programming style.

- Make all classes visible altho only one is used.
- Make a single class visible.
- fully qualified class name without an import.

<br>

> **Note** : If you forgot to write import statements, or don't remember which package a class is in, right click on the source file and choose Fix Imports. It will add all necessary import statements.

<hr>
<br>

**Sources**

- Packages and Import / Java Notes.

- A Guide to Java Loops / Baeldung.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
