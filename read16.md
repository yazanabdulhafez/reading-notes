# Spring Authentication

## Spring Security Architecture

### Authentication and Access Control

authentication is who are you and authorization are the things that you allowed to do.

#### Authentication

The main strategy interface for authentication is AuthenticationManager

```java
public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}
```

An AuthenticationManager can do in its authenticate() method:

1. Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.

2. Throw an AuthenticationException if it believes that the input represents an invalid principal.

3. Return null if it cannot decide.

#### Customizing Authentication Managers

Helpers used in spring to quickly get the authentication manager features set up. The most commonly used helper is the AuthenticationManagerBuilder which is great for setting up in-memory, JDBC, or LDAP user details

#### Authorization or Access Control

Once authentication is successful, we can move on to authorization, and the core strategy here is AccessDecisionManager.

Most people use the default AccessDecisionManager, which is if any voters return affirmatively, access is granted.

### Web Security

![spring security](https://1.bp.blogspot.com/-7UzovikCjTo/X-BCL0XC4oI/AAAAAAAAlD0/mSDIoH05IM07EjFPcSv1yMF9K3_wyhY-wCLcBGAsYHQ/w400-h274/multi-securityfilterchain%2Bin%2Bspring%2Bsecurity.png)

* Spring Security in the web tier (for UIs and HTTP back ends) is based on Servlet Filters.

* All filters internal to Spring Security are unknown to the container is important, especially in a Spring Boot application, where, by default, all @Beans of type Filter are registered automatically with the container.

* Spring Security is installed as a single Filter in the chain, and its concrete type is FilterChainProxy.

* To add a custom filter to the security chain, you need to either not make it be a @Bean or wrap it in a FilterRegistrationBean that explicitly disables the container registration.

### Creating and Customizing Filter Chains

The default fallback filter chain in a Spring Boot application (the one with the /** request matcher) has a predefined order of SecurityProperties.BASIC_AUTH_ORDER.

### Request Matching for Dispatch and Authorization

* WebSecurityConfigurerAdapter its a security filter chain has a request matcher used to decide whether to apply it to an HTTP request.

* In a filter chain, you can have more fine-grained control of authorization by setting additional matchers in the HttpSecurity configurer.

### Combining Application Security Rules with Actuator Rules

* When you add actuater to a secure an application then you can get an additional filter chain that applies only to the actuator endpoints.

* If you want your application security rules to apply to the actuator endpoints, you can add a filter chain that is ordered earlier than the actuator one and that has a request matcher that includes all actuator endpoints.

* If you prefer the default security settings for the actuator endpoints, the easiest thing is to add your own filter later than the actuator one.

* Spring Security in the web tier is currently tied to the Servlet API

## Method Security

* Spring Security offers support for applying access rules to Java method executions.

* There are other annotations to enforce security constraints:

1. notably @PreAuthorize
2. @PostAuthorize

## Working with Threads

Spring Security is fundamentally thread-bounddue to it needs to make the current authenticated principal available to a wide variety of downstream consumers.

### Processing Secure Methods Asynchronously

SecurityContext is a thread-bound, if you want to do any background processing that calls secure methods, you need to ensure that the context is propagated.

## Resources used in this reading

1. [Spring Security Architecture](https://spring.io/guides/topicals/spring-security-architecture/)
2. [Spring Auth Cheat Sheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)
