# Class 11 - Authorization & Authentication

## [What is OAuth? How the open authorization framework works](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

- OAuth allows websites and services to share assets among users.
- OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.
- This is as secure, third-party, user-agent, delegated authorization.
- OAuth is widely accepted by the top tech companies.
- OAuth is used for more cases than just loging in to another place with other credentials. In all cases, two or more services are being used for one transaction by the end-user, and every end-user would appreciate not being asked to log in a second time for what they feel is a single transaction.
- OAuth stands for authorization, not authentication
- OAuth vs. OpenID
  - OpenID is about authentication
  - "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."
  - OpenID as it was conceived no longer exists but was reinveded as an authentican layer for OAuth in 2014
- OAuth vs. SAML
  - SAML describes a framework that allows one computer to perform both authentication and authorization on behalf of one or more other computers.
  - It relies on XML protocols which have become less popular, where OAuth uses JSON for encoding data.
  - SAML is more often used for enterprise applications, Salesforce uses it. OAuth is more often used in the open internet.
- OAuth2: is less secure and more complex then the original and was not widely adopted.
  - One of the biggest criticisms of OAuth 2.0 is that the standard intentionally does not directly define or support encryption, signature, client verification or channel binding
  - Instead, OAuth expects implementers to use an outside protection protocol like Transport Layer Security (TLS)
- OAuth is not completely safe. There is a risk of Phishing, where a website will get these credentials during part of the OAuth process.
- There is no perfectly safe, universally accepted, SSO that works on all websites, but with OAuth, we’re getting closer.

## [Auth0 Docs](https://auth0.com/docs/flows)

- Authentication is different from Authorization:  If you can't prove your identity, you won't be allowed into a resource (Authentication). And even if you can prove your identity, if you are not *authorized* for that resource, you will still be denied access.
- There are several Authorization flows you can use with Auth0
  - **Authorization Code Flow**: Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow, which exchanges an Authorization Code for a token.
  - During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Use **Authorization Code Flow with Proof Key for Code Exchange (PKCE)**
  - **Implicit Flow with Form Post**: no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication
  - **Hybrid Flow**: This can be useful in situations where your application needs to immediately access information about the user, but must perform some processing before gaining access to protected resources for an extended period of time.
  - **Client Credentials Flow**: For machine-to-machine (M2M) applications
  - **Device Authorization Flow**: the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. (For TV perhaps)
  - **Resource Owner Password Flow**: It's not recommended, can be used for highly-trusted applications. You would need to re-enter passwords.

## [Auth0 for React](https://auth0.com/docs/libraries/auth0-react)

- `npm install @auth0/auth0-react`

- import Auth0Provider and wrap your App component in an Auth0Priver component.

```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import { Auth0Provider } from '@auth0/auth0-react';
import App from './App';
ReactDOM.render(
  <Auth0Provider
    domain="YOUR_DOMAIN"
    clientId="YOUR_CLIENT_ID"
    redirectUri={window.location.origin}
  >
  <App />
  </Auth0Provider>,
document.getElementById('app')
);
```

- Use `isLoading` and `error` to handle errors
- Use `loginWithRedirect` or `loginWithPopup` to log your users in.
- Use `logout` to log your users out. Make sure `returnTo` is specified in "Allowed Logout URLs" in your Auth0 Dashboard.
- Access user profile information with the `user` value: `const { user } = useAuth0();`
- Can add this to a component too in the render method.
- Protect a route component using the `withAuthenticationRequired`
- All kinds of things need to happen for an api request.... "To call a protected API with an Access Token, be sure to specify the `audience` and `scope` of your access token, either in `Auth0Provider` or `getAccessTokenSilently`. Then use it to call a protected API by passing it in the `Authorization` header of your request."
