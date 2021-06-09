# Thinking in React

### **1. How would you break a mock into a component hierarchy?**

1. draw boxes around every component (and subcomponent) in the mock and give them all names.

2. Use the same techniques for deciding if you should create a new function or object.

### **2. What is the `single responsibility principle` and how does it apply to components?**

which mean that the component should ideally only do one thing.

### **3. What does it mean to build a ‘static’ version of your application?**

build a version that takes your data model and renders the UI but has no interactivity.

### **4. Once you have a static application, what do you need to add?**

We need to Identify The Minimal Representation Of UI State.

### **.5 What are the three questions you can ask to determine if something is state?**

1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

### **.6 How can you identify where state needs to live?**

Is it passed in from a parent via props? If so, it probably isn’t state.

1. Identify every component that renders something based on that state.
2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
3. Either the common owner or another component higher up in the hierarchy should own the state.
4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

<hr>
<br>

**Sources**

- Thinking in React / reactjs.org.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
