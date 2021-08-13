# Authentication

## What is OAuth

1. What is OAuth?
**OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.**
2. Give an example of what using OAuth would look like.
**The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.**
3. How does OAuth work? What are the steps that it takes to authenticate the user?

* .The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
* .The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
* .The first site gives this token and secret to the initiating user’s client software.
The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
* .If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
* .The user approves (or their software silently approves) a particular transaction type at the first website.
* .The user is given an approved access token (notice it’s no longer a request token).
The user gives the approved access token to the first website.
The first website gives the access token to the second website as proof of authentication on behalf of the user.
* .The second website lets the first website access their site on behalf of the user.
The user sees a successfully completed transaction occurring.
* .OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. What is OpenID?
**OpenID is for humans logging into machines**

## Authorization and Authentication flows

* .What is the difference between authorization and authentication?

**authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.**

* .What is Authorization Code Flow?

**which exchanges an Authorization Code for a token. Your app must be server-side because during this exchange, you must also pass along your application's Client Secret, which must always be kept secure, and you will have to store it in your client.**

* .What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
**The PKCE-enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server; this secret is called the Code Verifier. Additionally, the calling app creates a transform value of the Code Verifier called the Code Challenge and sends this value over HTTPS to retrieve an Authorization Code.**
* .What is Implicit Flow with Form Post?
**which is intended for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.**

* .What is Client Credentials Flow?
**With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow.**
* .What is Device Authorization Flow?
**With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text.**
* .What is Resource Owner Password Flow?
**which requests that users provide credentials (username and password), typically using an interactive form. Because credentials are sent to the backend and can be stored for future use before being exchanged for an Access Token, it is imperative that the application is absolutely trusted with this information.**

## Things I want to know more about

1. How to use OAuth.

## Resources used in this reading

1. <https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html>
2. <https://auth0.com/docs/flows/resource-owner-password-flow>