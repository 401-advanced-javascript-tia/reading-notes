## July 6<sup>th</sup>

### Shay Howe's Intro to RWD
https://learn.shayhowe.com/advanced-html-css/responsive-web-design/

- *Responsive Wed Design* is industry's response to how to build websites suitable for all users (mobile usage)
- Practice of building site that works on every device
- *Responsive* reacts quickly, positively to changes
- *Adaptive* easily modified for new purpose or situation
- *Mobile* generally builds separate website solely for mobile users
- **Flexible layouts**
  - build website with flexible grid capable of dynamically resizing to any width
  - built using relative length units (% or em), then used to declare width, margin, padding
  - growing support for new CSS# units vw, vmin, vh, vmax
  - target / context = result
- **Media queries**
  - can use to specify different styles for individual browser/device circumstances (ex: width of viewport or device orientation)
    - **can use @media rule inside existing style sheet**
    - can import new style sheet using @import rule
    - can link to separate sheet from within HTML doc
    - common media types: all, screen, print, tv, braille (3d-glasses!)
    - can use *and*, *not*, *only* also to build expression
  - **Media features** identify what attributes or properties will be targeted within media query expression
    - *height* and *width* (max and min, less than or equal to and greater than or equal to)
    - *orientation* determins landscape or portrait
    - *aspect-ratio* and *device-aspect-ratio* specify width/height pixel ratio of targeted rendering area
    - *resolution* specifies resolution in pixel density- DPI (dots per inch)
    - *color*, *color-index*, *monochrome*, *grid*, *scan*
  - **Mobile first** technique builds websites for small first and then uses media queries to add styles as viewport grows
  - **viewport** meta tag identifies size, scale, resolution of website
    - can set multiple values separated by comma in the content attribute value
    - being moved to @viewport rules in CSS, instead of as meta tag in HTML
- **Flexible media**
  - images, videos, other media needs to be scalable as well as viewport size changes
  - can use CSS rule to set max-width of media to 100%, ensuring it gets smaller as page scales down
  - flexible embedded media workaround for iframes and other embedded media

### All About Floats
https://css-tricks.com/all-about-floats/

- Notes

### Don't Overthink it Grids
https://css-tricks.com/dont-overthink-it-grids/

- Notes

### CSS Floats Explained by Riding an Escalator
https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/

- Notes

### SMACSS Official Documentation
http://smacss.com/

- Notes

