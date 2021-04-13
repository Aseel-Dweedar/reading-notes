# LISTS - HTML

![list](https://744025.smushcdn.com/1245953/wp-content/uploads/2020/02/HTML-LISTS.jpg?lossy=1&strip=1&webp=1)

## 1-Ordered Lists : 

use numbers, When we care about the order.

**Syntax:**

```
<ol>
    <li>First element</li> 
    <li>Second element</li>
    <li>Third element</li>
</ol>
```
the result is:
<ol>
    <li>First element</li> 
    <li>Second element</li>
    <li>Third element</li>
</ol>
<hr>

## 2-Unordered Lists :

use bullets, When we don't care about the order.

**Syntax:**

```
<ul>
    <li>element</li> 
    <li>element</li>
    <li>element</li>
</ul>
```
the result is:
<ul>
    <li>element</li> 
    <li>element</li>
    <li>element</li>
</ul>

<hr>

## 3-Definition Lists :
are used to define terminology.

**Syntax:**

```
<dl>
    <dt>HTML</dt> 
    <dd>Hypertext Markup Language</dd>
    <dt>CSS</dt> 
    <dd>Cascading Style Sheets</dd>   
</dl>
```
the result is:
<dl>
    <dt>HTML</dt> 
    <dd>Hypertext Markup Language</dd>
    <dt>CSS</dt> 
    <dd>Cascading Style Sheets</dd>   
</dl>

> Notice that the `<dt>` This is used to contain the term being defined. `<dd>` This is used to contain the definition.
<hr>

## **Nested Lists**
You can put a second list inside an `<li>` element to create a sublist or nested list.

**EX:**

```
<ol>
    <li>First element</li> 
    <li>First element</li>
        <ul>
            <li>element</li> 
            <li>element</li>
            <li>element</li>
        </ul>
    <li>First element</li>
</ol>
```
the result is:

<ol>
    <li>First element</li> 
    <li>First element</li>
        <ul>
            <li>element</li> 
            <li>element</li>
            <li>element</li>
        </ul>
    <li>First element</li>
</ol>

## Bullet Point Styles

The **`list-style-type`** property in **CSS** allows you to control the shape or style of a bullet point (also known as a marker). 

```
For example:

ol {
list-style-type: upper-roman;}

numbering will be like: (I, II, III, IV, V, etc.)
```
## Images for Bullets
`list-style-image: url("images.png");`

## Positioning the Marker
Lists are indented into the page by default and the `list-style-position` property indicates whether the marker should appear on the inside or the outside of the box containing the main points. 


<hr>
<br>

# BOXES - CSS
**how CSS treats each HTML element as if it lives in its own box?**

By default a box is sized just big enough to hold its contents.

- To set your own dimensions for a box : `width:  ; / height:  ;`
- To set a Limiting Width `min-width: ; / max-width: ;`
- To set a Limiting hight `min-hight: ; / max-hight: ;`

**Overflowing Content** 

The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:

**hidden** This property simply hides any extra content that does not fit in the box.

**scroll** This property adds a scrollbar to the box so that users can scroll to see the missing content.
```
firsh {
overflow: hidden;}
second {
overflow: scroll;}
```
### **Border, Margin & Padding**

**Border** The border separates the edge of one box from another.

**Margin** outside the edge of the border. 

**Padding** s the space between the border of a box and any content contained within it.

![space](https://res.cloudinary.com/practicaldev/image/fetch/s--Epou9WnH--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://cdn-images-1.medium.com/max/682/1%2ARZy75Vjf8bETwl73-4iZPQ.png)

property you can apply it on **Border** :
- border-width
- border-style
- border-color

### **Change Inline/Block** display
<br>

![display](https://lh3.googleusercontent.com/proxy/AjU1w7z3NJSFZLkNC83Pc7S_SNkOqFhX-X05I1to0-3SxoXVeUISYvHjvHfTQEGcyyLe2nhyXZD_8-GZu8MSltltuhn3YtxccPFXK32unRs3ff2BXoFvAQThvV7_YTu-bNW88Rw60p4vI1uqdA0U4ib-gJMr)

you can hide boxes from users by using visibility property, it can take two values:

**hidden** This hides the element. 

**visible** This shows the element

>Notice that It leaves a space where the element would have been.

also you can add a drop shadow around a box by using `box-shadow` property. and make create rounded corners on any box, using a property called `border-radius`.


<hr>
<br>

# ARRAY - JS

**An array is a special type of variable. It doesn't just store one value; it stores a list of values.**

CREATING AN ARRAY : 

create an array and give it a name e just like you would any other variable,The values are assigned to the
array inside a pair of square brackets, and each value is separated by a comma.

EX:
```
var number;
colors ['one', 1, ];
```
>Notice that The values in the array do not need to be the same data type.

**Values** in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).

<hr>
<br>

# SWITCH STATEMENTS  - JS

A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 
|IF ELSE|SWITCH|
|--|--|
|There is no need to provide an el se option|You have a default option that is run if none of the cases match|
|With a series of if statements, they are all checked even if a match has been found|If a match is found, that code is run; then the break statement stops the rest of the switch statement running|

<br>

**Using switch**

![switch](https://www.bookofnetwork.com/images/javascript-images/JS_switch-syntax_20Sep16_1827.png)

<br>


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


<hr>
<br>

**Article sources**

* HTML & CSS Design and Build Websites / Jon Ducket

* JavaScript and jQuery Interactive / Jon Ducket

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)