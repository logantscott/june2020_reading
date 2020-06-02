[Table of Contents](https://github.com/logantscott/june2020_reading)

### Reading, Research, and Discussion
1. Name 3 advantages to Test Driven Development  
It can speed up development over time, can help make the code base more maintainable, and can easily help identify errors before going to production.
1. In what case would you need to use beforeEach() or afterEach() in a test suite?  
Working with a database (especially where you only temporarily want data populated, add before and remove after)
1. What is one downside of Test Driven Development  
It's slow/expensive to start development because there's a lot of upfront work to get tests up and running.
1. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?  
A class can be instantiated. 
1. Name a use case for a static method  
Maybe a person is a class, a common method would be firstname + lastname. No sense to make that an instance method if it's going to be used a lot, so make it a static method.
1. Write an example of a Higher Order function and describe the use case it solves  
```javascript
function fixArray(someArray) {
  someArray.map(arrayItem => doMath(arrayItem))
}
```
The simpler function *doMath* can be used separately from the *fixArray* function if needed.


### Vocabulary
**functional programming**  
The process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through *pure functions*.

**pure function**  
- Its return value is the same for the same arguments (no variation with local static variables, non-local variables, mutable reference arguments or input streams from I/O devices). 
- Its evaluation has no side effects (no mutation of local static variables, non-local variables, mutable reference arguments or I/O streams).

**higher-order function**  
A function that takes a function as an argument, or returns a function. Higher order function is in contrast to first order functions, which don’t take a function as an argument or return a function as output.

**immutable state**  
State that cannot be changed.

**object**  
In *object-oriented programming (OOP)*, is an abstract data type created by a developer. It can include multiple properties and methods and may even contain other objects. In most programming languages, objects are defined as *classes*.

**object-oriented programming (OOP)**  
Refers to a programming methodology based on *objects*, instead of just functions and procedures. These *objects* are organized into *classes*, which allow individual *objects* to be grouped together.

**class**  
Used in *object-oriented programming* to describe one or more objects. It serves as a template for creating, or instantiating, specific objects within a program. While each object is created from a single class, one class can be used to instantiate multiple objects.

**prototype**  
In JavaScript, the JavaScript engine adds a prototype property to the function. This prototype property is an object (called a prototype object) that has a constructor property by default. The constructor property points back to the function on which prototype object is a property. A function's prototype property can be accessed using *functionName.prototype*.

**super**  
Used to access and call functions on an object's parent. When used in a constructor, the super keyword appears alone and must be used before the this keyword is used. The super keyword can also be used to call functions on a parent object.

**inheritance**  
Inheritance is a major feature of *object-oriented programming*.  Data abstraction can be carried up several levels, that is, *classes* can have superclasses and subclasses. You can choose which of the superclass's attributes and methods to keep and add your own, making class definition very flexible. Some languages let a class inherit from more than one parent (multiple inheritance).

**constructor**  
A special method for creating and initializing an object created within a *class*. A constructor enables you to provide any custom initialization that must be done before any other methods can be called on an instantiated object. A constructor belongs to a particular class object that is instantiated. The constructor initializes this object and can provide access to its private information. The concept of a constructor can be applied to most object-oriented programming languages. Essentially, a constructor in JavaScript is usually declared at the instance of a class.

**instance**  
An *object* created by a *constructor* is an *instance* of that *constructor*.

**context**  
Context is always the value of the *this* keyword which is a reference to the object that “owns” the currently executing code or the function where it’s looked at.

**this**  
A property of an execution context (global, function or eval) that, in non–strict mode, is always a reference to an object and in strict mode can be any value.

**Test Driven Development (TDD)**  
A software development process that relies on the repetition of a very short development cycle: requirements are turned into very specific test cases, then the code is improved so that the tests pass.

**Jest**  
A delightful JavaScript Testing Framework with a focus on simplicity. Jest is a JavaScript testing framework designed to ensure correctness of any JavaScript codebase. It allows you to write tests with an approachable, familiar and feature-rich API that gives you results quickly.

**Continuous Integration (CI)**  
Automatically build and test your code as you push it to GitHub, preventing bugs from being deployed to production.

**unit test**  
A level of software testing where individual units/ components of a software are tested. The purpose is to validate that each unit of the software performs as designed. A unit is the smallest testable part of any software. It usually has one or a few inputs and usually a single output.