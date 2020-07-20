## July 19<sup>th</sup>

### EJS - Embedded JavaScript Templating
https://ejs.co/
- Body parser library extracts body of request
- Path is built in library of node, dont need to install, just require it
- Making variable available inside specific ejs view
- `<%= variable %>`
  - Can use ejs snippet for syntax (no = sign)
- Index.ejs acts as template
- Can iterate over loops in .ejs
- Use if/else statements to evaluate the data and render
- Large communicate active users, library is maintained
- We've been working with Express in the back end and linking it up to a front end thats already built out, EJS is a way for us to also work the front end with Express

### Templating with EJS
https://scotch.io/tutorials/use-ejs-to-template-your-node-application
- *"Turing-complete"* = comutationally universal
- Installation instructions, options, tags, CLI commands
- Can use custom delinters (although... why? seems confusing)
- GitHub with source code here: https://github.com/scotch-io/node-ejs

**Google Books APIs**
https://developers.google.com/books/docs/v1/using#WorkingVolumes
- Only required parameter is **q**, heaps of optional ones listed here
- 