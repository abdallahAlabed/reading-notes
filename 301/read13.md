# CRUD :
**1- In your own words, describe what each group of status code represents:**
- 100’s = Informational status codes. Header part of request has been recieved, and server will try to comply with response.
- 200’s = Success codes. Saying that a request was accepted. For an asyn processing of request
- 300’s = Redirection codes. The code one is trying to access is not available at the current time of the error.
- 400’s = Client error codes. Timeouts, wrong URI, missing auth… A client is doing something wrong- sending the wrong info.
- 500’s = The server encountered an unexpected condition which prevented it from fulfilling the request.
**2- What is a status code 202?**
- The request has been received but not yet acted upon.
**3- What is a status code 308?**
- This means that the resource is now permanently located at another URI
**4- What code would you use if an update didn’t return data to a client?**
- A 204, ‘No Content’ error. For things like saving something they have just changed.
**5- What code would you use if a resource used to exist but no longer does?**
- 410 Gone
**6- What is the ‘Forbidden’ status code?**
- 403 ‘Forbidden.’ This happens after authorization has been accepted, or if auth is not necessary, but the client does not have correct permissions to use the resource.
---
**1- Why do we need to pull our MongoDB database string out of our server and put it into our .env?**
- This is because when working on the code locally, you want to store the database as a local environment variable. This adds security and flexibility.
**2- What is middleware?**
- is software that provides common services and capabilities to applications outside of what's offered by the operating system.
**3- What does app.use(express.json()) do?**
- it is a method inbuilt in express to recognize the incoming Request Object as a JSON Object.
**4- What does the /:id mean in a route?**
- params object, with the name of the route parameter specified in the path as their respective keys
**5- What is the difference beween PUT and PATCH?**
- The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.
**6- How do you make a defalut value in a schema?**
- Make mongoose string schema type default value as blank and make the field optional.
**7- What does a 500 error status code mean?**
- A 500 error means that there has been an error on the server. This is good to be placed within the catch of a try/catch statement, because if it fails, something is wrong within that function.
**8- What is the difference between a status 200 and a status 201?**
- 201 = successfully created object 200 = everything was successful The 201 is more specific, so if it can be used, for example in a post route, it should be used. More information is always better!