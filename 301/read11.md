
# What is OAuth?

## OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

## Give an example of what using OAuth would look like.

## Is when you go to log onto a website and then click on the button linked to the other website, the other website authenticates you.

## How does OAuth work? What are the steps that it takes to authenticate the user?

#### - The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
#### - The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
#### - The first site gives this token and secret to the initiating user’s client software.
#### - The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
#### - If not already authenticated to the authorization provider,the client may be asked to authenticate. After authentication,the client is 
#### - asked to approve the authorization transaction to the second website.
#### - The user approves (or their software silently approves) a particular transaction type at the first website.
#### - The user is given an approved access token (notice it’s no longer a request token).
#### - The user gives the approved access token to the first website.
#### - The first website gives the access token to the second website as proof of authentication on behalf of the user.
#### - The second website lets the first website access their site on behalf of the user.
#### - The user sees a successfully completed transaction occurring.

## What is OpenID?
### OpenID would serve as a single sign-in, vouching for the identities of users rather than having multiple logins for multiple websites.

## Authorization and Authentication flows:
## What is the difference between authorization and authentication?
### authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.

## What is Authorization Code Flow?
### exchanges an Authorization Code for a token

## What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
### The PKCE-enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server; this secret is called the Code Verifier.

## What is Implicit Flow with Form Post?
### It does offer a streamlined workflow if the application needs only an ID token to perform user authentication.

## What is Client Credentials Flow?
### the system authenticates and authorizes the app rather than a user.

## What is Device Authorization Flow?
### rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.

## What is Resource Owner Password Flow?
### requests that users provide credentials (username and password), typically using an interactive form.#### 