# LaunchPad
This simple app is used for logging into internal web apps form a central location. It's a little like Single Sign On but not quite since we rolled our own. 

The user logs in with their Active Directory credentials and is authenticated on the backend and if the user is authenticated the server responds with some basic user information including a JWT. The reponse object is stored in localstorage and the JWT is sent back with every request across all the apps by using an http interceptor.

In this simple app once the user is authenticated the route changes and a call is made to the api to retrieve a list of applications that a user has access to based on a SQL DB Table and Active Directory group membership.



## Get Going
```bash
$ npm install
```

