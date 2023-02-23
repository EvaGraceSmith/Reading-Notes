## Authentication

### [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

### What is OAuth?
"OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential."

#### Give an example of what using OAuth would look like.
If I am wanting to have a photo printed from Walgreens from my Google storage, it would give Walgreens auth to get the photo from Google without having to log in to both services. 

#### How does OAuth work? What are the steps that it takes to authenticate the user?

1. Walgreens to Google says "Hey, Eva needs me to get a photo, can I get a token to do this?"

2. Google to Walgreens says "Here is a single token with a secret code to get the photo"

3. Walgreens gives the token to Eva's client software with some secret sauce.

4. Eva's software gives the token and sauce to the Auth provider.

5. The Auth provider takes the sauce and token, might verify it is the right token and sauce. 

6. Eva (or her computer software says, yep! I would like you to get this photo.

7. Google now gives Eva an access token, (Yay!)

8. Eva give the token Walgreens. "Here ya go!"

9. Walgreens shows the access token to Google. "I have permission to get a photo!"

10. Google: "Okay, here is your photo."

11. Walgreens: "Yay, look Eva! I have a photo to print for you!"

#### What is OpenID?
Provides Authentication (not Authorization.)

"OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."

### [Authorization and Authentication flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)

### What is the difference between authorization and authentication?

Authorization : gives permission
Authentication : is verifying user information/identification

### What is Authorization Code Flow?

exchanges an Authorization Code for a token.

### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

Additional security for mobile and native applications

### What is Implicit Flow with Form Post?
it offers a streamlined workflow if the application needs only an ID token to perform user authentication.

(no longer considered a best practice for requesting Access Tokens)

### What is Client Credentials Flow?

the system authenticates and authorizes the app rather than a user. 

### What is Device Authorization Flow?

Rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. 

### What is Resource Owner Password Flow?

Requests that users provide credentials (username and password), typically using an interactive form.

## Videos

### [Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)


#### How does this subject matter as it relates to what I am studying?
We are adding OAuth to lab 15 and our upcoming project. 


#### Things I want to know more about:
How can we better secure transactions for customers?