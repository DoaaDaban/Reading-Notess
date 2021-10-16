# Spring Security overview

* In the *Spring Security* we have two concepts:

  1. **Authentication**: that means who are you?

  2. **Authorization**: that means what are you allowed to do?

## Authentication

* The application needs to verify if the user is who he/she claims to be, typically done with a username and password check.

* For **Authentication** in spring we use the `AuthenticationManager` interface which has only one method:

```
public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}
```

An `AuthenticationManager` can do one of 3 things in its `authenticate()` method:

* Return an Authentication (normally with `authenticated=true`) if it can verify that the input represents a valid principal.

* Throw an `AuthenticationException` if it believes that the input represents an invalid principal.

* Return `null` if it cannot decide.

## Web Security 

The web Security in Spring is based on Sevlet Filters. It consists of several layers, each layer has a certain function when receiving a single HTTP request. For example, single HTTP request would:

1. Go through a LoginMethodFilter.

2. Then go through an AuthenticationFilter.

3. After that go through an AuthorizationFilter.

4. Finally hit the servlet.

