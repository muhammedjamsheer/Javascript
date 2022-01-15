
 
### Table of Contents

| No. | Questions |
|---- | ---------
|1 | [What is Angular Framework?](#what-is-angular-framework)|
|2 | [Why we use Angular ?](#why-we-use-angular )|
|3 | [Bootstrapping in Angular](#Bootstrapping-in-Angular )|
|3 | [Angular Decorators](#Angular-Decorators )|
|4 | [Angular Components](#Angular-Components )|
|5 | [Data Bindings in Angular](#Data-Bindings-in-Angular )|
|6 | [Angular Component Cammunication](#Angular-Component-Cammunication)|
|7 | [Angular Directives](#Angular-Directives )|
|8 | [Angular Pipes](#Angular-Pipes)|
|9 | [Component Life Cycle Hook](#Component-Life-Cycle-Hook)|
|10| [Content Projection In Angular](#Content-Projection-In-Angular)|





### Advantages of Using Angular
* Supports two-way data binding.
* Supports validations and template syntax (both angular and static).
* We can add custom animations, directives, and services.
* Hierarchical Dependency Injection structure (Parent-child).
* Provision to facilitate RESTful services and client-server communication.
* Lazy Loading: Lazy loading is based on the concepts of Angular Routing and it helps bring down the size of large files by lazily loading the data that are required.

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

