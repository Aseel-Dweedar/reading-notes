# RESTful web API design

### **1. What does REST stand for?**

Representational State Transfer.

### **2. REST APIs are designed around a \_\_\_\_**

resources.

### **3. What is an identifer of a resource? Give an example.**

URI that uniquely identifies that resource. For example, the URI for a particular customer order
:`https://adventure-works.com/orders/1`.

### **4. What are the most common HTTP verbs?**

GET, POST, PUT, PATCH, and DELETE.

### **.5 What should the URIs be based on?**

based on nouns (the resource) and not verbs (the operations on the resource).

### **.6 Give an example of a good URI.**

`https://adventure-works.com/orders`

### **.7 What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

APIs that expose a large number of small resources. and it's a bad thing because it's impose a load on the web server.

### **.8 What status code does a successful _GET_ request return?**

returns HTTP status code 200 (OK).

### **.9 What status code does an unsuccessful _GET_ request return?**

404 (Not Found).

### **.10 What status code does a successful _POST_ request return?**

HTTP status code 201 (Created).

### **.11 What status code does a successful _DELETE_ request return?**

the web server should respond with HTTP status code 204, indicating that the process has been successfully handled.

<hr>
<br>

**Sources**

- RESTful web API design / microsoft documention.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
