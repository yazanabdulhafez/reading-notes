# Spring Authorization

## Spring Boot and OAuth2

## Single Sign On With GitHub

Creating a New Project
First, you need to create a Spring Boot application, which can be done in a number of ways. The easiest is to go to <https://start.spring.io> and generate an empty project (choosing the "Web" dependency as a starting point).

Add a Home Page
In your new project, create index.html in the src/main/resources/static folder.

Securing the Application with GitHub and Spring Security
To make the application secure, you can simply add Spring Security as a dependency. Since you’re wanting to do a "social" login (delegate to GitHub), you should include the Spring Security OAuth 2.0 Client starter:

Add a New GitHub App
To use GitHub’s OAuth 2.0 authentication system for login, you must first Add a new GitHub app.

Select "New OAuth App" and then the "Register a new OAuth application" page is presented. Enter an app name and description. Then, enter your app’s home page, which should be <http://localhost:8080>, in this case. Finally, indicate the Authorization callback URL as <http://localhost:8080/login/oauth2/code/github> and click Register Application.

Making the Home Page Public: becouse the app work fine and authenticate, but it’s still going to redirect before showing the page. you need to make the link visible.

Add a Logout Button: adding a button that allows the user to log out of the app.

Adding a Logout Endpoint: The /logout endpoint requires us to POST to it, and to protect the user from Cross Site Request Forgery (CSRF, pronounced "sea surf"), it requires a token to be included in the request. The value of the token is linked to the current session.

Login with GitHub:

Initial setup.
Setting the redirect URI.
Adding the Client Registration.
Adding the Login Link.
Adding an Error Page for Unauthenticated Users: to give some feedback to users that cannot authenticate. And extends the authentication logic to include a rule that only allows users if they belong

## Resources used in this reading note

1. [Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)