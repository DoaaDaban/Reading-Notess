
# CRUD

## Status Codes Based On REST Methods

**In your own words, describe what each group of status code represents:**

**100’s =** These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.

**200’s =** These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

**300’s =** These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

**400’s =** These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.

**500’s =** These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

**What is a status code 202?**

202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

**What is a status code 308?**

308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

**What code would you use if an update didn’t return data to a client?**

204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

**What code would you use if a resource used to exist but no longer does?**

410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

**What is the ‘Forbidden’ status code?**

403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

Reference [**Status Codes Based On REST Methods**](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

---

## Build A REST API With Node.js, Express, & MongoDB - Quick

**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

**What is middleware?**

The code that run when the server get the request but before it gets passed to your route.

**What does app.use(express.json()) do?**

Let our server accept JSON as a body inside a post element our Router etc..

**What does the /:id mean in a route?**

if we time it like this /:id it means that it is a prameter that could be access by typing in request.

**What is the difference beween PUT and PATCH?**

PUT updates only what the user give it on the other hand PUT updates the whole resource.

**How do you make a defalut value in a schema?**

**What does a 500 error status code mean?**

500 status code mean that there is an error on your server.

**What is the difference between a status 200 and a status 201?**

The difference between them is that status 201 is more specific.

Reference [**Build A REST API With Node.js, Express, & MongoDB - Quick**](https://www.youtube.com/watch?v=fgTGADljAeg)

---

## Things I want to know more about?