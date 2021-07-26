# Exception

**Exception** is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.

**call stack** ordered list of methods that had been called to get to the method where the error occurred.

> **mine** --- _Method call_ ---> **Method with an expeption handler** --- _Method call_ --->**Method without an expeption handler** --- _Method call_ ---> **Method where error occurred**.

**exception handler** a block of code that can handle the exception. If the runtime system exhaustively searches all the methods on the call stack without finding an appropriate exception handler, the runtime system terminates.

### **The Catch or Specify Requirement**

Code that might throw certain exceptions must be enclosed by either of:

- **_A try statement_** that catches the exception. The try must provide a handler for the exceptions.

- **_A method_** that specifies that it can throw the exception. The method must provide a throws clause that lists the exception.

> Note: **NOT** all exceptions are subject to the Catch or Specify Requirement.

### **The Three Kinds of Exceptions**

1. **[Checked exception]** exceptional conditions that a well-written application should anticipate and recover from.

2. **[Error]** exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from.

3. **[Runtime exception]** exceptional conditions that are internal to the application, and that the application usually cannot anticipate or recover from. These usually indicate programming bugs.

<br>

# Primitives versus Objects

Java has a two-fold type system consisting of `primitives` such as int, boolean and `reference` types such as Integer, Boolean. Every primitive type corresponds to a reference type.

**WRAPPER CLASSES** are immutable, so that their state can't change once the object is constructed and are final, we can't inherit from them.

**AUTOBOXING** ---> `Integer j = 5;` The process of converting a primitive type to a reference one.

**AUTOBOXING** ---> `int i = new Integer(5);` The process of converting a reference type to a primitive one.

### **Pros and Cons**

The decision what object is to be used is based on:

### 1. Single Item Memory Footprint:

Variables of primitive types live in the stack and hence are accessed fast.

The reference types are objects, they live on the heap and are relatively slow to access. They have a certain overhead concerning their primitive counterparts.

### 2. Memory Footprint for Arrays:

single-element arrays of primitive types are almost always more expensive than the corresponding reference type.

> arrays of the primitive types long and double consume more memory than their wrapper classes Long and Double.

### 3. Performance:

it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.

### **Default Values**

the primitive types may acquire values only from their domains, while the reference types might acquire a value (null) that in some sense doesn't belong to their domains.

### **Usage**

When our application needs collections with a big number of elements, we should consider using arrays with as more “economical” type as possible.

<br>

# Scanning

Useful for breaking down formatted input into tokens and translating individual tokens according to their data type. By default, a scanner uses white space to separate tokens.

> **NOTE:** Even though a scanner is not a stream, you need to close it to indicate that you're done with its underlying stream.

We have to mention the locale, because thousands separators and decimal symbols are locale specific. That's not something you usually have to worry about, because your input data usually comes from sources that use the same locale as you do.

<hr>
<br>

**Sources**

- What Is an Exception? / Java Documentation.

- Scanning / Java Documentation.

- Java Primitives versus Objects / Baeldung.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
