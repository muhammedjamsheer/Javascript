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



1.### what is angular framework? 

* Angular is basically is an open-source, JavaScript-based client-side framework that helps us to develop a web-based application
* Angular is one of the best frameworks for developing any Single Page Application

2.### why we use angular?
* Angular is supported by google (saftey and updated)
* Typescript used in angular is a product of microsoft. So both are  open source and freely available
* Angular is based on modular approch.
* Angular is following component structure.By using components we can reuse codes and make testing easy
* Dependency injection- it  allows a class to receive dependencies from another class.
* Command Line Interface (CLI) –The Angular CLI is a command-line interface tool that you use to initialize, develop, and maintain Angular applications directly from a command       shell.This way, development and testing processes both become faster.

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

#### Bootstrapping in Angular
 Bootstrapping is a technique of initializing or loading our Angular application.    
 The Angular takes few steps to load our first view.             
 * Index.html Loads First
 * Angular, Third-party libraries & Application loads   
 * Main.ts the application entry point
 * Root Module -The angular bootstrapper loads our root module AppModule.
 * Root Component
 * Template

  
8. ### Angular Decorators
  Decorators are design patterns used to isolate the modification or decoration of a class without modifying the source code. 
  Decorators are the features of Typescript and are implemented as functions. The name of the decorator starts with @ symbol following by brackets and arguments.    
  
__1.Class Decorators__
Class Decorators are the top-level decorators that are used to define the purpose for the classes. 
They provide information to Angular that a particular class is a component, or module

__@NgModule Decorator__       
It defines the class is an Angular Module and  provides metadata about the module.

__@Component Decorator__      
It defines the class is an Angular Component and  provides metadata about the component.  

__@Injectable Decorator___
It Declares that a class has dependencies that should be injected into the constructor when the dependency injector is creating an instance of this class.       

__@Directive Decorator___   
It defines the class as an Angular directive. The directives help us to change the appearance, behavior, or layout of a DOM element.

__@Pipe Decorator___     
It defines the class as an  Angular Pipe  and provides metadata about the pipe.
