1. Self signed certificate:
   openssl req -x509 -newkey rsa:4096 -nodes -keyout key.pem -out cert.pem -days 365

2. Helmet.js
   Secure server, prevent data leaking and etc.

3. Auth = Authentication + Authorization
   401 - Unauthorized (authentication)
   403 - Forbidden (authorization)

   Authentication - validates that users are who they are (register, log in)
   Authorization - user has permission to the data (privileges, rights)

4. JWT - JSON web tokens, type of tokens. Set of credentials that grant access.
   Don't require additional. Extend server functionality. BASE64 encode.
   Includes header, payload and signature, separated by comma.
   Works only with https

5. OAuth - standard, flow based on redirects
   User (Resource Owner) ->
   We page (Client) + BE (Resource server) ->
   Redirect to the page where user enters credentials (Authorization Server) ->
   Redirect to the initial page with token

   Helps to keep password safe.
