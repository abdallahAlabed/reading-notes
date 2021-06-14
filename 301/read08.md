# API Design Best Practices
* What does REST stand for?
    > an architectural style for building distributed systems based on hypermedia
* REST APIs are designed around a _ resources___.
* What is an identifer of a resource? Give an example.
    > URI that identifies the resource /  https://adventure-works.com/orders/1
* What are the most common HTTP verbs?
   > GET, POST, PUT, PATCH, and DELETE.
* What should the URIs be based on?
   > nouns (the resource) and not verbs (the operations on the resource)
* Give an example of a good URI.
   > /customers
* What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
    >large number of small resources/bad
* What status code does a successful GET request return?
    > returns HTTP status code 200 (OK)
* What status code does an unsuccessful GET request return?
    > 404 (Not Found).
* What status code does a successful POST request return?
    > HTTP status code 201 
* What status code does a successful DELETE request return?
    >  HTTP status code 204