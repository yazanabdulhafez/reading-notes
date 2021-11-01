# Spring Authorization

## Spring Boot and OAuth2

The sample apps can be easily extended and re-configured for more specific use cases,there are multi sample apps to build:

* simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties when visit home you redirected to GitHub.

* click: adds an explicit link that the user has to click to login.

* logout: adds a logout link as well for authenticated users.

* two-providers: adds a second login provider so the user can choose on the home page which one to use.

* custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.

## Single Sign On With GitHub

* Creating a New Project

to create a new project we go to <https://start.spring.io> and generate an empty project.

* Add a Home Page

* Securing the Application with GitHub and Spring Security

* Add a New GitHub App

## Add a Welcome Page

* Conditional Content on the Home Page

* The /user Endpoint

* Making the Home Page Public: becouse the app work fine and authenticate, but it’s still going to redirect before showing the page. you need to make the link visible.

## Add a Logout Button

* Client Side Changes
* Adding a Logout Endpoint
* Adding the CSRF Token in the Client

## Login with GitHub

* Setting the redirect URI
* Adding the Client Registration
* Adding the Login Link

## How to Add a Local User Database

1. Choose a backend for your database, and set up some repositories.

2. Implement and expose OAuth2UserService to call the Authorization Server as well as your database.

## Adding an Error Page for Unauthenticated Users

* Switching to GitHub
* Detecting an Authentication Failure in the Client
* Adding an Error Message
* Generating a 401 in the Server

## Resources used in this reading note

1. [Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)
