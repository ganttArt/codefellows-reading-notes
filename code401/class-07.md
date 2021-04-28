# Reading: Bearer Authorization

## Review, Research, and Discussion

1. Write the following steps in the correct order:
    - Ask the client if they want to sign in via a third party
    - Redirect to a third party authentication endpoint
    - Register your application to get a client_id and client_secret
    - Receive authorization code
    - Make a request to the access token endpoint
    - Receive access token
    - Make a request to a third-party API endpoint
1. What can you do with an authorization code?
    - An authorization code is a short-lived token representing the user's access grant, created by the authorization server and passed to the client application via the browser. The client application sends the authorization code to the authorization server to obtain an access token and, optionally, a refresh token. src: [stackoverflow](https://stackoverflow.com/questions/8666316/facebook-oauth-2-0-code-and-token#:~:text=Access%20Token%20The%20access%20token,order%20of%20minutes%20or%20hours.)
1. What can you do with an access token?
    - Access Token The access token is used by the client to make authenticated requests on behalf of the end user. It has a longer lifetime than the authorization code, typically on the order of minutes or hours. When the access token expires, attempts to use it will fail, and a new access token must be obtained via a refresh token. src: [stackoverflow](https://stackoverflow.com/questions/8666316/facebook-oauth-2-0-code-and-token#:~:text=Access%20Token%20The%20access%20token,order%20of%20minutes%20or%20hours.)
1. What’s a benefit of using OAuth instead of your own basic authentication?
    - OAuth contains authorization requests, access tokens and refresh tokens. src: [stackoverflow](https://stackoverflow.com/questions/7561631/oauth-2-0-benefits-and-use-cases-why#:~:text=OAuth1%20(more%20precisely%20HMAC)%20requests,the%20data%20you're%20after.). It's a standard that makes your website or api more secure.

## Vocabulary Terms

- **Client ID** - A Client ID represents a unique browser/device and is created and assigned by Universal Analytics cookie _ga. Client ID is assigned to each unique user of your website. src: [optimizesmart](https://www.optimizesmart.com/understanding-the-difference-between-client-id-and-user-id/#:~:text=Analytics%20client%20ID%3F-,A%20Client%20ID%20represents%20a%20unique%20browser%2Fdevice%20and%20is,unique%20user%20of%20your%20website.)
- **Client Secret** - a secret used by the OAuth Client to Authenticate to the Authorization Server. The Client Secret is a secret known only to the OAuth Client and the Authorization Server. src: [ldapwiki](https://bit.ly/3tYHpqJ)
- **Authentication Endpoint** - used to request either access tokens or authorization codes. [src](https://identityserver.github.io/Documentation/docsv2/endpoints/authorization.html)
- **Access Token Endpoint** - used by the application in order to get an access token or a refresh token. src: [auth0](https://auth0.com/docs/protocols/protocol-oauth2)
- **API Endpoint** - the point of entry in a communication channel when two systems are interacting. It refers to touchpoints of the communication between an API and a server. src: [rapidapi](https://rapidapi.com/blog/api-glossary/endpoint/#:~:text=In%20simple%20terms%2C%20an%20API,an%20API%20and%20a%20server.)
- **Authorization Code** - an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space. [src](https://www.investopedia.com/terms/a/authorization-code.asp#:~:text=What%20Is%20an%20Authorization%20Code,into%20a%20security%2Dprotected%20space.)
- **Access Token** - an object encapsulating the security identity of a process or thread. A token is used to make security decisions and to store tamper-proof information about some system entity. src: [wiki](https://en.wikipedia.org/wiki/Access_token#:~:text=An%20access%20token%20is%20an,information%20about%20some%20system%20entity.)

## Preview

- [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)
- [Intro to JWT](https://jwt.io/introduction/)
- [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)
- [npm jsonwebtoken docs](https://www.npmjs.com/package/jsonwebtoken)

1. Which 3 things had you heard about previously and now have better clarity on?
    - JSON Web Token clarification: uses an open standard, used to securely transfer infomation between two places, digitally signed (verified and trusted).
    - A good why to use this: It is compact so it can be sent via url, post request or http headers. This makes transmission fast.
    - A JWT is actually made of 3 parts, a header, payload and a signature. Which are all Base64 encoded from the data that you've provided. These parts are combined with a `.`. The signature relies on the first two parts, so you can't change one without breaking the JWT.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - When should we consider using alternatives to JWTs?
    - When and how did JWT become the standard?... assuming that it is.
    - How do you come up with the secret for the JWT?
1. What are you most excited about trying to implement or see how it works?
    - Making a custom JWT, looking more into the JWT docs and seeing what functions could be useful in making my applications more secure.
