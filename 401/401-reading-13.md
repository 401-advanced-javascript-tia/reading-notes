## Aug 25<sup>th</sup>
## Bearer Authorization

1. Write the following steps in the correct order:

Register your application to get a client_id and client_secret
Make a request to a third-party API endpoint
Ask the client if they want to sign in via a third party


Receive access token
Make a request to the access token endpoint
Redirect to a third party authentication endpoint


Receive authorization code



2. What can you do with an authorization code?

3. What can you do with an access token?
- Exchange information between two bodies
- Self contained with information about the user
- Avoid querying the db more than once, you just pass the token each time and jwt system verifies it

4. What’s a benefit of using OAuth instead of your own basic authentication?


|   **Term**    | **Definition**  |
| ------------- | ----------- |
| Client ID     | Should be kept secret if possible, but not as important as client secret.             |
| Client Secret | Keep this very secret in a .env file            |
| Authentication Endpoint |             |
| Access Token Endpoint |             |
| API Endpoint |             |
| Authorization Code |             |
| Access Token |             |
