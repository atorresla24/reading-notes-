# Reading 15

## What is OAuth

1. OAuth is an open-standard authorization protocol or framwork that descrobes how unrelated services and servers can safely allow authenticated access to their assets without sharing the initial, related, single logon credential. It allows websites and services to share assets among users
2. An example of OAuth is myriad which uses a single physical sign-on to access sites that are unrelated to each other
3. OAuth focuses on authorization which is the process of letting a subject access resources after a single successful authentication. 
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. 6. After authentication, the client is asked to approve the authorization transaction to the second website.
7. The user approves (or their software silently approves) a particular transaction type at the first website.
8. The user is given an approved access token (notice it’s no longer a request token).
9. The user gives the approved access token to the first website.
10. The first website gives the access token to the second website as proof of authentication on behalf of the user.
11. The second website lets the first website access their site on behalf of the user.
The user sees a successfully completed transaction occurring.
12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).
4. OpenID is for humans logging into machines

## Authorization and Authentication flows

1. Authentication is the process of a user proving ownership by providing a passwrod or other unique factor but authorization is the process of letting a subject access resources after successfully authenticating once
2. Authorization code flow exchanges an Authorization code for a token which will allow granted access for a certain amount of time
3. Authorization code flow with proof key for code exchange is required additional security. A single-page can have special challenges.
4. Implicit flow with form post is intended for Public Clients and offers a streamlined workflow if the app needs only an ID token to perform user authentication
5. Client credentials flow is machine-to-machine applications that will have the system authenticate and authorize the app rather than a user
6. Device authorization instead of authenticating the user directly it asks the device to be authorized through a link. 
7. Resource owner password flow requests that a user provides credentials typically using an interactive form. 