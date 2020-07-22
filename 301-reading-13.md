## July 22<sup>nd</sup>

### HTML5 Forms

https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data
- Form submitted, client (browser) sends request to server using HTTP protocol
- Most important attributes are **action** and **method**
  - *Action* defines where data is being sent
  - If none selected, data is sent to same pg form is on
  - *Method* defines how data is sent  
  - Can be sent with GET and POST, need library for POST
  - Data appended to URL as name/value pairs
- Server receives string that needs to be parsed to get data as key/value pairs
- Extra steps if you want to send files
- **Security** issues
  - HTML forms most common places where attacks occur
    - Comes from how server handles them
  - *Never trust your users!*
  - All data that comes to server must be checked and sanitized
    - Escape potentially dangerous characters
    - Limit amount of incoming data to only what's necessary
    - Sandbox uploaded files

Great reference on elements of forms:
https://htmlreference.io/forms/
