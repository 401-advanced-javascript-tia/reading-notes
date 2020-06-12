## Reading 09 - June 9<sup>th</sup>

## **Duckett HTML**

### Ch 7 - Forms (p 144-175)
- Forms use (surprise) a \<form\> element
- Info from form sent in (surprise) key value pairs
- *Form controls* have names and the values are sent to the server
  - To add text, text area
  - To make choice
  - Submit form
  - Upload file
- Can group form elements
- New in HTML5
  - form validation
  - date input
  - email or url input
  - search input

### Ch 14 - Lists, Tables, Forms (p 330-357)
- Many CSS properties specifically used for lists, tables, forms
- **Lists**
  - list-style-type
    - bullet point styles
    - list-style-image
    - list-style-position
  - list-style is *shorthand* for these
- **Tables**
  - Properties to control borders and spacing, make more consistent across different browsers
    - gaps between cells
    - border on empty cells
- **Forms**
  - Vertically align form controls using CSS
  - Styling to make more interactive
  - Align form controls

## **Duckett JS**

### Ch 6 - Events (p 243-292)
*"Hey, this just happened!*
- *Binding* is process of stating which event you are waiting to happen, which element waiting for that even to happen upon
- Event occurs on element, triggers JavaScript function
- *Event delegation*
  - Monitor for events that happen on all children of an element

#### Notes from class


1. you need a target
2. you need to add an event listener to that target
  - 2a. listener need a type of event to listen to
  - 2b. need a function that the listener can call whenever the event happens

- an Event object will be passed into the callback function, if you define a parameter (potato) for it, you can use it

- function names for things that handle events start with handle
  - function handleMouseOverDiv
#### Book has page for heaps of event types

#### Form Submits
1. you need a target
2. you need to add an event listener to that target
  - 2a. listener need a type of event to listen to
  - 2b. need a function that the listener can call whenever the event happens
3. **prevent the default behavior of the submit, which is the page refresh- requires an event parameter**
  - potatoEvent.preventDefault();
  - THIS SHOULD BE THE FIRST LINE OF EVERY FORM SUBMIT, FOR NOW
  - to prevents the page refresh when you press enter, which is something specific to forms

##### Important Things to Keep in Mind
  1. Figure out how to get data out of forms
  2. If you have data, can you pass it through a contructor?


[Back to Home](README.md)