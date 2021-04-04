# Comparison operations

## EVALUATING CONDITIONS:
You can evaluate a situation by By uesing operator in this table:

|Operator|Name|Description|
|--|--|--|
|==|Equal to| if the operands are equal|
|===|Strict equal to| if the operands are equal and of the same type|
|!=|Not equal to| if the operands are not equal|
|!==|Strict not equal to|if the operands are equal but of different type or not equal at all|
|>|Greater than|if the left operand is greater than the right operand|
|<|Less than|if the left operand is less than the right operand|
|>=|Greater than or Equal to| if the left operand is greater than or equal to the right operand|
|<=|Less than or Equal to| if the left operand is less than or equal to the right operand|

> Note: The result will be a **boolean** : True or false.

## LOGICAL OPERATORS

|Operator|Name|Description|
|--|--|--|
|&&|AND|true if both the operands/boolean values are true, else evaluates to false|
| \|\| |OR|true if either of the operands/boolean values is true. evaluates to false if both are false|
|!|NOT|true if the operand is false and vice-versa|

> Note: You can also use logical operators with numbers. In JavaScript, 0 is false and all non-zero values are true.

# LOOPS
The **loop** check a condition, if it returns **true**, a code block will run, then the condition will be checked again and if it still returns **true**, the code block will run again. It repeats until the condition returns **false**.

### **Common types of loops**:

* **FOR** : if you want to run the code specific number of times.

```
for (statement 1; statement 2; statement 3) {
  code block to be executed
}
```

* **WHILE** : loops through a block of code while a specified condition is true.

```
while (condition) {
 code block to be executed
}
```

* **do/while** : loops through a block of code once, and then repeats the loop while a specified condition is true.

```
do {
  code block to be executed
}
while (condition);
```

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)