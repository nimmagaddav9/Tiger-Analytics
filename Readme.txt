1. What is your experience with Angular (8+), and how do you manage state in large applications?
   Answer:
   I've used Angular extensively in enterprise-scale applications. For state management, I've employed NgRx when dealing with complex shared state and RxJS for reactive data flows.
   I follow best practices like lazy loading, modular architecture, and using facades to abstract NgRx selectors and dispatches. This ensures scalability and maintainability.

2. How have you used TypeScript in full-stack development?
   Answer:
   TypeScript is my default language for both frontend (Angular) and backend (NestJS).
   It helps enforce type safety, reduces bugs during development, and improves developer experience via IDE support.
   On the backend, interfaces are shared between frontend and backend for consistency in data contracts, especially when using GraphQL or REST APIs.

3. Can you describe your experience with NestJS and building GraphQL APIs?
   Answer:
   I've built multiple APIs using NestJS due to its modular architecture and TypeScript support. For GraphQL, I’ve used @nestjs/graphql with Apollo Server, implementing resolvers, schemas, and integrating with services.
   I follow the code-first approach and use decorators to define types and inputs, which ensures tight integration and clear schema design.

4. Explain a scenario where you had to re-platform a legacy application to microservices in AWS.
   Answer:
   At [Previous Company], I led the effort to break a monolithic application into microservices hosted on AWS. We used ECS Fargate for containerized services, API Gateway + Lambda for
   lightweight endpoints, and DynamoDB for scalable storage. This shift improved deployment speed, scalability, and fault isolation.
   I also used CloudFormation for infrastructure-as-code.

5. How do you implement observability in your applications?
   Answer:
   Observability is essential for proactive monitoring and troubleshooting.
   I implement structured logging using Winston in Node.js, integrated with Splunk for log analysis.
   For metrics, I use AWS CloudWatch and Prometheus/Grafana where applicable. In the frontend, I use Sentry for error tracking.
   Alerts are configured based on thresholds or anomalies in logs/metrics.

6. What is your approach to testing in a TDD (Test Driven Development) environment?
   Answer:
   I start by writing unit tests for services/components using Jest (NestJS) and Jasmine/Karma (Angular).
   For API endpoints, I use Supertest for integration testing. I ensure >80% test coverage and focus on writing meaningful tests, including edge cases. For frontend E2E testing,
   I use Cypress. TDD helps ensure robust and predictable code.

7. How do you optimize application performance both in frontend and backend?
   Answer:
   Frontend: I use lazy loading, OnPush change detection in Angular, tree shaking, and code splitting to reduce bundle size.

   Backend: Caching with Redis (Elasticache), pagination, batching (for GraphQL), and optimizing database queries. I also profile APIs for bottlenecks and optimize compute and memory in AWS Lambda and ECS tasks.

8. Describe your experience working with Nrwl Nx Monorepo tooling.
   Answer:
   Nx allows us to manage multiple apps and libraries in a single monorepo with great tooling support. I've used it to streamline CI/CD, enforce code boundaries, and reuse logic across Angular and NestJS apps. It improves developer velocity and ensures consistent coding practices across teams.

9. How do you handle security in your applications (frontend & backend)?
   Answer:
   Frontend: Sanitize inputs, use Angular’s built-in XSS protection, implement Content Security Policies (CSP), and avoid direct DOM manipulations.

   Backend: Use helmet, rate limiting, JWT for auth, role-based access, and validate inputs using class-validator in NestJS. Also implement secure communication (HTTPS, encryption for sensitive data).

10. Have you worked with AWS Cost-tagging or CloudHealth for cost optimization?
    Answer:
    Yes, I've used AWS tagging policies to apply cost allocation tags to resources. This helps in identifying unused or underutilized resources.
    With CloudHealth, we analyze usage patterns, optimize reserved instances, and generate cost reports to maintain budget efficiency.

11. What is Dependency Injection in Angular?
    Communication between the component and Services is called DI.
    design pattern, integrate post and get API.

12. can we inject service without a constructor in the component?

13. features of angular 16? Do you know the application loads in angular 16?
    standalone project support
    SSR(server side rendering)
    syntax optimization

14. What's new in Angular 17?
    Typescript 5.2
    New Declarative Control flow
    Deferrable loading

15. How many ways we can create form in angualr ? which one is better?
    2types
    Template-driven forms
    Reactive Forms(Model-driven Forms)

if requirement simple form 2-3 fields template-driven forms
for complex - reactive forms

16. If we a form how will you set the value?
    setValue()
    patchValue()

17. What is Directives in angular ?
    To enhance view capabilities or view features we go for directives.
    change the structure of DOM at run time.
    Structural directives: ngStyle and ngClass
    Component Directive: ngIf, ngFor, ngSwitch

18. what is host binding and host listener?

@HostBinding and @HostListener are decorators in Angular that allow you to interact with the host element of a directive or a component.

Ex: @HostBinding('style.backgroundColor')
Ex: @HostListener('click')

19. Do you know the features of Standalone components?
    Standalone components are designed to be reusable and self-contained meaning they don't have strong dependencies on other components or services within the application.
    Ex: date picker, a modal dialog, a notification component, a progress bar or file uploader.

    key characteristics
    isolation
    Reusability
    Encapsulation
    Minimal dependencies
    Clear Responsibilities
    Independent Styling

20. What are differ blocks?

21. What are signals? Angular 17

22. What is interceptor?
    API call with redux with interceptor we can set Http headers and response(manupulate request and response)

23. how to add a header in the request?

24. rxjs operators? async operations
    do you know what operator is mostly used from rxjs? filter, mergeMap, switchMap, concatMap, combineLatest

25. How to handle errors in services?
    handling errors in services typically involves using RxJS observables along with the catchError operator.

    getData() method sends a HTTP GET request using Angular HttpClient and returns an observable.
    handleError() method is a private method in the service that receives the error as an argument.

26. difference between pure pipes and impure pipes?
    Pure Pipes are immutable and produce a new value when the input data changes.

    Impure pipes might be called more frequently as they are executed everytime there is a change detection cycle, even if the input hasm't changed.

27. What are standalone components?

28. Do you know SSR? Do you know Ngrx?

29. If you have 1 module in that you module you have 10 components then how will you implement this?

how can you pass the data between 10 components?
how will you get value in emit or do you know another way to use what subject you can use?

20. Can we use the subject to share data between 10 components?

21. What is change detection strategy in angular? what is on push and what is drawback of the default one?

In Angular, change detection is the mechanism that determines when and how the framework updates the Document Object Model (DOM) to reflect changes in your component's data.

============================
Section 1: Introduction & Experience

1. Tell me a little bit about yourself and your professional background.

I’m a Core UI Developer with over 12 years of experience building scalable and responsive .com websites across various industries. My technical expertise spans HTML5, CSS3, JavaScript, Angular 18, React.js, and Redux.

For the past two years, I’ve been part of the React migration team at United Airlines, where I helped modernize the united.com platform by converting legacy .NET pages to React. We leveraged the company-wide ATMOS component library and used Redux-Saga to handle asynchronous logic efficiently. I’ve contributed to multiple user account management features such as Sign-In, Forgot Password, MileagePlus recovery, Security Questions, United Club Pass, Recent Activity, and dashboard updates. I also implemented features like Known Traveler Number (KTN), Accessibility compliance, TSA PreCheck, Miles Pooling, and Under18 account functionality.

Before that, I was part of the Accelerator team at Visa, where I worked on remediating MBDA modules like Application and Account Management, Portfolio tools, Analytics, Recurring Billing, and Virtual Terminal—serving major banks like Wells Fargo and Bank of America.

