## Aug 20<sup>th</sup>
## Stacks and Queues

### What is Stack? FILO/LIFO
***
- A stack is.... a *stack*!
  - An *idea*, not an *implementation*
- **F**irst **I**n **L**ast **O**ut / **L**ast **I**n **F**irst **O**ut
- pop() and push()
  - O(1)
  - push onto and pop off of the stack
- peek()   
  - O(1)
  - inspect the top most thing in the stack
  - with a vanilla stack, you don't know the height of the stack and what is below
- isEmpty()  
  - O(1)
- **These are the only things you can do to a stack, even if it's in array form (for ex)**
  - Huge value in keeping it as a 'stack' 


### What is Queue? FIFO/LILO
***
- Instead of top and bottom, there's a notion of front and back
  - *enqueue*: adds to front of queue
  - *dequeue*: takes off back of queue
  - can also *peek* and check *isEmpty*