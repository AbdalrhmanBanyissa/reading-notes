# CRUD

## Status Codes Based On REST Methods

- The "CREATE" action is usually implemented via HTTPS POST method - used to create new resources or access tokens

- The "READ" action is usually implemented via HTTPS GET method - used to fetch resource representations.

- The "UPDATE" action is usually implemented via HTTP PUT or PATCH method.

  - `PUT` requires client to send ENTIRE representation of a resource to update it (Replace the old with a new one)

  - `PATCH` requires client only send parts of representation of a resource (Add, update, or delete these parts in the old version)

- The "DELETE" action can be implemented via HTTP DELETE method.

1.In your own words, describe what each group of status code represents:

- 100’s = Informational status.
- 200’s = Success - Request was accepted
- 300’s = Redirection - Requested resource isn't at the location anymore.
- 400’s = Client error - Client information/input is invalid.
- 500’s = Server error - Overwhelmed servers, unreachable servers, client requests triggering errors on the server.

2.What is a status code 202?

- Asynchronous processing of a request - it's waiting to process

3.What is a status code 308?

- Permanent redirect - Resource lives at a different URL and we can tell the client what it is

4.What code would you use if an update didn’t return data to a client?

- 204 - Update that doesn't return data to a client, for example when just saving a currently edited document.

5.What code would you use if a resource used to exist but no longer does?

- 410 - Gone: Resource was deleted or moved somehow, don't know where it is.

6.What is the ‘Forbidden’ status code?

- 403: Client has authorized but still doesn't have permissions to access the resource.

- Build A REST API With Node.js, Express, & MongoDB

- Dev dependency "nodemon" allows server to refresh upon making changes to the server code without having to stop/start the server

1.Why do we need to pull our MongoDB database string out of our server and put it into our .env?

- Because we'll want to change it from localhost to something else when we deploy our application. Setting it as a .env variable makes it easier to change later, and keeps it secret.

2.What is middleware?

- Code that runs when the server gets a request, but before it gets passed to the routes.

3.What does app.use(express.json()) do?

- app.use allows the server to accept middleware - this example allows the server to accept json as a body instead of a post element or git element.

4.What does the /:id mean in a route?

- It is an id parameter passed in - the colon in front means this is a param being passed in

5.What is the difference beween PUT and PATCH?

- PUT replaces an entire old version with a whole new version, PATCH replaces pieces of the old version with new pieces.

6.How do you make a defalut value in a schema?

- Add a "default" key into the schema object with a set value (Example: default value of a dateJoined object could use Date.now)

7.What does a 500 error status code mean?

- Error on the server causing the transaction to not work - it wasn't user or client fault.

8.What is the difference between a status 200 and a status 201?

- Status 200 tells client everything went good, whereas Status 201 confirms a resource was created successfully.
