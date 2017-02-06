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
5. Add a function "showStorageLength" as a property to the window object, using this keyword. This function should show the number of elements in the localStorage The function must be accessible using the this keyword in the global scope, as depicted below.
```javascript
  this.showStorageLength()
```
