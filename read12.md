# Spring RESTful Routing & Static Files

![spring annotation](https://2.bp.blogspot.com/-nhCHX8VGHF0/XLG6wSMv0RI/AAAAAAAANvE/rFJ9Ve7xJfU8k-xsWaaS9s8b7n2-Y45YACLcBGAs/s400/10%2BEssential%2BSpring%2BMVC%2BAnnotations%2BJava%2Bdevelopers%2Bshould%2Bknow.png)

## Spring RequestMapping

the annotation is used to map web requests to Spring Controller methods.

### RequestMapping Basics

mapping an HTTP request to a method using some basic criteria,it can be devided to:

1. @RequestMapping — by Path
2. @RequestMapping — the HTTP Method

### RequestMapping and HTTP Headers

The cases in this RequestMapping can be:

1. @RequestMapping With the headers Attribute
2. @RequestMapping Consumes and Produces

### RequestMapping With Path Variables

The cases in this RequestMapping can be:

1. Single @PathVariable
2. Multiple @PathVariable
3. @PathVariable With Regex

### RequestMapping With Request Parameters

@RequestMapping allows easy mapping of URL parameters with the @RequestParam annotation.

### RequestMapping Corner Cases

The cases in this RequestMapping can be:

1. @RequestMapping — Multiple Paths Mapped to the Same Controller Method
2. @RequestMapping — Multiple HTTP Request Methods to the Same Controller Method
3. @RequestMapping — a Fallback for All Requests
4. Ambiguous Mapping Error

Spring Framework new HTTP mapping annotations to make the RequestMapping easier:

* `@GetMapping`
* `@PostMapping`
* `@PutMapping`
* `@DeleteMapping`
* `@PatchMapping`

### Spring Configuration

simply need a @Configuration class to enable the full MVC support and configure classpath scanning for the controller.

## Spring Data repositories

There are diffrent data repositories in spring:

1. CrudRepository provides CRUD functions.
2. PagingAndSortingRepository provides methods to do pagination and sort records.
3. JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch.

There is inheritance relationship, the JpaRepository contains the full API of CrudRepository and PagingAndSortingRepository.

### CrudRepository

typical CRUD functionality:

1. save(…).
2. findOne(…).
3. findAll().
4. count().
5. delete(…).
6. exists(…).

## Resources used in this reading

1. [Spring RequestMapping](https://www.baeldung.com/spring-requestmapping)
2. [Accessing data jpa](https://spring.io/guides/gs/accessing-data-jpa/)
3. [Spring Data Repositories](https://www.baeldung.com/spring-data-repositories)