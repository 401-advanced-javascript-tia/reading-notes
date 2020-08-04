## July 7<sup>th</sup>

### JavaScript & jQuery, pg 293-301, 306-331, 354-357

- jQuery: simple way to do JavaScript
  - "Write less, do more"
- Add as script to HTML page
- Function lets you find element in page and then creates an object
- Does something with that element using jQuery methods
  - $('li.hot').addClass('complete');
- It's cross-browser compatible!
  - Uses *feature detection* to find best way to accomplish task
- **(See physical notes from pre-work jQuery assignment for various jQuery methods)**
- jQuery selection is created, stores reference to corresponding nodes in DOM tree
- Store reference to jQuery object in variable
  - these variable names often start with $
- *Implicit iteration* is ability to update all elements in jQuery selection
- Can *chain* multiple methods to selection
- .ready() method checks that page is ready to work with
  - can still use this eveb if script tag is at bottom of html
- Can use CDN to access jQuery, should incluce fallback version
- Always include script tags at end of HTML


### 6 Reasons for Pair Programming
https://www.codefellows.org/blog/6-reasons-for-pair-programming/

1. **Greater efficiency**
- Might take longer up-front, but more efficient in long run

2. **Engaged collaboration**
- Less time spent messing around when working with someone else
- Boosts confidence to rely on each other and not need TAs as much

3. **Learning from fellow students**
- Exposure to different techniques
- Utilizing each others strengths with added benefit of solidifying learning by teaching

4. **Social skills**
- Communication is key!
- Has major long term career impacts

5. **Job interview readiness**
- Common interview step is pair programming 

6. **Work environment readiness**
- This is real life, important to practice and gain comfort with it now


### jQuery notes from lecture on Tues

- can add data-anything="whatever-you-want" to any tag
  - like an id but with different syntax, distinguishes between developer and designer (designers use id, and they leave data- alone when they see it because they know its a developer thing)
