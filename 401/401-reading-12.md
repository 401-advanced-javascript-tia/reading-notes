## Aug 24<sup>th</sup>
## OAuth

- OAuth: When you log into a website using another websites login credentials

1. Why is authentication important?
- Authentication is super important because it's the way we can identify unique users and keep their unique, sensitive data secure. 

2. Why should we be careful about storing a user’s password?
- We should be careful about storing a user's password because as the developer, it's our responsiblity to make sure it's kept secure. 

3. What is the difference between hashing and encryption?
- Encryption is a two-way function in that something can be decrypted with the use of the key, whereas hashing is one-way. With a good process there's no way to reverse the hashing to get to the original text. 

4. What is the difference between encryption and encoding?
- Encoding is a process that reverses the algorith that encoded the thing in the first place, whereas encryption requires the use of a key to get it back to plain text.

5. What is a token used for?
- The token acts like a ticket to the fair, you need it to get through and do what you want to do.


|   **Term**    | **Definition**  |
| ------------- | ----------- |
| authentication| when an entity proves an identity. process of verifying the identify of a User  |
| authorization | when an entity proves a right to access. OAuth is meant for authorization between services  |
| encryption    | two-way function that requires a key |
| hashing       | one-way process to create a hash from plain text  |
| session       | a temporary exchange between communicating devices  |
| cookie        | a piece of information that is transferred via header  |
| token         | the ticket to do the thing it wants to do! |
| Basic Auth    | process of encoding username and password using base64 |
| encoding      | reverses the algorithm that encoded, to get back to plain text|
| secret        | the thing that is used to create the token through jwt |
| cryptography  | the science of protecting data  |

### Resources
- https://www.youtube .com/watch?v=t4-416mg6iU
- https://aaronparecki.com/oauth-2-simplified/
- https://developer.okta.com/blog/2018/08/21/build-secure-rest-api-with-node
