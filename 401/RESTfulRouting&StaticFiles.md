# Spring RequestMapping

the annotation is used to map web requests to Spring Controller methods:

**RequestMapping Basics**

- RequestMapping — by Path.
- RequestMapping — the HTTP Method : The HTTP method parameter has no default. So, if we don't specify a value, it's going to map to any HTTP request.

**RequestMapping and HTTP Headers**

- RequestMapping With the headers Attribute : The mapping can be narrowed even further by specifying a header for the request:

- RequestMapping Consumes and Produces.

**RequestMapping With Path Variables**

- Single @PathVariable : If the name of the method parameter matches the name of the path variable exactly, then this can be simplified by using `@PathVariable` with no value.

- Multiple @PathVariable: A more complex URI may need to map multiple parts of the URI to multiple values.

- @PathVariable With Regex.

**RequestMapping With Request Parameters**

`@RequestMapping` allows easy mapping of URL parameters with the @RequestParam annotation.

**RequestMapping Corner Cases**

- @RequestMapping — Multiple Paths Mapped to the Same Controller Method : Although a single @RequestMapping path value is usually used for a single controller method (just good practice, not a hard and fast rule), there are some cases where mapping multiple requests to the same method may be necessary.

- @RequestMapping — Multiple HTTP Request Methods to the Same Controller Method.

- @RequestMapping — a Fallback for All Requests.

- Ambiguous Mapping Error : The ambiguous mapping error occurs when Spring evaluates two or more request mappings to be the same for different controller methods. A request mapping is the same when it has the same HTTP method, URL, parameters, headers, and media type.

# Crud Repository

## Spring Data Repositories

Each of these defines its own functionality:

- **CrudRepository** provides CRUD functions
- **PagingAndSortingRepository** provides methods to do pagination and sort records.
- **JpaRepository** provides JPA related methods such as flushing the - persistence context and delete records in a batch.

because of this inheritance relationship, the JpaRepository contains the full API of CrudRepository and PagingAndSortingRepository. we can simply use the `CrudRepository`.

**The typical CRUD functionality:**

`save(…) - findOne(…) - findAll() - count() - delete(…) - exists(…).`
**JpaRepository**

methods:

- `findAll()` - `save(…)` - `flush()` - `saveAndFlush(…)` - `deleteInBatch(…)`.

<hr>
<br>

**Sources**

- Spring RequestMapping / baeldung.

- CrudRepository / baeldung.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
