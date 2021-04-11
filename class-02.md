# TEXT IN HTML :

## - HEADINGS : 
You can show the appropriate structure for your page using heading tags. these tags display the contents at different sizes.
<br/>

`<h1> <h2> <h3> <h4> <h5> <h6>`

The contents of an `<h1>` element is the largest, and the contents of an `<h6>` element is the smallest.  

## - PARAGRAPHS :
Under heading and subheading you can add a paragraphs by using this syntax :

`<p> write your pharagraph here </p>`

### **Style you page :**

1. make characters appear bold by using `<b>` tag.
2. make characters appear italic by using `<i>` tag.
3. use `<sup>` to contain characters that should be superscript such as the suffixes of dates or mathematical concepts .

ex:  `the 10<sup>th</sup> of september`

Result : the 10<sup>th</sup> of september

4. Use `<sub>` element to contain characters that should be subscript.

ex:  `H<sup>2</sup>O`

Result : H<sup>2</sup>O

5. Add a line break inside the middle of a paragraph by using `<br>` tag.
6. add a
horizontal rule between sections
using the `<hr>` tag.

## - SEMANTIC MARKUP :

You add extra information to your page by using semantic markup, they are not intended to affect the
structure of your web pages.

|Tag|Usage|Example|
|--|--|--|
|`<strong>`|show the contents in bold|`<strong>`Important`</strong>`class <br> <strong>Important</strong> class|
|<em>|show the contents in italic|My name is `<em>`Aseel`</em>` <br> My name is <em>Aseel</em>|
||||


### **QUOTATIONS :**

There are two elements commonly used for marking up quotations:

* The `<blockquote>` element is
used for longer quotes that take
up an entire paragraph.
* The `<q>` element is used for shorter quotes that sit within a paragraph.

> **NOTE:** Both elements may use the cite attribute to indicate where the quote is from.

### **Citations & Definitions:**

* the `<cite>` element can be used to indicate where the citation is from.

* The `<dfn>` element is used to indicate the defining instance of a new term.

### **Author Details:***
The `<address>` element has quite a specific use: to contain contact details for the author of the page.

### **Changes to Content:**

* The `<ins>` element can be used to show content that has been inserted into a document, while the `<del>` element can show text that has been deleted from it.

* The `<s>` element indicates something that is no longer accurate or relevant (but that should not be deleted).

<hr>

# INTRODUCING CSS

## - What is CSS :
CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

## - How CSS works
CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a **selector** and a **declaration**.

1. **Selectors** indicate which element the rule applies to.

2. **declaration** indicate how the elements referred to in the selector should be styled. 
Declarations are split into two parts :
   * **Properties** indicate the aspects of the element you want to change. 
   * **Values** specify the settings you want to use for the chosen properties.

![css](https://camo.githubusercontent.com/342e7c99e5b391b292df078d8ff8e95510f6fd053cc8c1b8c3aeab11d83bc1ca/68747470733a2f2f636f64652e6d616b6572792e63682f6c6962726172792f68746d6c2d6373732f70617274332f6373732d72756c652e706e67)

## - Using External CSS:

`<link>`: can be used in an HTML document to tell the browser where to find the CSS file used to style the page.

**It should use three attributes:**

1. **href :** This specifies the path to the CSS file (which is often placed in a folder called css or styles).

2. **type:** This attribute specifies the type of document being linked to. The value should be text/css.

3. **rel:**  This specifies the relationship between the HTML page and the file it is linked to.

## - Using Internal CSS:
include CSS rules within an HTML page by placing them inside a `<style>` element, which usually sits inside the `<head>`.

<hr>

![js](https://i.morioh.com/2020/04/28/db5257cad529.jpg)

# Basic JavaScript Instructions 

1. **STATEMENTS**
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon. 

    ex : `X = 120`

> Notes : <br> STATEMENTS ARE INSTRUCTIONS AND EACH ONE STARTS ON A NEW LINE .
<br> STATEMENTS CAN BE ORGANIZED INTO CODE BLOCKS 

2. **COMMENTS**

    write comments to explain what your code does. 

* **MULTI-LINE COMMENTS** To write a comment that stretches over more than one line, you use a multi-line comment, starting with the /* characters and ending with the */ characters. 

    ex : `/* add your comment here */`

* **SINGLE-LINE COMMENTS** In a single-line comment, anything that follows the two forward slash characters // on that line will not be processed by the JavaScript interpreter.

3. **VARIABLE**

    temporarily store the bits of information it needs to do its job. It can store this data in variables. 

    ![var](https://miro.medium.com/max/734/1*1CjVCzyVXh7TTKptnP1KnA.png)

4. **DATA TYPES**

    * **NUMERIC** DATA TYPE The numeric data type handles numbers. 

    * **STRING** DATA TYPE The strings data type consists of letters and other characters. 

    * **BOOLEAN** DATA TYPE Boolean data types can have one of two values: true or false. 

    * **ARRAYS** An array is a special type of variable. It doesn't just store one value; it stores a list of values. 

>In addition to these data types, JavaScript also has others (objects, undefined, and null).

## -EXPRESSIONS & OPERATORS

**Expressions** rely on **operators** to calculate a single value from one or more values.

![EXPRESSIONS](https://media.geeksforgeeks.org/wp-content/uploads/20190801163131/What-is-an-Expression_-3.jpg)

**Note:**
When you place quotes around a number, it is a **string** (not a numeric data type), and you cannot perform addition operations on strings. 

## -Decisions and Loops

There are some places in script where decisions are made that determine which lines of code should be ran next:

![run](https://media.geeksforgeeks.org/wp-content/uploads/if-else.png)

## -EVALUATING CONDITIONS:
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


## -LOGICAL OPERATORS

|Operator|Name|Description|
|--|--|--|
|&&|AND|true if both the operands/boolean values are true, else evaluates to false|
| \|\| |OR|true if either of the operands/boolean values is true. evaluates to false if both are false|
|!|NOT|true if the operand is false and vice-versa|

> Note: You can also use logical operators with numbers. In JavaScript, 0 is false and all non-zero values are true.
 ## -IF ELSE STATEMENT

The if/else statement executes a block of code if a specified condition is true. If the condition is false, another block of code can be executed.



 ![if](https://cdn.programiz.com/sites/tutorial2program/files/js-if-else-statement.png)


<hr>
<br>

**Article sources**

* HTML & CSS Design and Build Websites / Jon Ducket

* JavaScript and jQuery Interactive / Jon Ducket


**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)