## Reading 03 - June 2<sup>nd</sup>

#### Notes from during class 02:

*A variable by itself is an implicit conditional in anything checking for true or false. Becuase it exists, the condition is true.*

*0, null, NaN, undefined, '', are the things that evaluate as false in this kind of check (falsey)*

## **Duckett HTML**

### Ch 3 - Lists
- *Ordered lists* where each list item is numbered
- *Unordered lists* where each list item begins with a bullet point
- *Definition list* made up of terms and definitons for those terms
  - \<dl> 
    - \<dt>Tia\</dt>
      - \<dd>A human person.\</dd>
- Can nest lists as well 
  - \<ul>
    - \<li>
    - \<li>
      - \<ul>
        - \<li>
        - \<li>

### Ch 13 - Boxes (CSS)
- Set box dimensions with width and height
  - Pixels ( height : 300px )
  - Percentage (relative to size of browser window)
- Can limit (min and max) width and height since some pages expand/shrink to fit users device
  - min-width: 200px   
- *Overflow* property what to do if content in box is larger than box itself
  - overflow : hidden
  - overflow : scroll
- *Border* separates margin from padding
- *Margin* is outside border
- *Padding* is in between border and content within it
- **If you specify a width for a box, the borders, margin, and padding are added to its width and height.**
- *White space* is the space between items on the page
- (Can also use these for each side) border-width , border-style , border-color 
  - can shorthand on one line (border : 3px dotted #0088dd)
  - shorthand for sides too, clockwise order, top right bottom left (padding : 10px 5px 3px 2px)
- Can set *margins* to center box (need to set width for box first, otherwise it'd take up full page)
  - *auto* puts equal gaps on each side
- *Display* property changes inline/block. Other options:
  - inline-block (causes block level element to flow like inline)
  - none (hides element from page)
- *Visibility* property can hide box from user but leaves space
  - visibility : hidden (would hide element but leave space where it was)
<br></br>
- CSS3 *border-image* **need to look this up for more deets!**
  - *box-shadow*
  - *border-radius*

## **Duckett JS**

### Ch 4 - Decisions and Loops (from *switch statements*)
- *Switch statements* compare value against possible outcomes
  - Variable called *switch value* 
  - Within code block, each case has value for variable and what code to run if so
- *Truthy* and *falsey* values aer treated *as if* they are true/false
- **Loops**
  - *for*
    - used if you need to run the code for specific number times
    - *initialization*, *condition*, *update*
  - *while*
    - if you don't know how many times code should run
    - will continue to run as long as condition is *true*
  - *do while*
    - similar to while, but will always run *even if* condition evaluates to false

TRUTHY

FALSEY
0
null
undefined
NaN
' '

&& and || combine the values and become last valid value or fir invalid (falsey) value

&&
- short circuits on the first falsey thing

||
- short circuits on the first truthy that it finds

!
- flipper, makes anything falsey become true and another true become false
  - !0 becomes true (becuase 0 is falsey)
  - !10 becomes false (because 10 is a true thing and not flips it)

LOOK AT NOTES FROM DAY 3

[Back to Home](README.md)