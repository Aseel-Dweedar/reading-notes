## Forms - React

**1. What is a ‘Controlled Component’?**

An input form element whose value is controlled by React by controlling whats happens in that form on subsequent user input.

**2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

kept in the state property of components, and only updated with `setState()`. because you only need to update it in one place.

**3. How do we target what the user is entering if we have an event handler on an input field?**

By naming attribute to each element and let the handler function choose what to do based on the value of `event.target.name`.

<hr>
<br>

## The Conditional (Ternary) Operator Explained

**1. Why would we use a ternary operator?**

Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.

**2. Rewrite the following statement using a ternary statement:**

```JS
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

**_Selution:_**

```JS
x===y ? console.log(true) : console.log(false)
```

<hr>
<br>

**Sources**

- Forms / reactjs.org.
- JavaScript — The Conditional (Ternary) Operator Explained / Brandon Morelli .

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
