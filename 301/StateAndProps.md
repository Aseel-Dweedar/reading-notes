# Component Lifecycle Events

Lifecycle Events is The methods that you are able to use on Component. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.


![Component Lifecycle](../img301/compLifestyle.png)

## 1. **Mounting**
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase.

## 2. **Updating**
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.

## 3. **Unmounting**
The final phase of the lifecycle if called when a component is being removed from the DOM.

**constructor()**
it is mounted. If the component is a **subclass** you should call **super(props)**, or the props will be **undefined**.

>**NOTE**: Avoid using this.setState() in the constructor because it can lead to side effects, and it is unnecessary.

* **getDerivedStateFromProps()**
This method exists for rare cases where the state relies on changes in props over time.

* **render()**
the only required method in a class component. It will examine this.props and this.state when called.

> **NOTE**: The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. and should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false.

* **componentDidMount()**
This method is invoked immediately after a component is mounted. **setState()** can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.

* **shouldComponentUpdate()**
The default behavior in react is to rerender after every state change. 

* **getSnapshotBeforeUpdate()** 
allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.

* **componentDidUpdate()**
This method is useful for performing network requests after a change has occurred.

* **componentWillUnmount()**
This method allows you to clean up the DOM and netwrok requests/ subscriptions.

## After reading this you should be able to answer these questions :

what happens first, the `render` or the `componentDidMount`?

`render`

What is the very first thing to happen in the lifecycle of React?

`constructor`

Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`.

constructor --> React Updates --> render --> componentDidMount --> componentWillUnmount.


## React State Vs Props
 
![React State Vs Props](../img301/video.PNG)

**What types of things can you pass in the props?**

when you create a component inside a react and you want to render it you're going to pass it the props that you want to give to it.

**What is the big difference between props and state?**

props is handel outside the Component and must be updated outside it.
state is handel inside the Component and must be updated inside it.

**When do we re-render our application?**

when you change the state inside of your application it's going to re-render that section.

**What are some examples of things that we could store in state?**

we need state to store that thing that we're going to be updating like counts in the counter. and inside the form.

<hr>
<br>

**Article sources**

* React: Component Lifecycle Events / Joshua Blankenship.

* React State Vs Props / Web Dev Simplified-Youtube.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)