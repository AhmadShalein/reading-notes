# Read 08: APIs:

## API Design Best Practices:

**What does REST stand for?**

- Representational State Transfer.

**REST APIs are designed around a ____.**

- Designed around resources.

**What is an identifer of a resource? Give an example.**

- A URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:
`https://adventure-works.com/orders/1`

**What are the most common HTTP verbs?**

- The most common operations are GET, POST, PUT, PATCH, and DELETE.

**What should the URIs be based on?**

- Resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

**Give an example of a good URI.**

- `https://adventure-works.com/orders`

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

- "chatty" web APIs that expose a large number of small resources. Such API may require a client application to send multiple requests to find all of the data that it requires. And we should avoid using such API's and instead denormalizing the data and combining related information into bigger resources.

**What status code does a successful `GET` request return?**

- HTTP status code 200 (OK).

**What status code does an unsuccessful `GET` request return?**

- HTTP status code 404 (Not Found).

**What status code does a successful `POST` request return?**

- HTTP status code 201 (Created).

**What status code does a successful `DELETE` request return?**

- HTTP status code 204.

---------------------------------------------------------------------

### Things I want to know more about:

- HTTP requests and how to use them efficiently.
