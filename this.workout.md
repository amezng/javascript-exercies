#### Global context

1. Access all the Root DOM elements present in a HTML page using the this keyword.
    For example.

    ```javascript
    console.log("Document = " + this.document)
    console.log("localstorage = " +this.localStorage)
    ```
2. Access atleast 3 properties of the window elements elements(sessionStorage,Location,caches) using this keyword.
Example :
   ```javascript
    console.log("localStorage = " + this.caches)
   ```

3. Create a function to add two numbers and call the function using this keyword
4. Create a function which takes a window object and displays the innerHeight and innerWidth. Call this function by passing the "this"
Example.

  ```javascript
   function MyFunc(){...}
   MyFunc(this)
  ```
5. Add a function "showStorageLength" as a property using prototype keyword, to the window object, (use this). This function should show the number of elements in the localStorage The function must be accessible using the this/window keyword in the global scope, as depicted below.
  ```javascript
   this.showStorageLength()
   window.showStorageLength()
  ```
6. Create a function, named "AddToWindow" which takes window object, adds a function to it(same function "showStorageLength") and returns the window. Try accessing that newly created function using window/this
Example.

  ```javascript
   function AddToWindow(this){...}
   AddToWindow(window);
   window.showStorageLength()
  ```

### Function context

1. Create a Person object using "var" keyword, with properties name,age. Create a function which takes "Person" object and doubles the age, and return the updated object.
Example
   ```javascript
      var person = {...}
      function makeHimOld(person){
        ...
        return this;
      }
  ```
2. Make the above function makeHimOld a property of Person object and then try calling using Person object reference. See the difference.
