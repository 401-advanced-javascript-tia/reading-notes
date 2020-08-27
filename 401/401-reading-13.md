## Aug 25<sup>th</sup>
## OAuth cont.

1. Write the following steps in the correct order:

- Register your application to get a client_id and client_secret
- Ask the client if they want to sign in via a third party
- Make a request to the access token endpoint
- Receive access token
- Make a request to a third-party API endpoint
- Redirect to a third party authentication endpoint
- Receive authorization code

2. What can you do with an authorization code?

With the authorization code the application/client can make a request to the access token endpoint.

3. What can you do with an access token?

With an access token you can make the request to the third-party API endpoint in order to get the protected resource.
- Exchange information between two bodies
- Self contained with information about the user
- Avoid querying the db more than once, you just pass the token each time and jwt system verifies it

4. What’s a benefit of using OAuth instead of your own basic authentication?

If you're using OAuth you don't have to store the user's unique information in a database somewhere. 


## Vocabulary

|   **Term**    | **Definition**  |
| ------------- | ----------- |
| Client ID     | Used to authenticate with the authorization server. Should be kept secret if possible, but not as important as client secret.             |
| Client Secret | Password. Also used to authenticate with the authorization server. Keep this very secret in a .env file   |
| Authentication Endpoint | used to interact with the resource owner and get the authorization it needs  |
| Access Token Endpoint | used by the application to make a request for an access token  |
| API Endpoint | where the request is make for the authorization code |
| Authorization Code | the client exchanges this for the access token  |
| Access Token | the token given to grant client access to the API endpoint on behalf of the user             |

## Resources
- https://www.digitalocean.com/community/tutorials/an-introduction-to-oauth-2

