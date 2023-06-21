# Authentication-using-JWT-token
Authentication using JSON Web Tokens (JWT) is a popular method for implementing secure authentication and authorization in web applications and APIs. 
JWT is a compact, URL-safe token format that contains encoded information, allowing it to securely represent claims between two parties.

Below is the actual working :
**1. **Frontend:****
   - Collects the user's credentials (e.g., username and password) through a login form or user interface.
   - Sends the user's credentials securely to the backend for authentication.
**2. **Backend:****
   - Receives the user's credentials from the frontend.
   - Authenticates the user by verifying the credentials against a database or other authentication system.
   - If the credentials are valid, the backend generates a token (e.g., JWT) using a library or framework specifically designed for token generation.
   - The token is typically signed by the backend using a secret key or private key.
   - The generated token is then sent back to the frontend as a response to the login request.
**3. Frontend:**
   - Receives the token from the backend as part of the response to the login request.
   - Stores the token securely, typically using browser storage mechanisms like local Storage, sessionStorage, or secure HTTP-only cookies.
   - Includes the token in subsequent requests to the backend, typically in the Authorization header using the "Bearer" scheme.
**4. Backend:**
   - Receives subsequent requests from the frontend that include the token in the Authorization header.
   - Verifies the authenticity and validity of the token by checking the signature or using the secret key or public key associated with the token.
   - Performs authentication and authorization checks based on the extracted token information.
   - Responds to the frontend request based on the authentication and authorization results.

