## Reading 13 - June 16<sup>th</sup>

### Past, Present and Future for Local Storage of Web Apps
#### http://diveinto.html5doctor.com/storage.html

- Goals are:
  - lots of storage space
  - on the client
  - persists beyond page refresh
  - isnt transmitted to server
- Historical solutions were browser-specific or reliant on 3rd party plugins
- HTML5 wanted to provide standardized API, implemented consistenly in all browsers, not relying on 3rd party plugins

#### HTML5 Storage
- HTML5 Storage = Local Storage = DOM Storage
- Way for web pages to store named key/value pairs locally within web browser
- From JS, accessed through localStorage object on global window object

#### Using HTML5 Storage
- Store data based on named key (string), retrieve that data with same key
- Use parseINT and parseFloat if storing anything other than strings
- setItem() and getItem(), removeItem(), clear() and getter
- Can track storage area changes by trapping the storage event
- Storage event is not cancellable, simply a way for browser to tell this "this happened"
- Storage quota for each origin is 5MB, QUOTA_EXCEEDED_ERR is what you'll see if you try go past it

#### Another vision for advanced local storage
- Indexed Database API (formerly WebSimpleDB), known as IndexedDB
  - is this implemented yet? time of writing was 2011!

## CLASS NOTES

- we will store things in local storage
- local storage is unique to your machine
- local storage is unique to your browser
- its a secure way for the browser to store info on your harddrive
- other websites cant access each others local storage

#### has two methods
- getter and setter
  - these are functions that save and retrieve data
- setItem() takes two arguments
  - the key (or variable name), and the value

#### Steps for storage of an object
1. stringify the object (the right way) with JSON.stringify()
2. store the stringy object in local storage with localStorage.setItem

3. a) get item from local storage with localStorage.getItem()
3. b) unStringify the object, hydrate the dehydrated object with JSON.parse()

- representation of the object in readable format (in "dehydrated" form, it doesnt actually behave like an object), its possible to change it back to object version (reconstituting)

[Back to Home](README.md)