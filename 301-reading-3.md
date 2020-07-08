## July 8<sup>th</sup>

### Javascript Templating Language and Engine
https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2

- Can render client-side view templates with js by using a JSON data source 
  - HTML markup with templating tags to insert var or run programming logic 
- Mustache is a logic-less (becuase there are only tags) template syntax

### A Complete Guide to Flexbox
https://css-tricks.com/snippets/css/a-guide-to-flexbox/
- Really good visual examples here! 

- Parent element: flex container
  - **display**
    - display: flex 
  - **flex-direction** 
    - row, row-reverse, column, column-reverse
  - **flex-wrap**
    - nowrap, wrap, wrap-reverse
  - **flex-flow**
    - shorthand for flex-direction and flex-wrap
    - default is row nowrap
    - Ex: column wrap
  - **justify-content**
    - flex-start (default), flex-end, center are best options re browser support
    - space-between, space-around, space-evenly 
    - can also use safe and unsafe
  - **align-items**
    - stretch (default), flex-start, flex-end, center, baseline
    - safe and unsafe
  - **align-content**
    - flex-start, flex-end, center, stretch, space-between, space-around
  
- Child elements: flex items
  - **order**
    - default is 0, controls order they appear in flex container
  - **flex-grow**
    - unitless number, dictates what amount of available sace inside flex container the item should take up
  - **flex-shrink**
    - defines ability for a flex item to shrink if necessary
  - **flex-basis**
    - defines default size of element before reamining space distributed
  - **flex** 
    - shorthand for flex-grow, flex-shrink, flex-basis
    - first required, other 2 optional
    - shorthand sets other values intelligently 
  - **align-self**
    - allows default alignment to be overridden for individual flex items
    - stretch, flex-start, flex-end, center, baseline

- Items laid out following *main axis* (*main-start* to *main-end*) or the cross axis (*cross-start* to *cross-end*)



