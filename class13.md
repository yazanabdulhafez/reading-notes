# CRUD

## Status Codes Based On REST Methods

1. In your own words, describe what each group of status code represents:
**100’s =These are informational status codes; they usually tell the client that the header part of the request has been received**
**200’s =These are the success codes. They tell the client that its request was accepted**
**300’s =These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore.**
**400’s =These are the client error codes. They are all about invalid requests a client sent to a server.**
**500’s =These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies.**

2. What is a status code 202?
**This code tells the client that the request was valid, but its processing will finish sometime in the future**
3. What is a status code 308?
**This tells the client to use another URL to access the resource and not use the current URL anymore.**
4. What code would you use if an update didn’t return data to a client?
**204 No Content**
5. What code would you use if a resource used to exist but no longer does?
**410**
6. What is the ‘Forbidden’ status code?
**403**

## Build A REST API With Node.js, Express, & MongoDB 

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
**when we want to deploy our applcation we dont want to use localhost in it.**
2. What is middleware?
**code that runs when the server get request but before passed route**
3. What does app.use(express.json()) do?
**accept the json file and use it.**
4. What does the /:id mean in a route?
**It does: req.params.id**
5. What is the difference beween PUT and PATCH?
`PUT is a method of modifying resource where the client sends data that updates the entire resource.`
`Unlike PUT, PATCH applies a partial update to the resource.`

6. How do you make a defalut value in a schema?
**use default : Date.now**
7. What does a 500 error status code mean?
**error in the server**
8. What is the difference between a status 200 and a status 201?
**200: the request was received and understood and is being processed.**
**201: a request was successful and as a result, a resource has been created**

## Things I want to know more about

1. build a REST API with node js.

## Resources used in this reading

1. <https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/>
2. <https://aloneonahill.com/blog/http-status-codes>
3. <https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw>
