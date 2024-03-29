
 
### Table of Contents

| No. | Questions |
|---- | ---------
|1 | [Javascript Variables](#Javascript-Variables)|
|2 | [Javascript Data Types](#Javascript-Data-Types)|
|3 | [String Methods](#String-Methods)|
|4 | [Number Methods](#Number-Methods)|
|5 | [Array Methods](#Array-Methods)|
|6 | [Arithmetic Operators](#Arithmetic-Operators)|
|7 | [Assignment Operators](#Assignment-Operators)|
|8 | [Comparison Operators](#Comparison-Operators)|
|9 | [Logical Operators](#Logical-Operators)|





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
 
**[⬆ Back to Top](#table-of-contents)**

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
#### 6. Extracting String Parts
There are 3 methods for extracting a part of a string
* slice(start, end)
* substring(start, end)
* substr(start, length)

##### 1.JavaScript String slice()
slice() extracts a part of a string and returns the extracted part in a new string.     
The method takes 2 parameters: the start position, and the end position (end not included).
 ```javascript
let str = "Apple,Banana,Kiwi";
let part = str.slice(6, 12);
// output  Banana
 ``` 
 If a parameter is negative, the position is counted from the end of the string.
  ```javascript
let str = "Apple,Banana,Kiwi";
let part = str.slice(-11, -5);
// output  Banana
 ```
 If you omit the second parameter, the method will slice out the rest of the string:
  ```javascript
let str = "Apple,Banana,Kiwi";
let part = str.slice(13);
// output  Kiwi
let part = str.slice(-4);
// output  Kiwi
 ```
 
 #### 7. Extracting String Characters

##### 1.charAt(position)
The charAt() method returns the character at a specified index (position) in a string:  
  ```javascript
let text = "HELLO WORLD";
let char = text.charAt(0)
// output  H
 ```
##### 2.Property Access
  ```javascript
let text = "HELLO WORLD";
let char = text[0];
// output  H
 ```
 #### 8. Converting a String to an Array
 A string can be converted to an array with the `split()` method:

 ```javascript
text.split(",")    // Split on commas
text.split(" ")    // Split on spaces
text.split("|")    // Split on pipe
 ```
 
If the separator is omitted, the returned array will contain the whole string in index [0].    
If the separator is "", the returned array will be an array of single characters:

 #### 9.JavaScript Search Methods
* String indexOf()
* String lastIndexOf()
* String search()
* String match()
* String includes()
* String startsWith()
* String endsWith()

##### 1. indexOf()
The `indexOf()` method returns the index of (the position of) the first occurrence of a specified text in a string:

 ```javascript
let str = "Please locate where 'locate' occurs!";
str.indexOf("locate");
//output  7
 ```
 
 ##### 2. lastIndexOf()
The `lastIndexOf()` method returns the index of the last occurrence of a specified text in a string:

 ```javascript
let str = "Please locate where 'locate' occurs!";
str.lastIndexOf("locate");
//output  21
 ```
`Both indexOf(), and lastIndexOf() return -1 if the text is not found`

 ##### 3. search()
The `search()` method searches a string for a specified value and returns the position of the match:

 ```javascript
let str = "Please locate where 'locate' occurs!";
str.search("locate");
//output  7
 ```
 
  ##### 4. includes()
The `includes()` method returns true if a string contains a specified value.

 ```javascript
let text = "Hello world, welcome to the universe.";
text.includes("world");
//output  true
 ```
 ##### 5. startsWith()
The `startsWith()`  method returns true if a string begins with a specified value, otherwise false:

 ```javascript
let text = "Hello world, welcome to the universe.";
text.startsWith("Hello");
//output  true
 ```
##### 6. endsWith()
The `endsWith()`  method returns true if a string ends with a specified value, otherwise false:

 ```javascript
var text = "John Doe";
text.endsWith("Doe");
//output  true
 ```

**[⬆ Back to Top](#table-of-contents)**

 ### Number Methods
 ##### Adding Numbers and Strings
  ```javascript
let x = 10;    let y = 20;     let z = x + y;    //output  30
let x = "10";  let y = "20";   let z = x + y;    //output  1020
let x = 10;    let y = "20";   let z = x + y;    //output  1020
let x = "10";  let y = 20;     let z = x + y;    //output  1020
let x = 10;    let y = 20;     let z = "30";    let result = x + y + z;  //output  3030
let x = "100"; let y = "10";   let z = x / y;    //output  10
let x = "100"; let y = "10";   let z = x * y;    //output  1000
let x = "100"; let y = "10";   let z = x - y;    //output  90
 ```
 
  ##### The toString() Method
  The `toString()` method returns a number as a string.
 ```javascript
let x = 123 ;  x.toString()      //output  123
 ```
 
   ##### The toFixed() Method
  The `toFixed()` method returns a string, with the number written with a specified number of decimals:
 ```javascript
let x = 9.656;
x.toFixed(0);  //output  10
x.toFixed(2);  //output  9.66
x.toFixed(4);  //output  9.6560
x.toFixed(6);  //output  9.656000
 ```
 
 ##### Converting Variables to Numbers
 There are 3 JavaScript methods that can be used to convert variables to numbers:

* The Number() method
* The parseInt() method
* The parseFloat() method

 ###### The Number() Method
 `Number()` can be used to convert JavaScript variables to numbers:
 
  ```javascript
Number(true);     //output  1
Number(false);   //output  0
Number("10");    //output  10
Number("  10")   //output  10
Number("10  ")   //output  10
Number(" 10  ")  //output  10
Number("10.33")  //output  10.33
Number("10,33")  //output  NaN
Number("10 33")  //output  NaN
Number("John");  //output  NaN
 ```
 
  ###### The parseInt() Method
 `parseInt()` parses a string and returns a whole number. Spaces are allowed. Only the first number is returned:
 
  ```javascript
parseInt("-10");            //output  -10
parseInt("-10.33");         //output  -10
parseInt("10");             //output  10
parseInt("10.33");          //output  10
parseInt("10 20 30");       //output  10
parseInt("10 years");       //output  10
parseInt("years 10");       //output  NaN
 ```
 
   ###### The parseFloat() Method
 `parseFloat()`  parses a string and returns a number. Spaces are allowed. Only the first number is returned:
 
  ```javascript
parseFloat("10");         //output  10
parseFloat("10.33");      //output  10.33
parseFloat("10 20 30");   //output  10
parseFloat("10 years");   //output  10
parseFloat("years 10");   //output  NaN
 ```
  
 **[⬆ Back to Top](#table-of-contents)**
 
  ### Arithmetic-Operators
  
| Operator. | Description |
|----| ---------
|  + |  Addition    |
|  - | 	Subtraction |
|  * |  Multiplication    |
|  / | 	Division |
| ** |  Exponentiation (Power)     |
|  % | 	Modulus (Remainder) |
| ++ |  Increment     |
| -- |  Decrement |

  ```javascript
Addition        let x = 100 + 50;     //output  150
Subtraction     let x = 100 - 50;     //output  50
Multiplication  let x = 10 * 5;       //output  50
Division        let x = 10 / 5;       //output  50
Exponentiation  let x = 10 ** 2;      //output  100   let x = 10 ** 3;     //output  1000
Modulus         let x = 10 % 3;       //output  1
Increment       let x = 100++;        //output  101   
Decrement       let x = 100--;        //output  99
 ``` 

  **[⬆ Back to Top](#table-of-contents)**
  
  
###  Assignment-Operators
Assignment operators assign values to JavaScript variables
  
| Operator. | Example |  Same As | 
|----| -------------------|--------------|
| =  |  x=y     |    	x = y     |
| += |  x+=y    |    	x = x+ y  |
| -= |  x-=y    |    	x = x- y  |
| *= |  x*=y    |    	x = x* y  |
| /= |  x/=y    |    	x = x/ y  |

  ```javascript
Addition and assign       let x = 10; x += 5;     //console.log(x)  -> 15
Substract and assign      let x = 10; x -= 5;     //console.log(x)  -> 5
Multiply and assign       let x = 10; x *= 5;     //console.log(x)  -> 50
Division and assign       let x = 10; x /= 5;     //console.log(x)  -> 2
 ```
 
    
  ### Comparison-Operators
  Comparison operators are used in logical statements to determine equality or difference between variables or values.      
  let x=5;  
| Operator. | Description   |  	Comparing   |  Return   |
|----      | ---------------     |-------------- |-----------|
| ==       |  equal to                     |  x == 8    |  false  |
|          |                               |    x == 8    |  true    |
|          |                               |    x == "5"  |  true    |
|  ===     |  equal value and equal type   |   x === 5   |  true    |
|          |                               |    x === "5" |  false    |
|  !=      |  	not equal                   |    x != 4    |  true    |
| !==      |  not equal value or not equal type|  	x !== 5   |  false    |
|          |                                 |  	x !== "5"   |  false    |
|          |                                 |  	x !== 8   |  true    |
|>         |  greater than                   |  x > 8    |  false  |
| <       |  	less than                      |  x > 8    |  true  |
| >=      |  	greater than or equal to       |  x >= 8   |  false  |
| <=      |  less than or equal to           |  x <= 8    |  true  |

  ### Logical-Operators
  Logical operators are used to determine the logic between variables or values.
 * &&   logical and       ->   it returns true when all the conditions are true
 * || 	 logical or        ->   it return true when any of the conditions are true
 * !    logical not       ->   it returns the opposite of the result
  
```javascript

```  
