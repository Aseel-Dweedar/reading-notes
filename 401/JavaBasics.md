# **JAVA BASICS**

![java](../img401/java.png)

## Language Basics

- **VARIABLES** : an object stores its state in fields. kinds of variables:

  1. Instance Variables (Non-Static Fields): objects store their individual states in "non-static fields".
  2. Class Variables (Static Fields): any field declared with the static modifier; this tells the compiler that there is exactly one copy of this variable in existence, regardless of how many times the class has been instantiated.
  3. Local Variables: There is no special keyword designating a variable as local; that determination comes entirely from the location in which the variable is declared — which is between the opening and closing braces of a method.
  4. Parameters: The important thing to remember is that parameters are always classified as "variables" not "fields".

- **Operators**:

| Operators            | Precedence                    |
| -------------------- | ----------------------------- |
| postfix              | expr++ expr--                 |
| unary                | ++expr --expr +expr -expr ~ ! |
| multiplicative       | \* / %                        |
| additive             | + -                           |
| shift                | << >> >>>                     |
| relational           | < > <= >= instanceof          |
| equality             | == !=                         |
| bitwise AND          | &                             |
| bitwise exclusive OR | ^                             |
| bitwise inclusive OR | \|                            |
| logical AND          | &&                            |
| logical OR           | \|\|                          |
| ternary              | ? :                           |
| assignment           | = += -= \*= /= %= &= ^=       |

- **Expressions, Statements, and Blocks**

  1. Expressions: a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.

```java
// example
int a = 1;
int b = 5;
int result = a + b;
System.out.println("The sumption of a and b : " + result);
```

2. Statements: A statement forms a complete unit of execution.

```java
// declaration statement
int a = 1;
// increment statement
a++;
// method invocation statement
System.out.println("Wow!");
// object creation statement
Student joe = new Student();
```

3. Blocks: A group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed.

```java
if (condition) { // begin block
     System.out.println("Wow!");
} // end block
```

- **Control Flow Statements**: The statements inside the source files are generally executed from top to bottom, in the order that they appear. Control flow statements, break up the flow of execution by employing decision making, looping, and branching, enabling program to conditionally execute particular blocks of code.

## Compiling

putting everything in 1's and 0's -_machine language_- would be very difficult. So we made higher-level languages to write code in.
When you compile code, the compiler takes the program and converts it into the program the computer can understand. compile means to make the code executable.
the compiler checks if the program is written correctly according to the rules of the programming language.

## Java’s API Documentation

You can find things in the API documentation in a number of different ways:

1. Using the index.
2. Using the list of classes.

To create the API documentation, the captains of Java ran a program called javadoc. The javadoc program took lines like these right out of the PrintStream.java file and used the lines to make the documentation that you see in your web browser.

<hr>
<br>

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
