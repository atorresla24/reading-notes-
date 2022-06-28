# Reading 12

## Status Codes Based on REST Methods

1. 100 - Before any type of information is recieved it will say if the information will be passed on or not
200 - Depending on what is done correclty a certain 200s code will be sent
300 - Lets a user know that whatever information they are trying to find is no longer at the location is was previously
400 - Invalid requests that a client sent to the server
500 - Indicates that there is an error on the side of the server
2. A status code of 202 means **accepted** and tells the client that the request was valid but its processing will finish some time in the future.
3. A status code of 308 means **permanent redirect** and tells the client to use another URL to access the resource and not use the current URL anymore
4. A status code of 204 would be used if an update didn't return data to a client
5. A status code of 404 would be used to describe a resource used to exist but no longer does
6. The 'Forbidden' status code is 403 and tells the client that it has no permissions to access the resource

## Build A REST API With Node.js, Express, & MongoDB - Quick

1. We need to pull our MongoDB database string out of our server and put it into our .env because we want to use something that is not our local host
2. Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system
3. app.use(express.json()) parses incoming JSON requests and puts the parsed data in req
4. In a router /:id means that it is a parameter
5. The difference between Put and Patch is that PUT is a method of modifying resource where the client sends data that updates the entire resource while, Patch is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data
6. You make a default value in a schema by using the default keyword
7. A 500 error status code means there is an internal server error indicating that something is wrong in the server
8. The difference between a status 200 and a status 201 is that a status 200 means the client has requested documents from the server and a status 201 means that a request was successful and as a result a resource has been created. 

## Things I want to know more about

I want to know more about how I will know what parts of my code will require which status code

I want to know which status codes are the most important ones I need to know