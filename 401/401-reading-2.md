## Aug 10<sup>th</sup>
## Classes, Inheritance, Functional Programming

### 1. Name 3 advantages to Test Driven Development

- Focus: TDD can helps narrow your focus and will naturally force you to think in smaller chunks, thus increasing productivity.
- Safer Refactoring: once you write basic solution code that gets a test passing, you know you're safe to refactor from there
- Less Time Debugging: when you are practicing TDD and spending the time upfront to write more tests, you're reducing the overall time spent in the future fixing bugs 

### 2. In what case would you need to use ```beforeEach()``` or ```afterEach()``` in a test suite?

- You can use these to do repetitive work needed for several tests. 

### 3. What is one downside of Test Driven Development?

- One thing potentially seen as a downside is the upfront time is takes to write tests while working with the discipline of TDD. 

### 4. What's the primary difference between ES6 Classes and Constructor/Prototype Classes?

- "A class defines a type which can be instatiated at runtime, wheras a prototype is itself an object instance"
- https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up


### 5. Name a use case for a static method? 

- Static methods belong to the class instead of an instance of the class (instance not required to call the static method). You would use it when you want to implement functions that belong to a class but not to a specific object of it.


### 6. Write an example of a Higher Order function and describe the use case it solves. 

```function numberPlusOne(num) {```
  ```return num + 1;```
```}```

```const numArr = [1, 2, 3, 4];```

```const increasedNums = numArr.forEach(numberPlusOne);```

- this declares an array of numbers and then goes through that array, calling the function numberPlusOne on each item in the array, thus adding 1 to each


### Vocabulary

| **Term**      | **Definition** |
| ------------- | -------------- |
| **functional programming** | a way of programming that breaks down complex problems into smaller pieces and avoids state-changing and mutable data       |
| **pure function** | *referential transparency*: function alwways gives same return value for same arguments, cannot depend on any mutable state. *Side-effect free*: cannot cause any side effects like reassigning a variable, writing to console, modifying mutable object.       |
| **higher-order function**  | function that takes one or more functions as arguments and returns a functoin as its result    |
| **immutable state**  | the state of an object after creation where it cannot be changed or modified      |
| **object** | collection of properties that consist of key value pairs, when property value is a function it's called a method  |
| **object-oriented programming (OOP)** | model that organizes software design around objects and focuses on that data rather than functions and logic     |
| **class**  | template for creating an object   |
| **prototype**  |special property of a function, a way for an object to inherit properties and methods     |
| **```super```** | used to access properties and methods on an object's parent    |
| **inheritance**  | there are different ways of inheritance, its how a child objects get properties from a parent object   |
| **constructor** | function that creates an instance of an object   |
| **instance** | one iteration of an object created with key 'new' from constructor function   |
| **context**  | refers to the object to which a function belongs    |
| **```this```**  | points to the inheriting object when an inherited function is executed   |
| **Test Driven Development (TDD)** | the discipline of writing a test for something before writing any actual solution code   |
| **Jest** | package via npm that allows you to run tests   |
| **Continuous Integration (CI)** | development practice that involves sharing code into a shared repo and testing from there before changes are committed    |
| **unit test** | test that checks again one individual unit of code which is usually something like just one function   |


#### Rescouces

- https://www.madetech.com/blog/9-benefits-of-test-driven-development
- https://jestjs.io/docs/en/setup-teardown
- https://opensource.com/article/17/6/functional-javascript
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain
- https://blog.kevinchisholm.com/javascript/difference-between-scope-and-context/
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes
- https://javascript.info/static-properties-methods
- 
