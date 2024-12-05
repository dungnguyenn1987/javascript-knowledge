# Object-oriented programming
* Create object
```
let user = { // create object
  name: "John", //define object property
  age: 30
};

user.sayHi = function() { // define object method
  alert("Hello!");
};

user.sayHi(); // Hello!
```
OR
```
let user = {
  // ...
};

// first, declare
function sayHi() {
  alert("Hello!");
}

// then add as a method
user.sayHi = sayHi;

user.sayHi(); // Hello!
```

* Method shorthand
```
let user = {
  name: "John",
  age: 30,

  sayHi() {    // OR sayHi: function() {
    alert(this.name); // "this" is the "current object"
  }

};
user.sayHi(); // John
```
* **this** keyword
In JavaScript, keyword this behaves unlike most other programming languages. It can be used in any function, even if it’s not a method of an object.
```

```

* 
# Promise
https://javascript.info/promise-basics

The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.
* `async` method returns a `Promise` to supply the value at some point in the future.
* `await` used in `async` method to stop execution until `Promise` resolved/rejected. Instead of using `.then()` to work on Promise's result, we can use `await` to wait Promise's result and work on it as async value. It alse makes scripts more sequencely and readable by not using the multiple nested `then()`
* A Promise is in one of these states:
  * pending: initial state, neither fulfilled nor rejected.
  * fulfilled: meaning that the operation was completed successfully, fulfilled with a **value**
  * rejected: meaning that the operation failed,  rejected with a reason (**error**)

![image](https://github.com/user-attachments/assets/dc472fb5-3f80-477a-a225-a6ca65bc1676)

  * 
