## Reading 14a - June 17 <sup>th</sup>

### CSS Transforms
https://learn.shayhowe.com/advanced-html-css/css-transforms/
- **transform** property followed by the value
  - 2d
    - works on x and y axis
    - can **rotate** positive or negative
    - **scale** changes appeared size of element
      - can set x, y, or both
    - **translate** push and pull element in dif directions without changing flow of doc
      - px or %, positive values down and to right, negative do opposite
    - **skew** uses degrees
    - write multiple transform properties on one line without commas
    - can change the *default transform origin*, default is center of element
    - **perspective** (vanishing point) from which to transform
  - 3d
    - x, y, z axis
    - can rotate an element around any axis
    - puzzle card flipping game can be made with this stuff!
- vendor prefixes help it work across different browsers

### CSS Transitions & Animations
https://learn.shayhowe.com/advanced-html-css/transitions-animations/

#### Transitons
- Cqn write behaviors for transitions and animations
- For a **transition** an element needs change in state
  - :hover, :active, :focus, :target
  - *transition-property*
    - says what property will be altered, separate multiple with a comma
    - not all props can be transitioned, see site for list
  - *transition-duration*
    - use s and ms
  - *transition-timing-function*
    - sets speed during duration
    - *linear*, *ease-out*, *ease-in*
  - *transition-delay*
    - sets time value for stalling transition
- Can do shorthand for these
- Card flip!!

#### Animations
- When transitions need to have multiple states
- **@keyframes** to set multiple points at which element should undergo transition, to animate
- *Animation name* identified from keyframes rule
- Duration, timing function, delay
- (see Khan Academy tutorial for this too- v helpful)

### Simple CSS Tricks to WOW Users
https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/
- Fade in
- Change color
- Grow and shrink
- Rotate elements
- Square to circle
- 3D shadow
- Swing
- Inset border

### Examples of v cool CSS

#### 6 Buttons Animated
https://codepen.io/retyui/pen/ByoaXV?__cf_chl_jschl_tk__=ebbff39319ef48d7bb75cac96a85e5ad6d0058b7-1592492747-0-ATcVMttueUmN67FwbJyXE-cQvhNHHbkED_U4Vj-SUoghlSSIcB76CAW4f_zfx1Pr6KR3FYF8FuARUTBpGo-14nlq6KZihlvR4ES3k8asSd-uQwiwwJakiI0gE_64H1Wtt7RDNPR4O7gRxpqLcfuWpQRD-_g8i6RH4s5CtLLTIhoEkke0r0X_kVvEqRuJfcfqK-xS7BaFGCZ43sLblKgJpu1_EMrPCWANttdhZneX_SsMJYudt2hdz3gd4B3nqo3u3iTPYn-ljRVckY1e3g7vrLxdDfpGyUYQmlJGg5fcPuatUoCtIaZPQ9RX5mIyxS6Qix3zzW3wZkEPGbi14V1wDV_WOZwk640lVYNggV4WxNVI

#### Keyframe Animation
https://codepen.io/akshaychauhan/pen/oAfae

#### 404
https://codepen.io/kieranfivestars/pen/MYdQxX

#### Bounce Animation
https://codepen.io/dp_lewis/pen/gCfBv
- this is tight!

[Back to Home](README.md)