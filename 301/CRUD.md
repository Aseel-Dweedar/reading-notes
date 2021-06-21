# CRUD

## **1. In your own words, describe what each group of status code represents:**

- 100’s = tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client.

- 200’s = tell the client that its request was accepted. In case of asynchronous processing of a request (202).

- 300’s = tell the client that the resource they are requesting isn’t available at the expected location anymore.

- 400’s = These are the client error codes. They are all about invalid requests a client sent to a server.

- 500’s = These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies.

### **2. What is a status code 202?**

This code tells the client that the request was valid, but its processing will finish sometime in the future.

### **3. What is a status code 308?**

This tells the client to use another URL to access the resource and not use the current URL anymore.

### **4. What code would you use if an update didn’t return data to a client?**

204 No Content.

### **5. What code would you use if a resource used to exist but no longer does?**

410 Gone.

### **6. What is the ‘Forbidden’ status code?**

The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

<br>

# Build A REST API With Node.js, Express, & MongoDB

### **1.Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

Maybe we have sensitive information that we don't want to push it to GitHub.

### **2. What is middleware?**

functions which are passed control during execution of asynchronous functions.

### **3. What does app.use(express.json()) do?**

will allow us to use any middleware that we want.

### **4. What does the /:id mean in a route?**

this means that this is a parameter that we can access by typing in request: `rec.pram.id`

### **5. What is the difference between PUT and PATCH?**

- **_put_** update all the information it all at once.
- **_PATCH_** update just the information that gets passed

### **6. How do you make a default value in a schema?**

We use ` default : Date.now`

### **7. What does a 500 error status code mean?**

that there's an error on your server.

### **8. What is the difference between a status 200 and a status 201?**

200 which means everything was successful but 201 is more specific means successfully created an object .

<hr>
<br>

**Sources**

- Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/ moesif Blog.

- Build A REST API With Node.js, Express, & MongoDB - Quick / Web Dev Simplified.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
