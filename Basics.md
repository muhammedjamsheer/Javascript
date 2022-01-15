
 
### Table of Contents

| No. | Questions |
|---- | ---------
|1 | [Javascript Variables](#Javascript-Variables)|
|2 | [Project Folder Structure?](#Project-Folder-Structure)|





### Javascript Variables
* Variables are containers for storing data.
* We can declare JS variables in 3 ways var let const.

##### The general rules for constructing names for variables
* Names can contain letters, digits, underscores, and dollar signs.
* Names must begin with a letter or $ sign or _ underscore.
* Names are case sensitive (y and Y are different variables).
* Reserved words (like JavaScript keywords) cannot be used as names.
##### Let Variable
* The let keyword was introduced in ES6 (2015).
* Variables defined with let cannot be Redeclared.
 ```javascript
   let x = "John Doe";
   let x = 0;
 // SyntaxError: 'x' has already been declared
  ```


* Variables defined with let must be Declared before use.
* Variables defined with let have Block Scope.




* **[⬆ Back to Top](#table-of-contents)**

### Project Folder Structure
1. e2e - This folder is for an end to end testing purposes. It contains the configuration files related to performing the unit test of the projects.
1. node_modules - This folder contains the downloaded packages as per the configuration.
1. src - This folder contains the actual source code. It contains 3 subfolders as – 
   1. app - App folder contains the Angular project-related files like components, HTML files, etc.
   1. assets - Assets folder contains any static files like images, stylesheets, custom javascript library files.
   1. environments - Environments folder contains the environment-related files which are required during  build of the projects.
#### Different Config Files   
1. package.json-it is basically a JSON file that contains all information related to the required packages for the project.
1. angular.json – angular.json file is an Angular Application Environment based JSON file which contains all the information related to the project build and deployment. It tells the system which files need to change when we use ng build or ng serve command. 


**[⬆ Back to Top](#table-of-contents)**

