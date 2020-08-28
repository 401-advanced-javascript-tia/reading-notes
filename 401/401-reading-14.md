## Aug 26<sup>th</sup>
## Bearer Authorization and Access Control (ACL)

1. When is Basic Authorization used vs. Bearer Authorization?

- Basic authorization uses the username and secret and the bearer authorization uses the token
- Security vulnerabilities with basic
- "Bearer authentication" = "give access to the bearer of this token"

2. What does the JSON Web Token package do?

- A JSON web token is a way of transmitting information in a JSON object between parties, in a secure way

3. What considerations should we make when creating and storing a SECRET?

- We want to make sure that it actually is kept secret, and we can do so by putting it into an .env file and bringing it in

### Role Based Access Control benefits
- Policy not associated with person, it's associated with role
- Can automate what resources a person has access to based on their role, not individual person
- Always execute with smallest number of access right that can pass for the thing that needs to be done at the time
  - User could start in one role and have certain access (to certain # of files, for ex) and then when they change roles they can increase access easily 

## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| encryption     | two- way process that requires a key to get back to plain text |
| token          | the "county-fair ticket" that the requestor needs to do the thing it wants to do |
| bearer         | the entity that has the token  |
| secret         | the key that the authentication header uses to sign the header and payload and send back to user            |
| JSON Web Token | way of securely transmitting information between parties as a JSON object |

## Resources
- https://www.youtube.com/watch?v=C4NP8Eon3cA
- https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html
- https://en.wikipedia.org/wiki/Role-based_access_control
- https://blog.restcase.com/4-most-used-rest-api-authentication-methods/#:~:text=The%20name%20%E2%80%9CBearer%20authentication%E2%80%9D%20can,response%20to%20a%20login%20request
- https://blog.angular-university.io/angular-jwt/