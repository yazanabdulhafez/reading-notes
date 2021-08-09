# APIs

## API Design Best Practices

1. What does REST stand for?**Representational State Transfer**

2. REST APIs are designed around a**REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.**

3. What is an identifer of a resource? Give an example.
**which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:HTTP`https://adventure-works.com/orders/1`**

4. What are the most common HTTP verbs?**The most common operations are GET, POST, PUT, PATCH, and DELETE.**

5. What should the URIs be based on?
**URIs should be based on nouns (the resource) and not verbs (the operations on the resource).**
Give an example of a good URI.
`https://adventure-works.com/orders // Good`
`https://adventure-works.com/create-order // Avoid`

6. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
**that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires**
**Its a bad thing**
7. What status code does a successful GET request return?
**A successful GET method typically returns HTTP status code 200 (OK).**
8. What status code does an unsuccessful GET request return?
**If the resource cannot be found, the method should return 404 (Not Found).**
9. What status code does a successful POST request return?
**It returns HTTP status code 201 (Created).**
10. What status code does a successful DELETE request return?
**the web server should respond with HTTP status code 204 (No Content)**

## Things I want to know more about

1. HTTP methods.

## Resources used in this reading

1. <https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design>
