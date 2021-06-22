# Read 13: CRUD:

## Status Codes Based On REST Methods:

**In your own words, describe what each group of status code represents:**

- 100’s = These are informational status codes; From the request of the client the header part will be received and the server will response, for example telling the user to switch the protocol or a failure has occured before sending the body.

- 200’s = These are the success codes. Accepted request will be shown to the client.

- 300’s = These are redirection codes. The location that requested from isn't available anymore, so the client has to target a new one.

- 400’s = These are the client error codes. Timeouts, wrong URI, missing authentication. The user has to make sure to send the correct parameters in the search query.

- 500’s = These are the server error codes. They indicate problems with overwhelmed servers or unreachable servers behind proxies. Refreshing the request or re-send it againg would be the best to solve this issue from the client side.

**What is a status code 202?**

- It tells the client the request was valid but the processing will end soon, so It should provide him with another URL or endpoint to reach the tarqet, or when it will be available again.

**What is a status code 308?**

- Same like 202 but provided with the location, ome clients follow the status codes of the Redirect-class automatically. This code is usually only used for POST requests.

**What code would you use if an update didn’t return data to a client?**

- 204 No Content.

**What code would you use if a resource used to exist but no longer does?**

- 307 Temporary Redirect.

**What is the ‘Forbidden’ status code?**

- The client has already authorized or maybe doesn't need to do that, but still he can't access the resource.

---------------------------------------------------------------------

## Build A REST API With Node.js, Express, & MongoDB (Video):

**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

- To be ignored after pushing the code, to visible ony for me.

**What is middleware?**

- A function when be called will be move on to the next section of the code. Excuting the code like partitons sequentially.

**What does app.use(express.json()) do?**

- Let the server accept JSON as a body inside a POST or GET element.

**What does the /:id mean in a route?**

- To get only one object.

**What is the difference beween PUT and PATCH?**

- PUT: For creating a new route.

- PATCH: Updating a route that already exists.

**How do you make a defalut value in a schema?**

Passing inside the object as a parameter a default type then give it the value that we want it to be default.
{
	default: 'Hello'
}

**What does a 500 error status code mean?**

- Mean that there's an error on the server(Database)=> Has some errors that caused that actual transactions not to work and had nothing to do with the actuall user or client using the API.

**What is the difference between a status 200 and a status 201?**

- 201 => Successfully created an object

---------------------------------------------------------------------

### Things I want to know more about:

- About databases.
