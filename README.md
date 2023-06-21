# Authentication-using-JWT-token
Authentication using JSON Web Tokens (JWT) is a popular method for implementing secure authentication and authorization in web applications and APIs. JWT is a compact, URL-safe token format that contains encoded information, allowing it to securely represent claims between two parties.

-USERNAME AND PASSWORD FOR THIS PROJECT IS STATIC(DATABASE LAYER IS NOT IMPLEMENTED)

- **GET** http://localhost:8080/  //Will return user a message if the user is authentic (using token) else it will show "**_access to localhost was denied_**".
 ![image](https://github.com/pg348/Authentication-using-JWT-token/assets/89197939/9a58efc0-736c-4027-823d-125598cd7221)


- **POST** http://localhost:8080/authenticate //Need to POST username and password(password is encoded) if it matches then it generates a JWT token with expiration
 time as 5hrs.
 ![image](https://github.com/pg348/Authentication-using-JWT-token/assets/89197939/b8187db7-0067-4292-b3c2-b59bbd984bdb)

- After generation of token if we will again hit the GET api with authorization-**type bearer** and above generated token ||**the message will be displayed**||.
![image](https://github.com/pg348/Authentication-using-JWT-token/assets/89197939/b42349b7-236b-4915-81ba-d98da4f40916)


- ALGO USED "HS512".

OUTCOME:- while the frontend collects user credentials and includes the token in subsequent requests, the backend is responsible for generating the token, verifying its authenticity, and performing authentication and authorization checks

