# Application Architecture, MVC Design Pattern
01. What are the Pillars of Object Oriented Programming (`OOP`)?
  
  >	• Encapsulation: The bundling of data and the methods that act on that data such that access to that data is restricted from outside the bundle. This means that an object stores its state privately, and only the object’s methods have access to change it. • Abstraction: Abstraction is an extension of encapsulation. It is the process of selecting data from a larger pool to show only the relevant details to the object. • Inheritance: Inheritance is the ability of one object to acquire some/all properties of another object. • Polymorphism: Polymorphism gives us a way to use a class exactly like its parent so there is no confusion with mixing types.

02. How does `export` differ from `export default`?
  
  > JavaScript modules export values as live bindings except with export default.

03. What is Encapsulation?
  
  >Encapsulation is the bundling of data and the methods that act on that data such that access to that data is restricted from outside the bundle. It ensures that your data is clean and cannot be accessed directly.

04. What are some of the benefits of the `Proxy` object that we are using in our structure for applications?
  
  >They allow you to provide custom functionality to basic operations that can be performed on an Object. 

05. What the difference between a `class` and an instance of a `class`?
  
  >a Class . Class Instance is hard-coded in your AppState, as a default.

06. What is a computed Property?
  
  > ES6 allows you to use an expression in brackets []. It’ll then use the result of the expression as the property name of an object. 

07. What is the purpose of the `MVC` pattern?
  
  > Topline: It provides for a better division of labor and improved maintenance. The MVC (Model-View-Controller) is an architectural pattern that separates an application into three main logical components: the model, the view, and the controller. This is done to separate internal representations of information from the ways information is presented to and accepted from the user

08. What is the job of the `Controller` in the `MVC` Pattern?
  
  >Controllers (HomeController.js, GachamonsController.js, etc.): Controllers handle user input and interaction. They are instantiated when a route is loaded. They interact with the AppState to retrieve and update data. They also call the view rendering methods and listen to changes in the AppState.

09. What is the job of the `Service` in `MVC`?
  
  > Services (GachamonsService.js, etc.): Services manage business logic, data manipulation, and interactions with the backend. They are responsible for updating the AppState with new data and triggering listeners when changes occur.

10. What is the job of the `Model` in `MVC`?
  
  > Model (Gachamon.js, Value.js, etc.): Models define the data structure and encapsulate the logic related to data manipulation. They generate HTML templates to be used by the views.