At Capital Group, I worked on the DAVIS (Data Visualization) project where we built interactive highcharts using React and integrated them into the AEM platform, with a Java backend. I also contributed to the Creative Workbench tool used to publish articles on the Capital Group websites.

Earlier in my career, I built medical examination forms at Cerner Corporation, contributed to Black Friday reporting dashboards at Office Depot, and developed a tax portal and a school management website for Vignan schools at Satinos Technologies.

I’m passionate about building intuitive, secure, and high-performing user interfaces that enhance customer experience, and I’m always excited to take on challenges that push my skills further.

2. Why are you interested in this role at Tiger Analytics?

I’m excited about this role at Tiger Analytics because it aligns perfectly with both my technical background and my passion for building scalable, user-focused applications. I’m particularly drawn to the opportunity to work on cloud-based microservices and modern front-end technologies like Angular and NestJS, which I’ve been exploring alongside my core experience in React and Redux.

Tiger Analytics' reputation for solving complex business problems using data and technology really appeals to me. I’m also interested in the observability and performance monitoring aspects of the role—it shows the company’s focus on building robust, production-grade systems.

Overall, I see this as a chance to contribute my UI expertise while growing in a full-stack and data-driven environment that values innovation and collaboration.

3. Can you walk me through a recent project where you worked with AWS and microservices?
   What was your role, and what challenges did you overcome?

In a recent project at united.com, I worked on account security and management features using a microservices architecture hosted on AWS. My role focused on the frontend, integrating with backend services via API Gateway and handling async operations with Redux-Saga.

We used AWS Lambda for serverless logic and DynamoDB for data. A key challenge was managing inconsistent error responses across services, so I built a centralized error-handling layer to streamline the UX. I also collaborated closely with backend and security teams to ensure data protection and compliance, especially for features like KTN and Miles Pooling.

This project enhanced my experience working in cloud-native, microservices environments and reinforced my ability to deliver secure, scalable UI integrations.

Section 2: Technical Questions

4. TypeScript & Angular: How have you used TypeScript in your projects? What are some key advantages over JavaScript?

I’ve used TypeScript extensively in recent projects, especially with React and Angular, to build scalable and maintainable UI components. It helps catch errors early through static typing and improves code readability and auto-completion, which speeds up development. Compared to JavaScript, TypeScript offers better tooling support, safer refactoring, and stronger collaboration in large codebases.

5. Can you explain dependency injection in Angular and why it's useful?
   Communication between the component and Services is called DI.

   It’s useful because it:

Promotes modularity: Components focus on their own logic without managing how dependencies are created.

Enhances testability: You can easily swap real services with mocks during testing.

Improves maintainability: Dependencies are managed centrally, making it easier to update or replace them without changing the components.

Supports reusability: Services can be shared across multiple components without duplication.

6. Node.js & Nest.js: How does Nest.js improve backend development compared to Express.js??

   Nest.js builds on Express.js by adding a modular, scalable architecture with built-in support for TypeScript, dependency injection, and decorators. It enforces best practices, improves code organization, and makes backend development more maintainable and testable compared to plain Express.js.

7. What strategies do you use for GraphQL performance optimization in a microservices architecture?

   For GraphQL performance optimization in a microservices setup, I use:

   Query batching and caching to reduce redundant requests.

   DataLoader to batch and cache database or service calls within a request.

   Schema stitching or federation to efficiently combine microservices without overfetching.

   Pagination and filtering to limit data volume.

   Proper error handling and monitoring to quickly identify bottlenecks.

   And optimizing resolver logic to minimize unnecessary computations.

   These strategies help keep GraphQL APIs fast and scalable across distributed services.

8. How would you implement observability and monitoring in a cloud-based application using Splunk or another tool?

I’d implement observability by integrating centralized logging, metrics, and tracing into the cloud app. For example, using Splunk, I’d send logs and events from all services to Splunk’s platform for real-time analysis and alerting. I’d instrument the app with structured logs, expose key metrics (like latency and error rates), and use distributed tracing to track requests across microservices. This setup helps quickly identify issues, monitor performance, and ensure reliability.

9. What are the benefits of using Nrwl Nx for monorepo tooling, and how have you applied it?

Nrwl Nx offers powerful monorepo tooling that improves code sharing, enforces consistent standards, and speeds up builds with intelligent caching. It provides advanced dependency graph visualization and supports multiple frontend and backend frameworks in one workspace. I’ve used Nx to streamline development across teams by managing shared libraries, enabling scalable builds, and simplifying testing and deployment processes.

10. If you were designing an API in AWS, would you use GraphQL or REST? How do you decide?

I’d choose between GraphQL and REST based on the API’s needs. If clients require flexible, precise queries and want to minimize over-fetching or under-fetching of data, I’d prefer GraphQL. It’s great for complex, interconnected data and evolving frontend requirements.

If the API is simpler, with well-defined resources and straightforward CRUD operations, REST is often easier to implement and cache.

In AWS, both can be supported—REST via API Gateway and Lambda, and GraphQL via AWS AppSync—so the decision depends mainly on data complexity, client needs, and development speed.

11. AWS Services: What are the key differences between DynamoDB and RDS? When would you choose one over the other?

DynamoDB is a fully managed NoSQL database designed for high scalability and low-latency key-value or document storage. It’s schema-less and ideal for flexible, high-throughput applications with unpredictable traffic.

RDS is a managed relational database service supporting SQL databases like MySQL, PostgreSQL, and SQL Server. It’s best when you need complex queries, transactions, and strong relational integrity.

I’d choose DynamoDB for highly scalable, flexible workloads without complex joins, and RDS when the application requires structured data, complex relationships, or ACID transactions.

Section 3: Problem-Solving & System Design

12. Let's say you're asked to design a Fund Comparison tool from scratch. What would your approach be? How would you decide on the frontend, backend, and cloud architecture?

    To design a Fund Comparison tool, I’d start by understanding the key features and user needs. For the frontend, I’d use React or Angular with charting libraries for data visualization. The backend would be a REST or GraphQL API built with Node.js (NestJS or Express) to handle data processing and business logic.

    For the database, I’d choose AWS RDS for complex queries or DynamoDB for scalability. Cloud-wise, I’d host the backend on AWS Lambda or EC2, use API Gateway for APIs, and serve frontend assets via S3 and CloudFront. Security, caching, and monitoring would be integral to ensure performance and reliability.

13. Imagine your application is facing high latency in AWS Lambda functions. How would you diagnose and solve the issue?
    I’d start by reviewing CloudWatch logs and metrics to identify where latency spikes occur. Then, I’d check for cold starts and optimize by using provisioned concurrency if needed. I’d also analyze function code for inefficient logic or external API calls causing delays. Additionally, I’d review memory and timeout settings to ensure adequate resources. Finally, I’d consider breaking down the function into smaller parts or using caching to reduce execution time.

14. You've been assigned to refactor an old monolithic service into microservices. What are the first steps you would take?

    First, I’d analyze the monolith to understand its components and dependencies. Then, I’d identify logical boundaries to split the service into smaller, independent microservices based on business domains. Next, I’d define clear APIs for each service and plan data ownership to avoid tight coupling. I’d also set up CI/CD pipelines and choose appropriate communication methods like REST or messaging. Finally, I’d refactor incrementally, ensuring proper testing and monitoring throughout the process.

Section 4: Behavioral & Soft Skills

15. Tell me about a time you had a disagreement with a team member about a technical implementation. How did you resolve it?

    In one project, a teammate and I disagreed on whether to use a third-party library or build a custom solution. I suggested evaluating both options based on factors like maintainability, performance, and long-term support. We discussed pros and cons openly, involving the team to get broader input. After reviewing, we agreed to use the third-party library because it met our needs and saved development time. This collaborative approach ensured we made a well-informed decision and kept the project on track.

