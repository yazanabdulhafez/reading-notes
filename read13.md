# Related Resources and Integration Testing

## Working with Relationships in Spring Data REST

### One-to-One Relationship

* we define one-to-one relationship using the @OneToOne annotation.
* We must be careful to have different names for each association resource.
* to expose these entities as resources by extending the CrudRepository interface.
* Before we create an association, sending a GET request to this endpoint will return an empty object.
* After persisting both instances, we can establish the relationship by using one of the association resources.

### One-to-Many Relationship

A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.

### Many-to-Many Relationship

A many-to-many relationship is defined using @ManyToMany annotation, to which we can add @RestResource.
we must first create the resources before we can establish the association.


## Testing the Endpoints With TestRestTemplate

we create a test class that injects a TestRestTemplate instance and define the constants we need then we can using @Test method:

1. Test the One-to-One Relationship
2. Test the One-to-Many Relationship
3. Test the Many-to-Many Relationship

## Integration Testing in Spring

### Spring MVC Test Configuration

* by adding the @ExtendWith annotation to the test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.clas
* We need the @ContextConfiguration annotation to load the context configuration and bootstrap the context that our test will use.
* How to configure and run the Spring enabled tests.
Finally, we also annotate the test with @WebAppConfiguration, which will load the web application context.

### Writing Integration Tests

1. Verify View Name
2. Verify Response Body
3. Send GET Request With Path Variable
4. Send GET Request With Query Parameters
5. Send POST Request

### MockMvc Limitations

MockMvc used to mock the HTTP requests and responses, it may not support all features of a full-blown Spring application.

## Resources used in this reading

1. [Working with Relationships in Spring Data REST](https://www.baeldung.com/spring-data-rest-relationships)
2. [Integration Testing in Spring](https://www.baeldung.com/integration-testing-in-spring)