# Spring Authentication

## Authentication and Access Control

Application security boils down to two more or less independent problems: authentication (who are you?) and authorization (what are you allowed to do?).

### [Authentication]

The main strategy interface for authentication is `AuthenticationManager`, which has only one method:

```java
public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}
```

`authenticate()` method:

- Return an `Authentication` if it can verify that the input represents a valid principal.

- Throw an `AuthenticationException` if it believes that the input represents an invalid principal.

- Return `null` if it cannot decide.

An `AuthenticationProvider` is a bit like an `AuthenticationManager`, but it has an extra method to allow the caller to query whether it supports a given Authentication type:

```java
public interface AuthenticationProvider {

	Authentication authenticate(Authentication authentication)
			throws AuthenticationException;

	boolean supports(Class<?> authentication);
}
```

> A `ProviderManager` has an optional parent, which it can consult if all providers return `null`. If the parent is not available, a `null Authentication` results in an `AuthenticationException`.

### [Customizing Authentication Managers]

The most commonly used helper is the `AuthenticationManagerBuilder`, which is great for setting up in-memory, JDBC, or LDAP user details or for adding a custom `UserDetailsService`.

> Note that the `AuthenticationManagerBuilder` is `@Autowired` into a method in a `@Bean` — that is what makes it build the global (parent) `AuthenticationManager`.

### [Authorization or Access Control]

Once authentication is successful, we can move on to authorization, and the core strategy here is `AccessDecisionManager`. There are three implementations provided by the framework and all three delegate to a chain of `AccessDecisionVoter` instances, a bit like the `ProviderManager` delegates to `AuthenticationProviders`.

```java
boolean supports(ConfigAttribute attribute);
boolean supports(Class<?> clazz);
int vote(Authentication authentication, S object,
        Collection<ConfigAttribute> attributes);
```

### [Web Security]

Spring Security in the web tier (for UIs and HTTP back ends) is based on Servlet Filters, so it is helpful to first look at the role of Filters generally. The following picture shows the typical layering of the handlers for a single HTTP request.

![filters](../img401/filters.png)

The order of the filter chain is very important, and Spring Boot manages it through two mechanisms: @Beans of type Filter can have an @Order or implement Ordered, and they can be part of a FilterRegistrationBean that itself has an order as part of its API.

### [Request Matching for Dispatch and Authorization]

A security filter chain has a request matcher that is used to decide whether to apply it to an HTTP request. Once the decision is made to apply a particular filter chain, no others are applied.

### [Method Security]

As well as support for securing web applications, Spring Security offers support for applying access rules to Java method executions. For Spring Security, this is just a different type of “protected resource”.

>     It is not uncommon to combine Web security and method security. The filter chain Tip provides the user experience features, such as authentication and redirect to login pages and so on, and the method security provides protection at a more granular level.

<hr>
<br>

**Sources**

- Spring Security Architecture / spring.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