16. How do you stay up to date with the latest technologies, especially in frontend and cloud development?

    I stay updated by regularly following tech blogs, official documentation, and newsletters like Smashing Magazine and AWS blogs. I participate in online communities like Stack Overflow and GitHub, attend webinars and conferences when possible, and experiment with new tools through side projects. This helps me keep my skills current and apply the latest best practices in frontend and cloud development.

17. What do you do when you encounter a bug that you can’t immediately solve? What’s your debugging process?

    When I hit a tough bug, I first reproduce it consistently to understand the issue. Then, I isolate the problem by narrowing down the code and checking recent changes. I use debugging tools, logs, and breakpoints to gather more details. If needed, I consult documentation or ask teammates for insights. Once I identify the root cause, I fix it and thoroughly test to ensure it’s resolved without side effects.


JavaScript Interview Questions and Answers
========================================================

1. What are the data types in JavaScript?
JavaScript has eight data types, divided into two categories: primitive and non-primitive (object).

let number = 100;
let string = "hi";
let boolean = true;
let undefinedValue;
let nullValue = null;
let symbol = Symbol("unique");
let bigInt = 123455655555n;
let object = {name: "vijay", age: 21}


2. What is the difference between == and ===?
The == (equality) and === (strict equality) operators are used for comparison in JavaScript.
== (Equality): Performs type coercion before comparison and then it compares values after converting them to a common type.
=== (Strict Equality): Does not perform type coercion and it compares both value and type.

example:
console.log(5 == '5'); //true (compares string to number)
console.log(5==='5'); // false (different types)

3. What is the difference between null and undefined?
Null and undefined are both used to represent the absence of a value.
Null: Must be explicitly assigned. Typeof null returns "object" (this is a known JavaScript bug)
Undefined: Represents a variable that has been declared but not assigned a value .Typeof undefined returns "undefined"

let nullVar = null;
console.log(nullVar); //null
console.log(typeOf null); //"object"

let undefinedVar;
console.log(undefinedVar); //undefined
console.log(typeOf undefined); //"undefined"

4. Explain the concept of hoisting in JavaScript.
Hoisting is a behavior in JavaScript where variable and function declarations are moved to the top of their respective scopes during the compilation phase, before the code is executed. 
This means that regardless of where variables and functions are declared in the code, they are treated as if they are declared at the beginning of their scope.

example:
console.log(x); //output: undefined
var x = 5;
console.log(x); //output: 5

the declaration of x is hoisted to the top, but not its initialization. That's why the first `console.log outputs undefined.

let and const declarations are hoisted but not initialized. This leads to a "temporal dead zone" where accessing the variable before its declaration results in a ReferenceError.

console.log(y);
// throws ReferenceError: Cannot access 'y' before "initialization"
let y = 10;



5. What is the difference between let, const, and var?

var: Function-scoped or globally-scoped. Can be redeclared and updated and Hoisted and initialized with undefined.

let: Block-scoped. Hoisted but not initialized (Temporal Dead Zone).

const: Block-scoped. Cannot be updated or redeclared. Hoisted but not initialized (Temporal Dead Zone)

const a = 10;
a=20; // can't do this


6. What is variable scope in JavaScript?
Variable scope refers to the context in which a variable is declared and can be accessed. In JavaScript, there are two main types of scope:
Global Scope: Variables declared outside any function or block
Local Scope: Variables declared inside a function or block
JavaScript uses lexical scoping, which means that inner functions have access to variables in their outer scope.

let globalVar = "global";

function exampleFuntion(){
    let localVar = "local";

    console.log(globalVar); // "global"
    console.log(localVar); // "local"
}

exampleFuntion();
console.log(globalVar); // global
console.log(localVar);  // ReferenceError: localVar is not defined


7. Explain the difference between global and local variables.
Global Variables: Declared outside any function or block. Accessible from anywhere in the code, including inside functions. Have global scope
Local Variables: Declared inside a function or block. Only accessible within that function or block. Have local scope



8. What is the temporal dead zone?
The Temporal Dead Zone (TDZ) is the period between entering a scope and the point where a variable is declared and initialized.

Applies to variables declared with let and const.
Helps catch errors by preventing access to variables before they're declared

console.log(x);
let x = 5; // ReferenceError: Cannot access 'x' before initialization


9. What is variable shadowing?
Variable shadowing occurs when a variable declared in a certain scope has the same name as a variable in an outer scope. 
The inner variable "shadows" the outer one, effectively hiding it.

let x = 10;

function exampleFuntion(){
    let x = 20; // this x shadows the outer x
    console.log(x); // 20
    if(true){
        let x = 30; // this x shadows both outer x variables
        console.log(x); // 30
    }
    console.log(x); // 20
}
exampleFunction();
console.log(x); // 10

10. What is a closure in JavaScript?
if any inner function holding the outer function data, then such scenario called as closure.

<script>
    function fun_one(){
        var x = 10;
        var y = 20;
        return ()=>{
            console.log(x);
            console.log(y);
        }
    };
    console.dir( fun_one() );  //0: Closure (fun_one) {x: 10, y: 20}
  
</script>


11. What are the different ways to define a function in JavaScript?

// Function declaration: hoisted and can be called before it's defined.
function great(name){
    return `hello, ${name}!`;
}

// Function expression: assigned to a variable, not hoisted
const greet = function(name){
    return `hello, ${name}!`;
};


//arrow function: shorter syntax, lexically binds 'this'
const greet = (name) => `hello, $ {name}!`;

