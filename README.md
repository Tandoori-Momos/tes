RESTAPIDocs Examples
These examples were taken from projects mainly using Django Rest Framework and so the JSON responses are often similar to the way in which DRF makes responses.

Where full URLs are provided in responses they will be rendered as if service is running on 'http://testserver/'.

Open Endpoints
Open endpoints require no Authentication.

Login : POST /api/login/
Endpoints that require Authentication
Closed endpoints require a valid Token to be included in the header of the request. A Token can be acquired from the Login view above.

Current User related
Each endpoint manipulates or displays information related to the User whose Token is provided with the request:

Show info : GET /api/user/
Update info : PUT /api/user/
Account related
Endpoints for viewing and manipulating the Accounts that the Authenticated User has permissions to access.

Show Accessible Accounts : GET /api/accounts/
Create Account : POST /api/accounts/
Show An Account : GET /api/accounts/:pk/
Update An Account : PUT /api/accounts/:pk/
Delete An Account : DELETE /api/accounts/:pk/
