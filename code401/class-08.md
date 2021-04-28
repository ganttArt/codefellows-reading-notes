# Reading: Access Control (ACL)

## Review, Research, and Discussion

1. When is Basic Authorization used vs. Bearer Authorization?
    - Basic Auth is used to login and Bearer Auth is used to gain access to different parts of the website.
1. What does the JSON Web Token package do?
    - It allows you to create and validate JWTs.
1. What considerations should we make when creating and storing a SECRET?
    - When creating, it needs to be random enough to not be crackable. You want to store it in a place that is not going to be visible to users, so it will not be in github and it will not be stored in somewhere that you could find in dev tools. Environment variables to store secrets is the standard.

## Vocabulary Terms

- **encryption** - the method by which information is converted into secret code that hides the information's true meaning. [src](https://searchsecurity.techtarget.com/definition/encryption#:~:text=Encryption%20is%20the%20method%20by,encrypted%20data%20is%20called%20ciphertext.)
- **token** - a peripheral device used to gain access to an electronically restricted resource. The token is used in addition to or in place of a password. [src](https://en.wikipedia.org/wiki/Security_token)
- **bearer** - an HTTP authentication scheme that involves security tokens called bearer tokens. [src](https://swagger.io/docs/specification/authentication/bearer-authentication/)
- **secret** -  the piece of information or parameter that is used to encrypt and decrypt messages in a symmetric, or secret-key, encryption. [src](https://www.techopedia.com/definition/24865/secret-key)
- **JSON Web Token** - an open, industry standard RFC 7519 method for representing claims securely between two parties. [src](https://jwt.io/)

## Preview

- [RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)
- [5 steps to RBAC](https://www.csoonline.com/article/3060780/security/5-steps-to-simple-role-based-access-control.html)
- [wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

1. Which 3 things had you heard about previously and now have better clarity on?
    - RBAC is Role Based Access Control. Users with certain roles are going to have access/rights to see/do different things.
    - Employees in a role will have access to a limited number of files. And they would have to switch roles to gain access to other files.
    - RBAC is one a few options to monitor access, others include ACL and ABAC.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - How do we monitor and change the user permissions as an admin?
    - How can we make an admin panel in Node. Are there any prebuilt solutions?
    - Mandatory access control vs discretionary access control.
1. What are you most excited about trying to implement or see how it works?
    - Seeing the difference of implementation between RBAC and ACL (Access control lists) in JS.