//function constructor: creates a function dynamically
const greet = new Function("name", return `Hello, ${name}!`;");


12. What is a higher-order function?
A higher-order function is a function that treats other functions as data, either by taking them as arguments or returning them.

// Higher-order function that takes a function as an argument
function operate(x, y, operation){
    return operation(x, y); // calls the passed function with x and y
}

// function to be passed as arguments
const add = (a, b) => a + b; // arrow function for addition
const multiply = (a, b) => a * b; // arrow function for multiplication

//using higher order function
console.log(operate(5, 3, add)); // 8
console.log(operate(5,3, multiply)); // 15

13. Explain the concept of function hoisting?
Function hoisting is JavaScript's behavior of moving function declarations to the top of their scope during the compilation phase. 
This allows you to call a function before it appears to be defined in the code.

//this works due to hoisting
sayHello(); //output : "hello"

//function declaration is hoisted to the top of its scope
function sayHello(){
    console.log("hello!");
}

//note: function expressions are not hoisted
// hello(); // this would cause an error  --> ReferenceError: Cannot access 'hello' before initialization
// const hello = function(){console.log("hello");};

14. What is a pure function?
A pure function is a function that: Always returns the same output for the same inputs. 
Has no side effects (doesn't modify external state). Doesn't rely on external state. Make code more predictable and easier to test.

//pure function: always returns the same
//output for the same inputs
function add(a, b){
    return a + b; //deterministic and no side effects
}

// Impure function: modifies external state
let total = 0;
function addToTotal(value){
    total+= value; //modifies external variable 'total'
    return total;
}

15. What is the difference between function declaration and function expression?
Hoisting: Function declarations are hoisted, function expressions are not. 

Usage: Function declarations can be called before they appear in the code, function expressions cannot.

Naming: Function declarations require a name, function expressions can be anonymous.

// function declaration: hoisted and can be called before definition
sayHello(); // works due to hoisting
function sayHello(){
    console.log("hello");
}

// function expression: not hoisted, must be defined before use
// greet(); // error
const greet = function() {
    console.log("greetings");
};
greet(); // works when called after the expression.


16. What is an Immediately Invoked Function Expression (IIFE)?

An IIFE is a JavaScript function that runs as soon as it is defined.
// Arrow function with IIFE syntax
(()=>{
    console.log("Arrow function IIFE");
})();

//IIFE with parameters
(function(name){
    console.log(`hello, ${name}!`);
})("john");


17 How do you create an object in JavaScript?

//object literal notation
let person1 = {
    name : "vijay",
    age: 30,
    greet: function() {
        console.log(`hello, i'm {this.name}`);
    }
};

//constructor function
function Person(name, age){
    this.name = name;
    this.age = age;
    this.greet = function(){
        console.log(`hello, i'm ${this.name}`);
    };
}
let person2 = new Person("bob", 25);

-------------------------------------------
//object.create() method
let personProto = {
    greet: function() {
        console.log(`hello, i'm ${this.name}`);
    }
};
let person3 = Object.create(personProto);
person3.name = "charlie";
person3.age = 35;

//Es6 class syntax
class PersonClass {
    constructor(name, age){
        this.name = name;
        this.age = age;
    }
    greet(){
        console.log(`hello, i'm ${this.name}`);
    }
}
let person4 = new PersonClass("David", 40);

18 How do you add/remove properties to an object dynamically?

let car = {
    brand: "toyota",
    model: "corolla",
};

//adding properties
car.year = 2022; // dot notation
car["color"] = "blue"; //bracket notation

//removing properties
delete car.model; // removes the "model" property


19. How do you check if a property exists in an object?

let person = {
    name: "Alice",
    age: 30,
};

// using the in operator
console.log("name" in person); //true
console.log("job" in person); //false

// using hasOwnProperty method
console.log(person.hasOwnProperty("age")); // true
console.log(person.hasOwnProperty("city")); // false

// using undefined check
console.log(person.name !== undefined); // true
console.log(person.salary !== undefined); //false

// using Optional Chaining
console.log(person?.job); // undefined


20. What is the purpose of the this keyword in JavaScript?

The `this` keyword refers to the object that is executing the current function. Its value is determined by how a function is called.

// In a method
let person = {
    name: "alice",
    greet(){
        console.log(`hello, i'm ${this.name}`);
    },
};
person.greet(); //output: hello, i'm alice


// In an arrow function
let arrowGreet = () => {
    console.log(`hello, ${this.name}`);
};
arrowGreet.call({name: "charlie"}); 
// Output: hello, undefined (arrow functions don't bind their own 'this')

// In a constructor function
function Person(name){
    this.name = name;
    this.greet = function (){
        console.log(`hello, i'm ${this.name}`);
    };
}
let david = new Person("david");
david.greet(); //Output: hello, i'm david


21 What are the different ways to loop through an array in JavaScript?
1. for loop
2. for...in
3. for...of
4. map method(creates a new array)
5. while loop
6. do..while loop

example:
const fruits = ["apple", "banana", "orange", "mango"];

// 1.  for loop
for(let i =0; i < fruits.length; i++){
    console.log(fruits[i]);
}

// output: 
apple
banana
orange
mango

// 2. forEach method
fruits.forEach((fruit, index)=>{
    console.log(`${index}: ${fruit}`);
});

// output:
0: apple
1: banana
2: orange
3: mango

// 3. for... of loop(Es6+)
for(const fruit of fruits){
    console.log(fruit);
}

// output:
apple
banana
orange
mango

// 4. map method (creates a new array)
const upperFruits = fruits.map((fruit)=> fruit.toUpperCase());
console.log(upperFruits);
// Output:
[ 'APPLE', 'BANANA', 'ORANGE', 'MANGO' ]


// 5. while loop
let i = 0;
while(i < fruits.length){
    console.log(fruits[i]);
    i++;
}
// output:
apple
banana
orange
mango

// 6. do...while loop
let j = 0;
do {
    console.log(fruits[j]);
    j++;
} while(j < fruits.length);

// output
apple
banana
orange
mango


22. Explain the difference between for...in and for...of loops.

Key differences:
1. for...in iterates over all enumerable properties(including inherited ones)
2. for...of iterates over the values of an iterable object
3. for...in is generally used for objects, while for...of is used for arrays and other iterables

const fruits = ["apple", "banana", "orange"];
fruits.color = "mixed"; // adding a property to the array

// for...in loop(iterates over properties)
for(let index in fruits){
    console.log(index); 
} 

// output:
0
1
2
color

// for...of loop(iterates over iterable values)
for(let fruit of fruits){
    console.log(fruit);
}
// output:
apple
banana
orange


23. How do you add/remove elements from an array?

let fruits = ['apple', 'banana', 'orange'];

// adding elements
fruits.push('mango');
console.log(fruits);
// adds to the end: [ 'apple', 'banana', 'orange', 'mango' ]

fruits.unshift('grape');
console.log(fruits);
// adds to the beginiing: [ 'grape', 'apple', 'banana', 'orange', 'mango' ]

// removing elements
let lastFruit = fruits.pop();
console.log(fruits); // [ 'grape', 'apple', 'banana', 'orange' ]
// removes from the end: lastFruit = "mango"

let firstFruit = fruits.shift();
console.log(fruits); // [ 'apple', 'banana', 'orange' ]
// removes from the beginning: firstFruit = 'grape'

// adding/removing at specific index
fruits.splice(1, 0, 'kiwi');
console.log(fruits);  // [ 'apple', 'kiwi', 'banana', 'orange' ]
// adds 'kiwi' at index 1.

24. What is the purpose of the map() function? Es6 method
The map() method creates a new array with the results of calling a provided function on every element in the array.

const numbers = [1, 2, 3, 4, 5];

// using map to double each number
const doubledNumbers = numbers.map(num => num * 2);
console.log(doubledNumbers);  // [ 2, 4, 6, 8, 10 ]

// using map to create object from each number
const numberObjects = numbers.map(num => ({value: num, squared: num * num}));
console.log(numberObjects);
// Output:
[
  { value: 1, squared: 1 },
  { value: 2, squared: 4 },
  { value: 3, squared: 9 },
  { value: 4, squared: 16 },
  { value: 5, squared: 25 }
]

25. Explain the difference between filter() and find() methods. (ES6 methods)

Key differences:
1. filter() returns an array, find() returns a single element or undefined.
2. filter() checks all elements, find() stops at the first match.
3. filter() is used when you need all matching elements, find() when you need just the first match.

const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// filter(): returns a new array with all elements that pass the test
const evenNumbers = numbers.filter(num => num % 2 === 0);
console.log(evenNumbers); // [ 2, 4, 6, 8, 10 ]

// find(): returns the first element that satisfies the condition
const firstEvenNumber = numbers.find(num => num % 2 === 0);
console.log(firstEvenNumber); // 2

26. Explain the difference between some() and every() method.
some() method: Returns true if at least one element in the array satisfies the provided testing function. 
               Stops iterating as soon as it finds an element that satisfies the condition. 
               Returns false if no elements satisfy the condition.


every() method: Returns true if all elements in the array satisfy the provided testing function. 
                Stops iterating as soon as it finds an element that doesn't satisfy the condition.

const people = [
    {name: 'alice', age: 25 },
    {name: 'bob', age: 30},
    {name: 'charlie', age: 35}
];

// check if any person is over 30
const anyOver30 = people.some(person => person.age > 30);
console.log(anyOver30); // true (charlie is over 30)

// check if all people are over 20
const allOver20 = people.every(person => person.age > 20);
console.log(allOver20); // true (all are over 20)


27. How do you select elements in the DOM using JavaScript?

<div id = "myDiv" class="myClass">
    <p>First paragraph</p>
    <p>Second paragraph</p>
</div>

// select by ID
const divById = document.getElementById('myDiv');

// select by class name (returns a live HTMLCollection)
const elementByClass = document.getElementByClassName('myClass');

// select by tag name(returns a live HTMLCollection)
const paragraphs = document.getElementByTagName('p');

// select using CSS selectors (returns the first matching element)
const divBySelector = document.querySelector('#myDiv');

// select all matching elements using CSS selectors (returns a static NodeList)
const allParagraphs = document.querySelectorAll('p');

// using newer methods (less browser support)
const divByID = document.getElementById('myDiv');
console.log(divByID.querySelector('p')); // first <p> inside #myDiv
console.log(divByID.querySelectorAll('p')); // all <p> elemebts inside #myDiv 

28. How do you create and append elements to the DOM?

// create a new element
const newParagraph = document.createElement('p');

// set its content
newParagraph.textContent = "this is new paragraph.";

// add some attributes
newParagraph.id = "newPara";
newParagraph.className = "highlight";

// create a text node 
const textNode = document.createTextNode('Additional text.');

// append the text node to the paragraph
newParagraph.appendChild(textNode);

// append the new paragraph to an exisitng element
document.body.appendChild(newParagraph);

// alternative method using insertAdjacentHTML
const existingDiv = document.getElementById('existingDiv');
existingDiv.insertAdjacentHTML('beforeend', '<p>Inserted using unsertAdjacentHTML</p>');

29. Explain the difference between innerHTML and textContent.

Key differences:
innerHTML parses content as HTML, textContent does not
innerHTML can be slower and less secure (risk of XSS attacks)
textContent is generally faster and safer
innerHTML returns all content, including script and style element content
textContent returns the text content of all elements, ignoring tags

const div = document.createElement('div');

// innerHTML interprets the content as HTML
div.innerHTML = '<p>this is <strong>bold</strong> text</p>';
console.log(div.innerHTML);
// "<p>this is <strong>bold<strong> text<p>"

// textContent treats the content as plain text
div.textContent = '<p> this is <strong> bold</strong> text </p>';
console.log(div.textContent);
// "<p> this is <strong> bold </strong> text </p>"


30. How do you remove an element from the DOM?

<div id="parent"><p id="child">remove me</p></div>

// 1. method: using removeChild
const parent  = document.getElementById("parent");
const child = document.getElementById("child");
parent.removeChild(child);

// Method 2: using remove (newer, but less supported in older browsers)
const elementToRemove = document.getElementById("child");
elementToRemove.remove();

// Method 3: setting innerHTML to an empty string (removes all children)
document.getElementById("parent").innerHTML = "";

// Note: when removing elements, be sure to remove any associated event listeners
// to prevent memory leaks

31. What are arrow functions and how do they differ from regular functions?

key differences:
1. syntax: arrow functions have a more concise syntax.
2. "this" binding: arrow functions don't have their own "this"
3. No "arguments" object: arrow functions don't have the "argument" object


// arrow function
const addArrow = (a, b) => a + b;

// example of "this" binding difference
const obj = {
    name: "John",
    sayHello: function () {
        console.log("hello, " + this.name);
    },
    sayHelloArrow: () => {
        console.log("hello, " + this.name);
    },
};

obj.sayHello();
// output: hello, John

obj.sayHelloArrow();
// output: hello, undefined
// this refers to global/window object


32. Explain the concept of destructuring in JavaScript. ES6 concept
Destructuring is a way to extract multiple values from data stored in objects and arrays.

const person = {name: "alice" , age: 30, city: "new york"};

// old way
// const name = person.name;
// const age = person.age;

// destructuring
const {name, age, city} = person;
console.log(name, age, city); // alice 30 new york

// renaming variables
const { name: fullName, age: years } = person;
console.log(fullName, years); // alice 30

// array destructuring
const colors = ["red", "green", "blue"];

// Old way
// const firstColor = colors[0];
// const secondColor = colors[1];

// Destructuring
const [first, second, third] = colors;
console.log(first, second, third); // red green blue


33 What are template literals?
Template literals are string literals that allow embedded expressions and multi-line strings.

const nameVal = "alice";
const age = 30;

// old way
console.log("my name is " + nameVal + "and i'm" + age + "years old.");

// using tempalte literals
console.log(`my name is ${nameVal} and i'm ${age} years old.`); // my name is alice and i'm 30 years old.

// multi-line strings
const multiLine = `
this is a
multi-line
string
`;
console.log(multiLine); 
// output:
this is a
multi-line
string


34. How do you use the spread operator? Explain with example?
The spread operator (...) allows an iterable to be expanded in places where zero or more arguments or elements are expected.

// spreading arrays
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const combined = [...arr1, ...arr2];
console.log(combined); // (6) [1, 2, 3, 4, 5, 6]

// spreading objects
const obj1 = {a: 1, b: 2};
const obj2= {c: 3, d: 4};
const mergeObj = {...obj1, ...obj2 };
console.log(mergeObj); // (4) {a: 1, b: 2, c: 3, d: 4}

// copying arrays
const original = [1, 2, 3];
const copy = [...original];
copy.push(4);
console.log(original, copy); //(3) [1, 2, 3] (4) [1, 2, 3, 4]

// spreading strings
const str = "hello";
const chars = [...str];
console.log(chars); //(5) ["h", "e", "l", "l", "o"]

35. What are default parameters in ES6?
Default parameters allow you to set default values for function parameters if no value or undefined is passed.

// using default parameters
function greetES6(name = "guest"){
    console.log(`hello, ${name}!`);
}
greetES6(); // hello, guest!
greetES6("alice"); // hello, alice!

// default parameters with expressions
function multiply(a, b = a * 2){
    return a * b;
}
console.log(multiply(5)); // 50
console.log(multiply(5, 3)); // 15

36. How do you use the rest parameter in functions?
The rest parameter syntax allows a function to accept an indefinite number of arguments as an array.

//using rest parameter
function sumES6(...numbers){
    return numbers.reduce((total, num)=> total + num, 0)
}

console.log(sumES6(1, 2, 3, 4, 5)); // 15


// rest parameter with other parameters
function multiply(multiplier, ...numbers){
    return numbers.map((num)=> multiplier * num);
}
console.log(multiply(2,1,2,3,4)); // (4) [2, 4, 6, 8]

// object rest properties
const { a, b, ...rest} = { a: 1, b: 2, c: 3, d: 4};
console.log(a,b, rest); // 1 2 (2) {c: 3, d: 4}

//array rest elements
const [first, second, ...others] = [1, 2, 3, 4, 5];
console.log(first, second, others); // 1 2 (3) [3, 4, 5]

// rest parameters in arrow functions
const logAll = (...args) => console.log(args);
logAll(1, 2, 3, "four", {five: 5}); //(5) [1, 2, 3, "four", {...}]

37. What is callback & callback hell explain with example?
Callbacks are functions passed as arguments to other functions, often used for asynchronous operations. 
Callback hell occurs when multiple nested callbacks make code hard to read and maintain.

// simple callback example
function greet(name, callback){
    //simulate an async operation
    setTimeout(()=>{
        console.log(`hello, ${name}!`);
        callback();
    }, 1000);
}

// using the callback
greet("alice", ()=>{
    console.log("greeting finished");
});
// output:
hello, alice!
greeting finished

// Callback hell example
function step1(callback){
    setTimeout(()=>{
        console.log("step 1");
        callback();
    }, 1000);
}

function step2(callback){
    setTimeout(()=>{
        console.log("Step 2");
        callback();
    }, 1000)
}

// callback hell
step1 (()=>{
    step2(()=>{
        console.log("Done");
    });
});

// output
step 1
Step 2
Done

38. What is a Promise in JavaScript with example?
A Promise is an object representing the eventual completion or failure of an asynchronous operation.

// Promise example
function fetchData() {
    return new Promise((resolve, reject)=>{
        setTimeout(()=>{
            const success = true;
            if(success){
                resolve("data fetched successfully");
            } else {
                reject("error fetching data");
            }
        }, 1000);
    });
}

fetchData().then((data)=> console.log(data))
.catch((error)=> console.error(error));
// output: data fetched successfully


39. How do you chain Promises?
Promise chaining allows you to perform sequential asynchronous operations.

function step1(){
    return Promise.resolve("step 1 complete");
}

function step2(prevResult){
    return Promise.resolve(`${prevResult}, step 2 complete`);
}

step1()
    .then((result) => step2(result))
    .then((finalResult)=> console.log(finalResult))
    .catch((error)=> console.error(error));

    // output: step 1 complete, step 2 complete

40. What is the purpose of the Promise.all() method?
Promise.all() takes an iterable of promises and returns a single Promise that resolves when all input promises have resolved, or rejects if any input promise rejects.

const promise1 = Promise.resolve(3);
const promise2 = new Promise((resolve)=> setTimeout(()=> resolve(42), 100));

Promise.all([promise1, promise2])
.then((values)=> console.log(values))    // (2) [3, 42]
.catch((error)=> console.error(error));


41. What is the purpose of the finally() method in Promises?
The finally() method is used to specify code that should be executed regardless of whether the promise is fulfilled or rejected.

function fetchData(){
    return new Promise((resolve, reject)=>{
        const success = Math.random() > 0.5;
        setTimeout(()=>{
            if(success){
                resolve("data successfully fetched");
            } else {
                reject("Error: failed to fetch data");
            }
        }, 1000);
    });
}

fetchData()
    .then((result)=>{
        console.log(result);
    })
    .catch((error)=>{
        console.error(error);
    })
    .finally(()=>{
        // this block always run, regardless of fulfillment or rejection
        console.log("operation completed. loading status:");
    });

    //output:
    Error: failed to fetch data
    operation completed. loading status:


42 What is the purpose of the async await ?
The purpose of async/await is to simplify the syntax for working with Promises, making asynchronous code easier to write and read. 
It allows you to write asynchronous code that looks and behaves more like synchronous code.

// function that returns a promise
function fetchData() {
    return new Promise((resolve)=>{
        setTimeout(()=> resolve("data fetched"), 2000);
    });
}

// using async/await
async function getData() {
    console.log("fetching data...");
    const result = await fetchData();
    console.log(result);
    console.log("Data processing complete");
}

getData();

// output:
fetching data...
data fetched
Data processing complete

43. How do you handle errors in async/await?

async function fetchUserData(userId){
    try {
        const response = await fetch(`https://api.example.com/users/${userId}`);
        if(!response.ok){
            throw new Error('Failed to fetch user data');
        }
        const userData = await response.json();
        console.log(userData);
    } catch (errror){
        console.error("error:", error.message);
    }
}

fetchUserData(123);


44. What is the difference between async/await and Promises?
Syntax: Async/await provides a more linear, synchronous- looking code structure.
Error handling: Async/await uses try/catch, which is more familiar for synchronous code.
Chaining: Promises use .then() for chaining, while async/await uses regular JavaScript control flow.
Debugging: Async/await can be easier to debug as it behaves more like synchronous code


45. What is the difference between default and named exports?
A module can have multiple named exports but only one default export.
Named exports are imported using curly braces, while default exports are imported without them.
Default exports can be imported with any name, while named exports must be imported with their exact names (unless renamed using `as`).

// named exports
export const add = (a, b) => a + b;
export const subtract = (a, b) => a - b;

// default export
export default function multiply(a, b) {
    return a * b;
}

// importing named exports
import { add, subtract} from "./math.js";

// importing default export
import multiply from "./math.js; // it can be import vijay

console.log(add(5, 3)); // 8
console.log(subtract(10, 4)); // 6
console.log(multiply(2, 3)); // 6


46. How do you convert a JavaScript object to a JSON string ?

const user = {
    name: "john doe",
    age: 30,
    isAdmin: false,
};

const jsonString = JSON.stringify(user);
console.log(jsonString);
// Output: {"name":"john doe","age":30,"isAdmin":false}


47. How do you parse a JSON string back into a JavaScript object?

const jsonString = '{"name":"john doe","age":30,"isAdmin":false}';

const user = JSON.parse(jsonString);
console.log(user.name); // john doe
console.log(user.age); // 30
console.log(user.isAdmin); //false


48. What is localStorage in JavaScript, and how do you store and retrieve data from it?
localStorage is a web storage object that allows you to store key-value pairs in the browser with no expiration time.

// storing data
localStorage.setItem('username', 'vijay');
localStorage.setItem('isLoggedIn', 'true');

// retrieving data
const username = localStorage.getItem('username');
console.log(username); //vijay

const isLoggedIn = localStorage.getItem('isLoggedIn') === 'true';
console.log(isLoggedIn); // true

// storing and retrieving objects
const user = {name: 'John', age: 30};
localStorage.setItem('user', JSON.stringify(user));

const storedUser = JSON.parse(localStorage.getItem('user'));
console.log(storedUser.name); // John

49. What is the difference between localStorage and sessionStorage?
Both localStorage and sessionStorage are web storage objects, but they differ in data persistence.
localStorage data persists even after the browser is closed and reopened. 
sessionStorage data is cleared when the page session ends (i.e., when the tab is closed).
Both have the same API and are limited to storing string data.

// localstorage: persists even after the browser window is closed.
localStorage.setItem(
    "persistentData", 
     "This will remain after closing the browser"
);

// session storage: data is cleared when the browser session ends
sessionStorage.setItem(
    "temproraryData",
    "This will be cleared when the session ends"
);

// both are used similarly
console.log(localstorage.getItem("persistentData"));
console.log(sessionStorage.getItem("temporaryData"));

50. How do you delete a specific item from localStorage or clear all data from it?

// storing some data
localStorage.setItem("username", "JohnDoe");
localStorage.setItem("isLoggedIn", "true");

// removing a specific item
localStorage.removeItem("isLoggedIn");

console.log(localStorage.getItem("username")); //JohnDoe
console.log(localStorage.getItem("isLoggedIn")); // null

// clearing all data from localstorage
localStorage.clear();
sessionStorage.clear();

console.log(localStorage.getItem("username")); // null



=====
1. What is Angular? Why? Client-side structuring
Angular is a component-based framework for building structured, scalable(open and flexible) and single page web applications for client side.
SPA: Loading 1 component to another component without refreshing the whole project.

2. What are Angular advantages? building SPA.
It is Relatively simple to build Single Page Applications(Components).
To make flexible and structured applications(OOPS friendly)
It is Cross platform and Open Source(Free)
Reusable Code(Services)
Testability(Unit testing spec.ts file)

3. What is the difference between AngularJS and Angular?
Google Angular JS 2010 --> Angular 2, 4,

Angular JS                                    Angular
1. It only supports JavaScript.           1. It supports both JavaScript and Typescript.
2. This framework has MVC architecture.   2. This framework has a component based architecture.
3. It does not have CLI tool.             3. It has CLI Tool.
4. It does not use Dependency Injection.  4. It uses Dependency Injection.
5. It does not support mobile browsers.   5. It also support mobile browsers.
6. It is not so fast.                     6. It is very fast(Data binding and Component based architecture).

4. What is NPM?
Node Package Manager. Node.js --> NPM. google developed Node and Angular.
NPM/Node Package Manager is a Online repository from where you can get thousands of free libraries which can be used in your angular project.
The node_modules folder is used to save all downloaded packages from npm in your computer.


5. What is CLI tool?
CLI is command-line interface tool that you use to initialize and develop Angular applications.
Ex: ng generate component TestComponent

Components & Modules

6. What are Components in Angular?
Components are the most basic UI building block of an Angular app.
Ex: Inside src --> app --> app.component.css(CSS code), app.component.html(html template), app.component.spec.ts(Unit tests), app.component.ts(link css, html)

7. What is a Selector and Template?
A selector is used to identify each component uniquely into the component tree.
A template is a HTML view of an Angular component.

8. What is Module in Angular? What is app.module.ts file?
Module is a place where you can group the components, directives, pipes amd services which are related to the application.
app.module.ts file --> Root module.
@NgModule({
    declarations:[
        AppComponent
    ],
    imports:[
        BrowserModule,
        AppRountingModule
    ],
    providers[],
    bootstrap:[AppComponent]
})

9. How an Angular App gets Loaded and Started? What are index.html, app-root, selector and main.ts?
index.html --> Main.ts --> app.module.ts(bootstrap) --> App-component(bootstrap).
Angular is used to create Single Page Applications. 
index.html file is that single page.
index.html will invoke main.js file which is the JavaScript version of main.ts file.

main.ts file is like the entry point of web-app.
It compiles the web-apps and bootstraps the AppModule to run in the browser.

App module file will then bootstrap the Appcomponent.

App-component or app-root component is the html which you will see finally.


10. What is a Bootstrapped Module & Bootstrapped Component?
When the Angular Web application will start then the first module launched is the bootstrapped module and same is true for the bootstrapped component also.

Data Binding

11. What is Data Binding in Angular?
Data binding is the way to communicate between your typescript code of your component and your html view.
TypeScript Code(app.component.ts)        -------->      HTML Template(app.component.html)view
                                    String Interpolation, Property Binding, Event Binding, 2-way data binding.

12. What is String Interpolation in Angular?
String Interpolation is a one-way data binding technique that is used to transfer the data from TypeScript code(Component) to an HTML template(view).

String Interpolation can work on string type only not numbers or any other type.
It is represented inside{{data}} double curly braces.


13. What is Property Binding in Angular?
Property Binding is a superset of interpolation. It can do whatever interpolation can do.
In addition, it can set an element property to a non-string data value like Boolean.

14. What is Event Binding in Angular?
Event Binding is used to handle the events raised by the user actions like button click.
Ex: Submit button.

15. What is Two way Binding in Angular? combination of Property Binding and Event Binding.
Two-way data binding in Angular will help users to exchange data from the view to component and then from component to the view at the same time.

Section 4 
16. What are Directives? What are the type of directives?
Directives are classes that add additional behavior to elements in your Angular applications.
                        Types of directives
                Structural              Attribute          Component
                *ngIf                   [ngClass]           
                *ngFor                  [ngStyle]
                *ngSwitch

Structural directives change appearance of DOM by adding or removing elements.
Attribute directives change the appearance or behavior of an element.
Component directive are directives with its own template.

17. What is *ngIf Structural directive?
Structural Directives are classes that change appearance of DOM by adding or removing elements.
ngIf Directive is used to add or remove items based on the if condition.

18. What is *ngFor Structural directive?
The *ngFor directive is used to iterate a list of items and then display them.

19. What is *ngSwitch Structural directive?
ngSwitch is an Structural directive used in combination with *ngSwitchCase and *ngSwitchDefault that are both structural directives.

20. What is [ngStyle] Attribute directive?
Attribute directives change the appearance or behavior of an element.
ngStyle is an Attribute directive that updates styles for the HTML element.


21. What is [ngClass] Attribute directive?
ngClass directive adds and removes CSS Classes on an HTML element.

22. What is the difference between Component, Attribute and Structural Directives?

Component Directive
Component Directive is responsible for showing the first whole view. It is the mosed used one.
Starts with @ Sign.
Like: @Component

Structural Directive
Structural directive is responsible for adding and deleting html elements in the view.
Starts with * sign.
Like: *ngIf, *ngFor, *ngSwitch

Attribute Directive
Attribute directive is responsible for changing the appearance of view by adding or removing styles/css classes of the html elements.
Set inside square brackets. []
Like: [ngClass], [ngStyle]

Section 5 Decorator & Pipes

23.What is Decorator?
Angular decorators store metadata about a class, method, or property.
Metadata is "data that provides information about other data".
All decorators are represented with @ symbol.

24. What are the types of Decorator?
4 types
Class Decorators Ex: @NgModule, @Component

Property Decorators Ex: @Input, @Output

Method Decorators Ex: HostListner

Parameter Decorators Ex: @Inject, @Self


25. What are Pipes? What are the types of Pipes & Parameterized Pipes?
Pipes are simple functions which accept an input value and return a transformed value.

                        Angular Pipes
            Build-in Pipe                   Custom Pipe
lower-case, upper-case (conversion)
When we pass any parameters to the pipes, it is called Parameterized pipes.

26. What is Chaining Pipes?
The chaining pipes use multiple pipes on a data input. Ex: {{dob | date | uppercase}}


Section 6
27. Explain Services with Example?
A service is a typescript class and a reusable code which can be used in multiple components.
Service can be implemented with the help of Dependency Injection.

Ex: LoginComponent       MenuComponent

ErrorLoggingService

28. How to create Service in Angular? App/login/Menu Component
open terminal --> ng generate service

29. How to use Dependency Injector with Services in Angular? 3 step process.
    Register the service.
    Create the new property and assign the Service type.
    this.loggingService.logError(); 

30. What is Hierarchical Dependency Injection? Parent --> Child


31. What is Provider in  Angular?
A provider is an object declared inside the decorators which inform Angular that a particular service is available for injecting inside the components.


32. What is the role of @Injectable Decorator in a Service? How to use one service inside another service?
With @Injectable decorator one service can be used by another service.


Section 7 -Lifecycle Hooks
33. What are Parent-Child Components?
Suppose Parent Component with input field, button.
create ng g c child
ng serve
 
34.  What are Lifecycle Hooks in Angular?
A component from creation to destruction goes through several stages and these stages are life cycle hooks.
The Stages will cover activities like:
    1. Component instantiating.
    2. Rendering the component html view.
    3. Creating the Child Components(if required).
    4. Destroying the component.

constructor: It is a default method of the typescript class that is executed when the class is instantiated. 
It always run before any angular hook and it is not part of lifecycle hooks.

ngOnChanges : called when input property changes.

ngOnInit: called when the component is created.

ngDoCheck : if changes not detected then it is called.

ngAfterContentInit
ngAfterContentChecked
ngAfterViewInit
ngAfterViewChecked  ---> 4 of them are called for component children.

ngOnDestroy: called when the component is destroyed.


35. What is a Constructor in Angular?
The Constructor is a method in a Typescript class that automatically gets called when the class is being instantiated.
Constructor always run before any angular hook and it is not part of Lifecycle Hooks.
Constructor is widely used to inject dependencies(services) into the component class.

Syntax: 
export class SampleComponent implements onInit {
    constructor(){
        console.log("inside constructor");
    }
        ngOnInit():void{
            console.log("Inside ngOnInit");
        }
    }


36. What is ngOnInit life cycle hook in Angular?
1. NgOnInit signals the activation of the created component.
2. This is the second hook and called after ngOnChanges.
3. NgOnint called only once during lifecyle.
4. By default, present in the component.

37. What is the difference between constructor and ngOnInit?
ngOnInit                                                
1. NgOnInit is an Angular Lifecycle hook which signals the activation of the created component.
2. ngOnInit is called after ngOnChanges lifecycle-hook.
3. When ngOnInit called, everything about component is already ready, so it's use is to perform most of the business logic on component.

Constructor
1. The Constructor is a method in a TypeScript class, that automatically gets called when the class is being instantiated.
2. Constructor is called before any lifecycle-hook.
3. When Constructor called, everything in component is not ready, so it's mostly used for injecting dependencies only.


Section 8 Observable/ HttpClient/RxJS

38. What are Asynchronous operations?
Observables are used to perfrom Asynchronous operations and handle asynchronous data.
4Tasks run at same time.


39. What is the difference between Promise and Observable?
Observables
1. Emit multiple values over a period of time. also called streaming of data.
2. Are lazy: they're not executed until we subscribe to them using the subscribe() method.
3. Have subscriptions that are cancellable using the unSubscribe() method.

Promise
1. Emit a single value at a time.
2. Are not lazy: execute immediately after creation.
3. Are not cancellable.

40. What is RxJS?
RxJS is a library for composing asynchronous and event-based programs by using observable sequences.
RxJS is a JavaScript library, that allow us to work with asynchronous data stream with the help of Observables.
Observables introduced by RxJS Library.
RxJS stands for Reactive Extensions for JavaScript.

41. What is Observable? How to implement Observable
Observables are used to stream data to multiple components.
It's a 3 step process:
1. Import Observable from RxJS Library.
2. Create Observable & Emit Data.
3. Finally subscribe the Data.

42. What is the role of HttpClient in Angular?
HttpClient is a built-in service class available in Angular.
@angular/common/http package.
Performs HTTP requests.

Section 9 
43. What is Typescript? Or What is the difference between Typescript and Javascript?
1. Tyescript is a strongly typed language. Ex: let someValue: string="test message";
2. Tyescript is a superset of JavaScript.
3. It has Object oriented features.
4. Detect error at compile time.

44. What is the difference between let and var keyword?
Var has global scope inside function.
let keyword scope is limited to the block only, from where it is declared.

45. What is Type annotation?
Definition: Type annotation is assigning a variable or object.
a type which will show the compile time error,
if we will try to assign the variable a different type.

46. What are Built in/ Primitive and User-Defined/ Non-primitive Types in Typescript?
Built-in Data types are used to store simple data.
User-Defined Types are used to store complex data.

47. What is “any” type in Typescript?
Definition - When a value is of type any,
then no typechecking will be done by compiler and
the flexibility is there to do anything with the variable.

48. What is Enum type in Typescript?
Definition - Enums allows to define a set of named constants.

49. What is Type Assertion in Typescript?
Definition: Type assertion is a technique that informs the compiler about the type of a variable.

50. What are Arrow Functions in Typescript?
Arrow functions are the shorthand Syntax
for defining the anonymous function


=============================================================================================

Angular IQ
 
1. What is CSS Float Property?
The float property specifies how an element should float.
 
2. What is CSS Position?
The position property specifies the type of positioning method used for an element (static, relative, fixed, absolute or sticky).
 
3. HTML5 Semantic Web?
A semantic element clearly describes its meaning to both the browser and the developer.
Examples of non-semantic elements: <div> and <span> - Tells nothing about its content.
Examples of semantic elements: <form>, <table>, and <article> - Clearly defines its content.
 
4. Difference b/w local storage and session storage
Session storage is temporary which exists as long as the current window is opened and data gets lost when window 
is closed, where as Local Storage is persistant and remains intact across sessions unless anyone deletes it.
 
5.What is Javascript function?
Functions are one of the fundamental building blocks in JavaScript.
Particular business logic called as function. 
 
6.What is the scope of the variable?
Scope determines the accessibility (visibility) of variables.
 
In JavaScript there are two types of scope:
 
Local scope
Global scope
JavaScript has function scope: Each function creates a new scope.
 
Scope determines the accessibility (visibility) of these variables.
 
Variables defined inside a function are not accessible (visible) from outside the function.
 
7. What is Callback, closure?
Passing "one function" to "another function" as an argument called as "CallBack".
if any inner function accessing the outer function data, then such scenario called as closure.
 
 
8.explain crud operations in angular?
CRUD operations in Angular refer to the four basic functions for managing data: Create, Read, Update, and Delete.
Create
Creating new data involves sending a POST request to the server API. In Angular, this is typically done using the HttpClient service.


9.why we use bootstrap? explain some bootstrap class?
Bootstrap is a framework to help you design websites faster and easier. 
It includes HTML and CSS based design templates for typography, forms, buttons, tables, navigation, 
modals, image carousels, etc. It also gives you support for JavaScript plugins.  
 
10.explain directives
To enhance view capabilities or view features we go for directives. 
Types of Directives – 2 types 
Predefined Directives --- Directives given by the Angular framework 
Custom Directives --- Directives developed by users
 
11.explain routing?  Navigating from 1 component to another component is called routing. 
 
12.Events in HTMl?
HTML has the ability to let events trigger actions in a browser, like starting a JavaScript when a user clicks on an element.
 
 
13.differnce between display:block and visibility hidden?
display:none will hide the element and collapse the space is was taking up, 
whereas visibility:hidden will hide the element and preserve the elements space.
 
14.difference between var, let, const keyword?
 
                             var                                         let 
 
    1) ES1                                                          1) ES6 
    2) duplicate variables allowed                                  2) duplicate variables not allowed 
    3) won't obey scope rule                                        3) obeys scope rule 
    4) global polluting issue raised                                4) we can overcome global polluting issue
    5) variable hoisting raised                                     5) we can overcome variable hoisting  
    6) var keyword is the global scope                              6) let keyword is the block scoped member 
       member 
