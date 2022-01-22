
 
### Table of Contents

| No. | Questions |
|---- | ---------
|1 | [Javascript Variables](#Javascript-Variables)|
|2 | [Javascript Data Types](#Javascript-Data-Types)|





### Javascript Variables
* Variables are containers for storing data.
* We can declare JS variables in 3 ways var let const.

##### The general rules for constructing names for variables
* Names can contain letters, digits, underscores, and dollar signs.
* Names must begin with a letter or $ sign or _ underscore.
* Names are case sensitive (y and Y are different variables).
* Reserved words (like JavaScript keywords) cannot be used as names.

A variable declared without a value will have the value undefined.
```javascript
  var name;   //undefined
```

If you re-declare a JavaScript variable declared with var, it will not lose its value.
 ```javascript
 var carName = "Volvo";
 var carName;
 // Volvo
  ```
##### Var Variable
* The var is the oldest keyword to declare a variable in JavaScript. . 
* Variables defined with let have Block Scope. 
* Variables declared inside a { } block cannot be accessed from outside the block:

##### Let Variable
* The let keyword was introduced in ES6 (2015).
* Variables defined with let must be Declared before use. 
* Variables defined with let have Block Scope. 
* Variables declared inside a { } block cannot be accessed from outside the block:
 ```javascript
 {
   let x = 2;
 }
 // x can NOT be used here
 ```

* Variables defined with let cannot be Redeclared.
 ```javascript
  let x = "John Doe";
  let x = 0;
  // SyntaxError: 'x' has already been declared
  ```
  ###### Const Variable
  * The const keyword was introduced in ES6 (2015).
  * Variables defined with const cannot be Redeclared.
  * Variables defined with const have Block Scope.
  * Variables defined with const cannot be Reassigned.

 ```javascript
  const PI = 3.141592653589793;
  PI = 3.14;      // This will give an error
  PI = PI + 10;   // This will also give an error
  ```



   




* **[⬆ Back to Top](#table-of-contents)**

### Javascript Data Types 
JavaScript variables can hold different data types:  string, number, boolean,object and more:


**[⬆ Back to Top](#table-of-contents)**

