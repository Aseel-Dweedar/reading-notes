# Call Stack

### **1. What is a ‘call’?**

Is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

### **2. How many ‘calls’ can happen at once?**

It is single-threaded. Meaning it can only do one thing at a time.

### **3. What does LIFO mean?**

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### **4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

```JS
function sum (a, b) {
    return a + b;
}
function avg(a, b) {
    return sum (a, b) / 2;
}
let average = avg(10, 20);
```

### **.5 What causes a Stack Overflow?**

when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accommodate before throwing a stack error.

<br>

# Error messages && Debugging

### **1. What is a ‘reference error’?**

when you try to use a variable that is not yet declared you get this type os errors.

### **2. What is a ‘syntax error’?**

when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

### **3. What is a ‘range error’?**

The RangeError object indicates an error when a value is not in the set or range of allowed values.

### **4. What is a ‘tyep error’?**

when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

### **5. What is a breakpoint?**

The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

### **6. What does the word ‘debugger’ do in your code?**

when running the code above you can see the “history” before reaching that breakpoint.

<hr>
<br>

**Sources**

- The JavaScript Call Stack - What It Is and Why It's Necessary / Charles Freeborn.

- JavaScript error messages && debugging / Diogo Spínola.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
