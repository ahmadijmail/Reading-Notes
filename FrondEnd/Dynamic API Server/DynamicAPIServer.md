# Dynamic API Server


The path parameter defines the resource location, while the query parameter defines sort, pagination, or filter operations. The user's input (the query) is passed as a variable in the query parameter, while each path parameter must be substituted with an actual value when the client makes an API call.


**http://amazingapi.com/api/v1/products/12345**

/api/v# where # is the version number of our API

/model where ‘model’ is the name of the data model to operate on

/id where ‘id’ is the id number of a specific entity in the data model


### User Roles will be pre-defined and will each have a list of allowed capabilities:
 

admin can read, create, update, delete

editor can read, create, update

writer can read, create

user can read



ign In (OAuth)
The OAuth processes is initiated in the browser, using a 3rd party authentication/authorization service. It will, once the user has granted permission, invoke a GET on your /oauth route. The OAuth middleware should at this point complete the handshaking process, create/update a local user account in our database, and return an object with a re-authentication/bearer token and the user object

GET http://yourauthserver.com/oauth

Output from the server should be the same as with **Basic Authentication”:

Re-Authentication (Bearer Auth)
POST http://yourauthserver.com/signin

Send Basic Authentication Header

Authorization: Basic encodedpasswordcombo

With httpie from the command line: -a awesomecoder:youcantguessthis33!

With an HTTP REST client, use “Basic Auth” and set the username and password

From a website that has a login form, using Basic Auth, enter the username and password

Query String and Request Body shall be ignored