//const keyword 
 
//const keyword used to declare the variables 
 
//const keyword introduced in "ES6" 
 
//in const keyword "reinitialization" not possible 
  
15.types of Binding in angular?
There are four different types of ways through which we can do data bindings in Angular 2 namely 
event binding, 
unidirectional binding (i.e. one-way binding), 
bi-directional binding (i.e. two-way binding), 
and the interpolation.
 
 
16.Lifecycle hooks in Angular?
 
ngOnChanges: Called every time a data-bound input property changes. 
It’s called a first time before the ngOnInit hook. The hook receives a SimpleChanges object that contains the previous and current values for the data-bound inputs properties. This hook gets called often, so it’s a good idea to limit the amount of processing it does.
 
ngOnInit: Called once upon initialization of the component.
 
ngDoCheck: Use this hook instead of ngOnChanges for changes that Angular doesn’t detect. It gets called at every change detection cycle, so keeping what it does to a minimum is important for performance.
 
ngAfterContentInit: Called after content is projected in the component.
 
ngAfterContentChecked: Called after the projected content is checked.
 
ngAfterViewInit: Called after a component’s view or child view is initialized.
 
ngAfterViewChecked: Called after a component’s view or child view is checked.
 
ngOnDestroy: Called once when the component is destroyed and a good hook to use to cleanup and unsubscribe from observables.
 
 
 
17.differnce between promise and observable?
 
Promises Establishes the communication between "producer" and "consumer". 
       - Promises also called as "special javascript objects". 
       - we will create Promises by using "Promise" class constructor. 
        - Promises have 3 states 
            1) success  (resolve) 
            2) error    (reject) 
            3) pending 
          - we will consume promises by using "then()" 
 
a Promise is always asynchronous,
while an Observable can be either synchronous or asynchronous,
a Promise can provide a single value,
whereas an Observable is a stream of values (from 0 to multiple values), 
you can apply RxJS operators to an Observable to get a new tailored stream
 
=====================================================================================================

What is | ? 
In JavaScript, the | symbol is primarily used as the bitwise OR operator.
Pipes in Angular are a way to transform data in your template
they are simple functions that accept an input value and return a transformed value. 
Pipes are used in template expressions to modify the way data is displayed.

What is arrow function ?   Arrow functions acts like "callbacks" to receive the response from server.

React                                           Angular
Architecture: only the View of MVC              Complete MVC
Rendering: Server Side Rendering                Client-side rendering
DOM: use Virtual DOM                            uses Real DOM
Data Binding: 1-way data binding                2-way data binding
Debugging: Compile-time Debugging               Runtime debugging
Author: Facebook                                Google