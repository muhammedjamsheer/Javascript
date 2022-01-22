
 
### Table of Contents

| No. | Questions |
|---- | ---------
|1 | [Javascript Variables](#Javascript-Variables)|
|2 | [Javascript Data Types](#Javascript-Data-Types)|
|3 | [String Methods](#String-Methods)|





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
#### 1.JavaScript Strings
Strings are written with quotes. You can use single or double quotes:
 ```javascript
let carName1 = "Volvo XC60";   // Using double quotes
let carName2 = 'Volvo XC60';   // Using single quotes
  ```
#### 2.JavaScript Numbers
Numbers can be written with, or without decimals:
 ```javascript
let x1 = 34.00;     // Written with decimals
let x2 = 34;        // Written without decimals
  ```
  
#### 3.JavaScript Boolean
Booleans can only have two values: true or false.

#### 4.JavaScript Arrays
JavaScript arrays are written with square brackets.
Array items are separated by commas.
 ```javascript
const cars = ["Saab", "Volvo", "BMW"];
  ```
  
#### 4.JavaScript Objects
JavaScript objects are written with curly braces {}.
Object properties are written as name:value pairs, separated by commas.
 ```javascript
const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
  ```
  
#### The typeof Operator
JavaScript typeof operator to find the type of a JavaScript variable.
 ```javascript
typeof ""             // Returns "string"
typeof "John"         // Returns "string"
typeof "John Doe"     // Returns "string"

typeof 0              // Returns "number"
typeof 314            // Returns "number"
typeof 3.14           // Returns "number"
typeof (3)            // Returns "number"
typeof (3 + 4)   
  ```
  
#### Undefined
In JavaScript, a variable without a value, has the value undefined. The type is also undefined.
 ```javascript
 let car;    // Value is undefined, type is undefined
  ```
Any variable can be emptied, by setting the value to undefined. The type will also be undefined.
 ```javascript
car = undefined;    // Value is undefined, type is undefined
 ``` 
 ### String Methods
 #### 1.String Length
 To find the length of a string, use the built-in length property:
 ```javascript
let text = "Apple";
let length = text.length;

// output 5
 ``` 
  #### 2.Converting to Upper and Lower Case
A string is converted to upper case with `toUpperCase()`:      
A string is converted to lower case with `toLowerCase()`:
 ```javascript
let fruit = "Apple";
let result = fruit.toUpperCase();
// output APPLE
let result = fruit.toLowerCase();
// output apple
 ```

  #### 3.JavaScript String concat()
`concat()` joins two or more strings:
 ```javascript
let text1 = "Hello";
let text2 = "World";
let text3 = text1.concat(" ", text2);
// output Hello World
 ``` 
 #### 4. JavaScript String trim()
The `trim()` method removes whitespace from both sides of a string:
 ```javascript
let text1 = "      Hello World!      ";
let text2 = text1.trim();
// output  Hello World!
 ``` 
 
 #### 5. Replacing String Content
The `replace()` method replaces a specified value with another value in a string
 ```javascript
let text = "Please visit Microsoft!";
let newText = text.replace("Microsoft", "W3Schools");
// output  Please visit W3Schools
 ``` 

 



**[⬆ Back to Top](#table-of-contents)**

