### September 27<sup>th</sup>
## Application State with Redux

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”
- Not as vulnerable to XSS attack because a cookie isn't accessible via JavaScript
  - XSS is cross-site scripting which enables attackers to inject client-side javascript into web pages viewed by others. Often used to bypass access controls.

2. Explain 3rd party cookies.
- 3rd party cookies are those that are established by domains other than the one you're on. Used mainly for tracking and online-advertising.

3. How do pixel tags work?
- Pixel tag is a tiny snippet of code that allows you to gather info about website users. Usually a small img that contains code to an external link (the pixel server). If/when user visits the destination site the code is processed by the client, the user's browser. Browser follows link, opens graphic, which is registered and noted in server's log files



## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| cookies | small files located on user's computer designed to hold data specific to client and website, so it can be accesses by either web server or client computer. allows server to deliver page tailored to user, designed to carry info from one visit to the site to the next |
| authorization | the thing received when an access token is verified  |
| access control | the practice of restricing access in specific ways to a resource based on your user status, an example being RBAC |
| conditional rendering | the go-ahead of rendering certain components that have all the behavior you need, when the specific conditions are true (can use operators like `if` and conditional operator) |
| Redux | JS library for managing application state |



## Resources
- https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6/
- https://dev.to/cotter/localstorage-vs-cookies-all-you-need-to-know-about-storing-jwt-tokens-securely-in-the-front-end-15
- https://clearcode.cc/blog/difference-between-first-party-third-party-cookies/#third-party-cookies
- https://medium.com/datadriveninvestor/cookies-vs-local-storage-2f3732c7d977