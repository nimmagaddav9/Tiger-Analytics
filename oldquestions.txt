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



===========================================================================
Frontend — Angular
1. Explain how you structure a large Angular 16 project for maintainability.
I structure large Angular projects by organizing them using a modular architecture. Each feature is placed in its own module following the feature-name.module.ts convention, making the codebase scalable and easier to maintain. I follow the separation of concerns by grouping related files: components, services, models, and routing modules into their respective folders.

Shared modules are used for reusable components, directives, and pipes, while core modules are for singleton services and interceptors. This separation allows for clean dependency management and ensures clear boundaries between features.

2. What is the role of Nrwl Nx in Angular development? Have you used it in monorepo setups?
Yes, I’ve used Nrwl Nx extensively in monorepo setups. Nx plays a key role in organizing enterprise-scale Angular applications by enabling dependency graphs, code sharing, and enforcing boundaries between applications and libraries.

With Nx, we can maintain multiple Angular apps and shared libraries (UI, models, utilities, etc.) in a single monorepo. It improves build times through affected-only builds, facilitates CI/CD with better caching, and integrates well with Storybook and Jest for testing.

3. What is your approach to lazy loading modules in Angular?
I use Angular’s built-in lazy loading via the loadChildren property in route configuration. Each feature module is lazy-loaded using dynamic imports, ensuring that the initial bundle size remains small and the app loads faster.

I also use route guards where necessary and preload certain critical modules using Angular’s PreloadAllModules strategy. For performance monitoring, I track lazy-load timing via analytics to optimize the user experience.

4. How do you manage state in Angular? Compare services vs NgRx or other patterns you've used.
I typically start with Angular services and BehaviorSubject for simpler apps. As the app grows and state becomes complex across multiple components or modules, I prefer using NgRx for scalable state management.

NgRx offers a predictable unidirectional data flow, with actions, reducers, and effects making the state management clear and testable. It also integrates well with the Redux dev tools for debugging. For mid-sized apps, I’ve used Akita or component-store for a lighter alternative to NgRx.

5. Have you worked with AG Grid? How did you customize it for large data sets?
Yes, I’ve used AG Grid in Angular apps for high-performance tabular data. For large datasets, I enabled server-side row model to fetch data in chunks. I implemented infinite scrolling, pagination, and sorting/filtering on the server.

I also customized AG Grid themes with SASS, created cell renderers for complex UI, and used dynamic column definitions. Performance-wise, I ensured virtual DOM rendering and memoization where needed.

6. What is the benefit of using SASS over plain CSS, and how do you structure your stylesheets in a component-based architecture?
SASS provides features like variables, nesting, mixins, and functions, which are invaluable for maintaining a large UI codebase. It promotes DRY principles and modular styling.

In Angular, I use component-scoped styles (.component.scss) and maintain global variables, mixins, and utility classes in a shared styles folder. I follow a BEM-style naming convention and avoid deep nesting to keep styles readable.

🔹 Backend — Node.js / NestJS / GraphQL
7. How do you design scalable REST or GraphQL APIs in Node.js/NestJS?
I use NestJS for scalable API design due to its modular architecture and built-in support for decorators, DI, and middlewares. I separate concerns using modules, controllers, services, and DTOs. I use middleware for logging and validation pipes for input sanitization.

For GraphQL, I use schema-first or code-first approaches depending on the use case. I utilize resolvers for field-level logic and leverage tools like Apollo Server for performance and introspection.

8. Can you explain the concept of a bounded context in API modeling?
A bounded context refers to the clear definition of responsibilities and scope within a service or domain. In API design, it ensures that a specific service (like fund-management or user-profile) owns its own data and logic.

I’ve used this in microservices to avoid tight coupling, by keeping APIs self-contained and integrating using events or API gateways. This supports scalability and maintainability in distributed systems.

9. Describe your experience with AWS Lambda and API Gateway.
I’ve built and deployed serverless APIs using AWS Lambda and API Gateway. For example, I created a microservice to process portfolio analytics which would ingest fund data and perform calculations asynchronously.

I used API Gateway to expose these Lambda functions securely, implemented custom authorizers, and leveraged throttling and usage plans for consumer control. I also integrated these with DynamoDB and S3 for storage.

10. What is the difference between REST and GraphQL, and when would you choose one over the other?
REST provides fixed endpoints and is easier to cache, while GraphQL offers flexibility by allowing clients to query exactly what they need.

I prefer REST for simple CRUD operations and internal services. For complex UIs where over-fetching is a concern — such as fund comparison or analytics dashboards — I choose GraphQL for its efficiency and developer experience.

11. What tools or techniques do you use for functional and performance testing of your APIs?
I use Postman for manual functional testing and Newman for automated test suites. For performance testing, I use Artillery and JMeter to simulate load and track latency, throughput, and error rates.

I also write Jest-based unit and integration tests in NestJS and use Swagger to document and test API contracts.

🔹 AWS & Observability
12. Which AWS services have you used in production? Describe a real-world solution you built using them.
I’ve used Lambda, API Gateway, S3, DynamoDB, CloudFront, and ECS Fargate in production. For example, I built a serverless backend for a portfolio analytics dashboard using Lambda + DynamoDB + API Gateway. S3 served the UI assets via CloudFront.

I configured cost tagging, monitoring, and alarms via CloudWatch to keep the stack resilient and observable.

13. Have you used ECS Fargate? Can you walk us through your container deployment pipeline?
Yes, I’ve used ECS Fargate to deploy containerized Node.js services. The pipeline used GitHub Actions to build and push Docker images to ECR. Then, using CloudFormation templates or Terraform, we deployed to ECS Fargate with autoscaling policies.

I also used service discovery and ALB for routing, and parameter store for secure config management.

14. What strategies have you used for cost-tagging and monitoring AWS usage?
I applied resource-level tagging (e.g., Project, Environment, Owner) across all AWS services. I used AWS Budgets and Cost Explorer to track and alert on anomalies.

We also used CloudHealth to generate reports by project/team and implemented lifecycle policies on S3 to reduce storage costs.

15. What observability tools have you used (e.g., Splunk, UiPath, CloudWatch)? How did you set up alerts for production systems?
I’ve used CloudWatch for logs and metrics, setting up dashboards and alarms for CPU, memory, and error rates. I also used Splunk for deeper log analysis and alerting based on custom queries.

For example, I configured Lambda error rates and DynamoDB throttles to trigger SNS alerts and PagerDuty incidents.

16. How do you ensure your microservices are observable and maintain proper health metrics?
I ensure observability by:

Adding structured logging and trace IDs

Exposing health check endpoints (/healthz, /readyz)

Instrumenting metrics with CloudWatch or Prometheus

Using OpenTelemetry for distributed tracing in larger systems

🔹 Bonus / Wrap-Up
17. How do you stay up-to-date with frontend and full-stack trends?
I regularly follow platforms like Dev.to, Medium, and Hacker News. I also take courses on Pluralsight and Udemy, subscribe to Angular and AWS newsletters, and actively contribute to developer communities on GitHub and LinkedIn.

18. What interests you most about this role and working in the investment industry domain?
I’m excited about the opportunity to modernize applications that impact international investments. Building tools like portfolio analytics and fund comparison has meaningful real-world value. The scale, performance, and security needs in this domain challenge me to build better systems and continuously improve.

19. Do you have any questions for us?
How is success measured for this role in the first 6 months?

Can you share more about the current architecture and team structure?

What are the biggest technical challenges the team is currently facing?


========================

Previous Interview question and answers

1. Tell me about yourself and your journey into front-end development.

I am a core UI Developer with 12+ years of experience building .com websites for different organizations using HTML5, CSS3, JavaScript, Angular 18, React.js, and Redux.
In the past 2 years, I worked on the React migration team, where I converted the .net pages to react on united.com.
Frontend is React, and used ATMOS (Own library) components used company wide.

Worked on Security features for users where they can manage there account like Forgot password, Forgot MileagePlus number,
security questions, Sign-in features, Miles-Pooling, United Club pass, Recent Activity, dashboard updates and
KTN(Known Traveler Number), Accessibility guidelines features on united.com.

used middleware such as redux-saga to handle asynchronous tasks such as API calls, data fetching, and impure actions in a more organized and efficient way.

Previously worked with Accelerator team for Visa Inc. remediation of MBDA modules like Application Management, Account Management, Portfolio Management, Analytics, Recurring billing, Virtual Terminal, etc for bank users like Wells Fargo, Bank of America, etc

Capital Group worked on DAVIS Project. Davis stands for Data visualization where we build different highcharts using react and integrate into the AEM., the backend is Java. Previously I worked on Creative Workbench, a writing tool where articles are published on capital group websites.

At Cerner Corporation worked on the medical examination forms.

In Office Depot worked on black Friday reporting.

Satinos Technologies created a tax portal and a schoomin website for the Vignan schools.

2. Walk me through your latest project – what problems did you solve?

React migration - Converted pages in .net to react.
The new initiative worked on Miles-Pooling( points you get after traveling), TSA Precheck, Account security and management features, and Under18.

3. How does the virtual DOM work in React?

Suppose line of code is changed , processing is done on particular line.
It will process the whole code in real DOM. Virtual DOM is faster.

4. What’s the difference between props and state in React?

Props (short for "properties") are read-only and passed from a parent component to a child component.
They allow components to communicate by passing data down the component tree.
Since props are immutable within the receiving component, they cannot be changed by the component itself.

State, on the other hand, is mutable and managed within a component.
It represents data that can change over time due to user interactions or other factors.
A component's state can be updated using React's useState hook (in functional components) or
setState (in class components), causing the component to re-render.

5. What is useEffect and how have you used it in your projects?

In React, useEffect is a hook that allows you to perform side effects in functional components.
Side effects include things like fetching data, updating the DOM, setting up subscriptions, and cleaning up resources.

How useEffect Works:
useEffect runs after the component renders.

It can be configured to run only once, on every render, or when specific values change.

You can return a function inside useEffect to clean up resources (like removing event listeners or unsubscribing from an API).

<!-- import { useEffect, useState } from "react";

function ExampleComponent() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    console.log(`Count changed to ${count}`);

    return () => {
      console.log("Cleanup before next useEffect runs or component unmounts");
    };
  }, [count]); // Runs whenever "count" changes

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
} -->

How I've Used useEffect in Projects:
Fetching Data: I’ve used useEffect to fetch API data when a component mounts ([] as the dependency array).

Listening to Window Events: Tracking things like window resizing or scroll position changes.

Setting Up Timers: Managing intervals and timeouts for features like countdown timers.

Cleaning Up Resources: Removing event listeners or stopping subscriptions when a component unmounts.

6. How do you manage API calls and error handling in React?

Ans: 1. Using Fetch or Axios for API Calls
You can make API requests using fetch or axios. Axios provides some extra features like automatic JSON parsing
and request cancellation.

    2. Using Axios for Cleaner Code
    3. Handling Errors Gracefully
    4. Using useEffect for API Calls
    5. Avoiding Memory Leaks

7. What’s the folder structure you prefer for a scalable front-end project?

A well-organized folder structure is crucial for scalability, maintainability, and readability in a front-end project. Here’s the structure I usually recommend for React-based projects (but it applies to other frameworks as well):

/project-root
├── public/ # Static assets (favicon, index.html)
├── src/ # Main source code
│ ├── assets/ # Images, fonts, global styles
│ ├── components/ # Reusable UI components
│ ├── pages/ # Individual pages/views
│ ├── hooks/ # Custom React hooks
│ ├── utils/ # Utility/helper functions
│ ├── services/ # API calls, authentication logic
│ ├── contexts/ # Global state management (Context API)
│ ├── styles/ # Global styles or component-specific styles
│ ├── store/ # State management (Redux, Zustand, etc.)
│ ├── config/ # Environment variables, app settings
│ ├── routes/ # Centralized route definitions
│ ├── tests/ # Unit & integration tests
│ ├── index.tsx # App entry point
│ ├── App.tsx # Root component
├── .env # Environment variables
├── package.json # Dependencies & scripts
├── tsconfig.json # TypeScript config (if using TypeScript)
├── README.md # Documentation

8. What is the role of Express.js in the MERN stack?

Express.js plays a crucial role in the MERN stack by acting as the backend framework that connects the front end (React) with the database (MongoDB) via Node.js.. Here's how it fits into the stack:

🚀 Role of Express.js in MERN:

1. Handles HTTP Requests & Routes

Express.js provides a simple and flexible way to define API routes (GET, POST, PUT, DELETE) that interact with the MongoDB database.

2. Middleware Integration

It allows middleware functions that handle authentication, logging, error handling, and request parsing (like body-parser).

3. Database Connectivity

Express.js interacts with MongoDB (usually via Mongoose) to perform CRUD operations efficiently.

4. Server-Side Logic & Business Rules

This is where backend logic is implemented—handling authentication, form validation, and access control.

5. API Development for Frontend Communication

The React front end makes API calls to Express.js, which then fetches or modifies data in MongoDB.

9. How do you optimize performance in a React app?

1. Memoization with useMemo and useCallback: Use this hooks to memoize values and, reducing unnecessary recalculations.
1. Optimizing Renders with React.Fragment: Use it to avoid unnecessary wrapper elements that could cause additional DOM nodes.
1. Lazy loading with React.lazy: Use it to load components lazily, reducing the intial bundle size and imporving intial loading performance.
1. Code splitting: Employ code splitting to divide your application into smaller chunks that are loaded on demand, improving initial load times.
1. Optimizing Images and Assets: Compress and optimize images, use responsive images and leverage lazy loading for images to reduce network and rendering overhead.

1. Difference Between Flex and Grid
• Flexbox (Flex):
○ One-dimensional layout: Arranges elements in a row or column.
○ Ideal for simple layouts with horizontal or vertical alignment.
○ Responsive: Easily adapts to different screen sizes.
○ Great for navigation bars, footers, and single-dimensional content sections.
• CSS Grid (Grid):
○ Two-dimensional layout: Creates rows and columns for complex layouts.
○ Superior for intricate structures with precise positioning.
○ Responsive: Maintains flexibility across devices.
○ Perfect for dashboards, product listings, and multi-column layouts.
Visual Demonstration:
• Flex: Show a navigation bar with elements aligned horizontally.
• Grid: Display a product listing with items arranged in rows and columns.
Choosing Between Flex and Grid:
• For simple layouts or single-dimensional alignment, flexbox often suffices.
• For complex structures with precise positioning, opt for grid.
• They can even be combined for more versatile layouts.
Example (Code Snippet):
JavaScript
// Flexbox for a navigation bar
<nav style={{ display: 'flex', justifyContent: 'space-between' }}>
  <a href="#">Home</a>
  <a href="#">About</a>
  <a href="#">Contact</a>
</nav>
// Grid for a product listing
<div style={{ display: 'grid', gridTemplateColumns: 'repeat(auto-fit, minmax(200px, 1fr))' }}>
  <div className="product">Product 1</div>
  <div className="product">Product 2</div>
  {/* More products... */}
</div>

1. getElementById vs. getElementByClass
   • getElementById:
   ○ Retrieves an element by its unique ID.
   ○ Faster when you know the exact ID.
   ○ Use for elements that should only appear once.
   • getElementsByClassName:
   ○ Returns an array of elements with the same class name.
   ○ Useful when you have multiple elements with the same class.
   ○ Can be less performant for large numbers of elements.
   Choosing Between getElementById and getElementByClass:
   • Use getElementById for elements with a unique ID.
   • Use getElementsByClassName for multiple elements with the same class.
   Example (Code Snippet):
   JavaScript
   const heading = document.getElementById('main-heading'); // Use for unique ID
   const buttons = document.getElementsByClassName('btn'); // Use for multiple buttons
   Use code with caution.

1. What are ES6 Features ?


    • Arrow Functions: Concise syntax for defining functions.

JavaScript
const greet = name => `Hello, ${name}!`;

    • Template Literals: Embedded expressions within strings for dynamic content.

JavaScript
const message = `Welcome, ${user.name}`;

    • Destructuring: Extract properties from objects or arrays.

JavaScript
const { firstName, lastName } = user;

    • Classes: Object-oriented programming with inheritance.

JavaScript
class Person {
constructor(name) {
this.name = name;
}

greet() {
console.log(`Hello, I'm ${this.name}`);
}
}

    • Modules: Organize code in reusable modules.

JavaScript
// myModule.js
export function add(a, b) {
return a + b;
}

// main.js
import { add } from './myModule.js';
console.log(add(2, 3));

13. What are promises ?


    • Promises: Represent the eventual completion (or failure) of an asynchronous operation.
    • Benefits:
    	○ Improved code readability and maintainability by handling asynchronous operations asynchronously.
    	○ Chaining of asynchronous operations for a more fluid flow.
    	○ Error handling for potential issues during asynchronous execution.

Code Example (Using Fetch API):
JavaScript
fetch('https://api.example.com/data')
.then(response => response.json())
.then(data => {
console.log(data);
// Process the data
})
.catch(error => {
console.error(error);
// Handle errors
});

14. Redux is a state management library for JavaScript applications, including React. It provides a centralized store to hold application state, actions to update that state, and reducers to handle those updates.
    • Store: Holds the entire application state as a single JavaScript object tree.
    • Actions: Plain JavaScript objects describing the intention to change the state.
    • Reducers: Pure functions that accept the current state and an action, returning the new state.
    Dispatcher.
    Pros of Redux:
    • Predictable State Management: Easier to reason about application state and track changes.
    • Improved Testability: Easier to test components in isolation due to centralized state.
    • Scalability: Well-suited for large and complex applications.
    Cons of Redux:
    • Boilerplate Code: Requires setting up stores, reducers, actions, and middleware.
    • Complexity: Learning curve for managing state with reducers and actions.

15. Why Fetch Inside useEffect?
16. We typically fetch data inside useEffect in React because it ensures
    the data is fetched only when the component is mounted (or when
    dependencies in the array change).
17. This prevents unnecessary re-renders on every update and improves performance.
18. Additionally, useEffect allows for easy cleanup of side effects
    like subscriptions when the component unmounts.

19. What are props in Reactjs ?

Building Blocks of Communication
Imagine building Lego houses. Each Lego piece has properties that
define its color, size, and shape. Similarly, in React, props are
properties passed down from parent components to child components.
They act as a way for components to communicate and share data.
This allows you to create reusable and dynamic components!

17. What are different Component Types:

React offers two main types of components:

Class Components: These are like blueprints defining how a
component behaves and renders. They use the class keyword and
allow for functionalities like state management and lifecycle methods.
Structured way.

Functional Components: These are simpler and more concise.
They are pure functions that take props as input and return JSX
to describe what the component renders. They're a great choice
for presentational components.

18. What are states in ReactJS ?

Think of state as the internal memory of a component.
It allows components to react to user interactions or data changes.
You can use the useState hook to manage state in functional components.

19. What are stateless components in react ?

Stateless components, essentially functional components,
don't manage internal state. They simply take props as
input and return JSX based on those props. This makes
them lightweight and easier to reason about.

Example of a Stateless Component:

function Greeting(props) {
return (
<div>
<h1>Hello, {props.name}!</h1>
</div>
);
}

20. What are arrow functions in JS ?

Arrow functions (introduced in ES6) are a
concise way to write JavaScript functions.
They're often preferred for their cleaner syntax,
especially when dealing with props and state in React components.

Example of an Arrow Function:
JavaScript

const handleClick = () => {
console.log('Button clicked!');
};
handleClick()

21. What is redux ? and when to use it ?

Redux (although not strictly required for basic React applications)
is a popular state management library for managing complex application
state. It provides a centralized store to hold your application's state,
actions to update that state, and reducers to handle those updates.
(Think of it as a central bank for your app's data!)

22. What is JSX is reactjs ?

JSX (JavaScript XML) is a syntax extension that allows you to write
HTML-like structures within your JavaScript code. This makes
it easier to visualize and build user interfaces in React components.

Example of JSX:

return (

  <div>
    <h1>Welcome to My App</h1>
    <p>This is some content.</p>
  </div>
);

23. What is strict mode in JS

React's Strict Mode is a development tool that helps identify potential
issues in your application code. It enables warnings for deprecated
features, lifecycle methods, and other potential problems,
allowing you to catch them early during development.

---

HTML Interview questions

1. HTML5 new features vs HTML4?

Major New Features in HTML5:

Semantic tags: <article>, <section>, <header>, <footer>, <nav>, <main>, etc., for clearer document structure and better SEO.

Multimedia: <audio> and <video> tags allow native embedding of media without third-party plugins.

Graphics: <canvas> for 2D drawing and animation, plus improved SVG support.

Form controls: New input types (email, date, color, etc.), validation, and attributes like placeholder, required, and autofocus.

APIs: Geolocation, offline storage (local/session storage), drag-and-drop, Web Workers for background processing, and WebSockets for real-time communication.

Simplified syntax: Easier doctype and cleaner markup.

Improved accessibility and SEO: Semantic elements help search engines and assistive technologies understand content structure.

2. Storage in HTML?

1. Local Storage (localStorage)

Stores data permanently until manually cleared.

Data is saved across page reloads and browser sessions.

Example:
localStorage.setItem("username", "Vijay");
console.log(localStorage.getItem("username")); // Output: Vijay

2. Session Storage (sessionStorage)

Stores data temporarily (only until the browser tab is closed).

Example:
sessionStorage.setItem("theme", "dark");
console.log(sessionStorage.getItem("theme")); // Output: dark

3. Cookies (document.cookie)

Used for small amounts of data, typically for tracking user sessions.

Sent to the server with each request.

Example:
document.cookie = "username=Vijay; expires=Fri, 31 Dec 2025 23:59:59 GMT";

4. IndexedDB

A powerful NoSQL database inside the browser.

Supports complex data storage, including objects.

Example:

let db;
const request = indexedDB.open("myDatabase", 1);
request.onsuccess = () => { db = request.result; console.log("Database opened successfully"); };

5. Cache API (Service Workers)

Used for storing resources like files, images, and responses for offline use.

Works well for Progressive Web Apps (PWAs).

Example:
caches.open("my-cache").then(cache => {
  cache.add("/index.html");
});



3. iframe HTML

<iframe>, short for inline frame, is an HTML element that lets you embed another document (webpage, video, map, etc.) 
inside the current webpage.

🚀 How <iframe> Works
An <iframe> allows you to load external content within a designated area on your site.

<iframe src="https://example.com" width="600" height="400"></iframe>

✅ Common Use Cases
Embedding YouTube videos, Google Maps, or third-party widgets.

Loading external pages without redirecting users.

Displaying ads or content from other sources.


4. HTML5 features

Semantic Elements

New elements like <section>, <article>, <header>, <footer>, and <nav> improve the structure and readability of web pages.

Multimedia Support

Native <audio> and <video> elements let you embed media without requiring third-party plugins like Flash.

Why HTML5 is Better?
✅ Eliminates dependency on external plugins 
✅ Enhances performance and SEO 
✅ Optimized for mobile-friendly websites 
✅ Enables interactive web applications


5. which video type support HTML5

✅ MP4 – Best for maximum compatibility across all browsers. 
✅ WebM – Optimized for the web with good compression and fast loading. 
✅ Ogg – Open-source, but less widely supported compared to MP4 and WebM.


6. Maximum heading tag size?
In HTML, heading tags range from <h1> to <h6>, with <h1> being the largest and <h6> being the smallest by default.


7. marque tag?
The <marquee> tag in HTML was used to create scrolling text or moving elements across a webpage. 
However, it's now deprecated and no longer recommended for use.

<marquee behavior="scroll" direction="left">This is moving text!</marquee>


8. DOM?
The DOM (Document Object Model) is a programming interface for web documents that represents the structure of an HTML or 
XML document as a tree-like hierarchy. 
It allows JavaScript to dynamically manipulate content, structure, and styles on a webpage.

🚀 Key Features of DOM

✅ Tree Structure Representation

The DOM represents an HTML page as a tree, where elements like <html>, <body>, and <div> are nodes.

✅ Dynamic Content Manipulation

Developers can use JavaScript to add, remove, and modify elements dynamically.

✅ Event Handling

The DOM enables event-driven programming, allowing interactions through events like clicks, key presses, and hovers.

✅ Cross-Browser Compatibility

Works across different browsers, ensuring uniform behavior of web pages.



9. CSS integrate type in React.js? external (index.css), internal, inline css

✅ Inline Styles – Uses JavaScript objects for styling. 
✅ CSS Stylesheets – Imports regular CSS files. 
✅ CSS Modules – Scoped styles to avoid global conflicts. 
✅ Styled Components – CSS-in-JS for dynamic styling. 
✅ Tailwind CSS – Utility-first approach with predefined classes.

React and JS Interview questions:

1. what is shouldComponentUpdate?

shouldComponentUpdate() is used to optimize performance by preventing unnecessary re-renders. 
It returns true (default) to allow rendering or false to block it.

Ex: 
shouldComponentUpdate(nextProps, nextState) {
  return nextProps.value !== this.props.value; // Only update if "value" changes
}

✅ Helps with performance optimization 
✅ Mainly used in class components (functional components use React.memo) 
✅ Not required unless optimizing complex UI updates

2. pure component?

A Pure Component in React is a class component that automatically implements shouldComponentUpdate() with a shallow prop 
and state comparison to prevent unnecessary re-renders.

Ex: import React, { PureComponent } from "react";

class MyComponent extends PureComponent {
  render() {
    return <h1>Hello, Pure Component!</h1>;
  }
}


3. Local Storage (syntax) vs session storage vs cookies


Syntax Examples
1️⃣ Local Storage (Stores data permanently)

localStorage.setItem("username", "Vijay"); // Set item
console.log(localStorage.getItem("username")); // Get item
localStorage.removeItem("username"); // Remove item

2️⃣ Session Storage (Clears when tab is closed)
sessionStorage.setItem("theme", "dark"); // Set item
console.log(sessionStorage.getItem("theme")); // Get item
sessionStorage.clear(); // Clear all items

3️⃣ Cookies (Stores small data, sent with HTTP requests)
document.cookie = "username=Vijay; expires=Fri, 31 Dec 2025 23:59:59 GMT; path=/";
console.log(document.cookie); // Get all cookies


4. size of local storage
The size limit for Local Storage in most modern browsers is around 5MB per domain. 
This means each website can store up to 5MB of data in Local Storage.

5. context in react js syntax?
In React.js, Context API allows you to manage global state without passing props manually at every level.

🚀 Syntax Example
1️⃣ Create Context:
const MyContext = React.createContext();
2️⃣ Provide Context:
<MyContext.Provider value={sharedData}>
  <ChildComponent />
</MyContext.Provider>

3️⃣ Consume Context:
const value = useContext(MyContext);

✅ Helps avoid prop drilling 
✅ Ideal for theme, authentication, and global state 
❌ Not a replacement for complex state management like Redux

6. es6 features

ES6 introduced powerful features for modern JavaScript development: 
✅ let & const – Block-scoped variable declarations. 
✅ Arrow functions – Shorter function syntax (()=>{}).
✅ Template literals – ${variable} inside backticks for dynamic strings. 
✅ Destructuring – Easy extraction of object/array properties. 
✅ Spread & Rest (...) – Expands or collects elements flexibly. 
✅ Default parameters – Assign default values in functions. 
✅ Classes – Simplified object-oriented programming. 
✅ Modules (import/export) – Enables modular code structure. 
✅ Promises – Handles asynchronous operations (then/catch). 
✅ Map & Set – New data structures for unique values and fast lookups.



7. why we use promises?

We use Promises in JavaScript to handle asynchronous operations efficiently. 
They help avoid callback hell and make code more readable by using .then() and .catch() for handling success and errors.

✅ Improves readability – Avoids nested callbacks 
✅ Handles async operations – Fetch API, database queries, timers 
✅ Error handling – .catch() method simplifies error management 
✅ Chaining support – .then() allows sequential execution

Ex:
fetch("https://api.example.com/data")
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error("Error:", error));


8. virtual DOM?

The Virtual DOM is a lightweight copy of the actual DOM that React uses to improve performance.

✅ Fast Updates – React updates the Virtual DOM first, then efficiently syncs with the real DOM. 
✅ Minimizes Re-renders – Uses diffing to update only necessary elements, avoiding full page refreshes. 
✅ Enhances Performance – Reduces direct manipulations of the real DOM, improving speed.

Example process: 
1️⃣ React updates Virtual DOM. 
2️⃣ It compares changes (diffing). 
3️⃣ Only necessary updates are applied to the real DOM.

9. props drilling?

Props drilling occurs when data (props) is passed deeply through multiple nested components in React, even when some components don’t need it.

✅ Problem: Makes code harder to manage in large applications. 
✅ Solution: Use Context API or state management (Redux, Zustand, etc.) to avoid unnecessary prop passing.


10. webpacks uses why? 

Webpack is a powerful JavaScript module bundler used to optimize and manage assets in web applications.

✅ Bundles & Minifies – Combines multiple files into one, reducing load time. 
✅ Code Splitting – Loads only necessary code for better performance. 
✅ Asset Management – Handles CSS, images, and fonts efficiently. 
✅ Hot Module Replacement – Allows real-time updates during development. 
✅ Tree Shaking – Removes unused code for a smaller bundle size.


11. without npm project will run?

Yes, a JavaScript project can run without npm, but it depends on how dependencies are managed.

🔥 Explanation:
Pure JavaScript Projects (Vanilla JS) can run without npm if dependencies are manually included via CDN or local files.

Node.js Applications may require npm for package management, but can use manual installation or alternative package managers like Yarn or PNPM.

React, Vue, or Angular Projects typically rely on npm for dependencies and won't run properly without a package manager.


12. how to start rendering in react.js project

🚀 Basic Steps to Start Rendering
✅ Import React and ReactDOM:
import React from "react";
import ReactDOM from "react-dom";
import App from "./App";


✅ Use ReactDOM.createRoot() (React 18+):
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<App />);

✅ Ensure the root div exists in index.html:
<div id="root"></div>

This initializes the React app and renders the App component inside the root element.

13. how react code will get executed?

React code executes in the following steps:

✅ JSX Compilation – JSX is transformed into JavaScript using Babel. 
✅ Component Rendering – React creates the Virtual DOM. 
✅ Reconciliation – React compares Virtual DOM changes with the real DOM. 
✅ DOM Updates – React efficiently updates only necessary elements. 
✅ Event Handling – React listens for user interactions via synthetic events.


14. how to achieve optimization? 

React.js optimization can be achieved through several techniques:

✅ Use React.memo – Prevents unnecessary re-renders for functional components. 
✅ Use useCallback & useMemo – Optimizes function and value memoization. 
✅ Code Splitting – Load only required components using React.lazy & Suspense. 
✅ Avoid unnecessary state updates – Keep components minimal and optimize re-renders. 
✅ Virtualization – Improve performance for large lists with react-window. 
✅ Efficient rendering – Use key props correctly to avoid unwanted re-renders. 
✅ Avoid props drilling – Use Context API or Redux for state management.


15. difference between normal reducer and useReducer

✅ Normal Reducer – A function that manages state updates, typically used in Redux for global state management. 
✅ useReducer – A React hook that manages local component state using a reducer function, useful for complex state logic inside components.

Key Differences:

Normal Reducer works globally via Redux, while useReducer is for local component state.

useReducer is a React Hook, does not require Redux setup.

Redux Reducers use dispatch(actions), while useReducer relies on dispatch within the component.


16. class vs className

In HTML, class is an attribute used to define a CSS class for styling elements. 
In React (JSX), className is used instead of class, because class is a reserved keyword in JavaScript.

✅ HTML Example:
<div class="container">Hello</div>

✅ React Example:
<div className="container">Hello</div>


17. React Native

React Native is a framework for building mobile applications using React and JavaScript.

✅ Cross-platform – Develop once, run on both iOS & Android. 
✅ Uses JavaScript & JSX – Write mobile apps using familiar React syntax. 
✅ Native Performance – Renders UI components using native platform APIs. 
✅ Reusable Components – Share code between mobile and web applications. 
✅ Popular for mobile development – Used by apps like Instagram, Facebook, and Airbnb.

18. how many ways there to create react native app

You can create a React Native app in three main ways:

✅ Expo CLI – Easiest way, requires minimal setup (npx create-expo-app myApp). 
✅ React Native CLI – More customizable, allows direct access to native code (npx react-native init myApp). 
✅ Third-party tools – Tools like Ignite or ReNative for advanced setups.

19. redux saga (put, call, every)

Redux Saga is a middleware for handling side effects (like async API calls) in Redux using generator functions.

✅ put() – Dispatches an action to the Redux store. 
✅ call() – Calls a function (like an API request) and waits for the result. 
✅ takeEvery() – Listens for every occurrence of an action and runs a saga.

Example:
function* fetchDataSaga() {
  const data = yield call(api.getData);
  yield put({ type: "DATA_SUCCESS", payload: data });
}

function* watchFetchData() {
  yield takeEvery("FETCH_DATA", fetchDataSaga);
}


20. redux without api call

✅ Yes! Redux can manage state without API calls.

🚀 Use Cases Without API Calls:

UI State Management – Toggle dark mode, modal visibility.

Local Data Handling – Manage form inputs across components.

Client-Side Caching – Store temporary data for better performance.

Static Data Flow – Predefined data for UI updates.

Example without API calls:

const initialState = { count: 0 };

function counterReducer(state = initialState, action) {
  if (action.type === "INCREMENT") {
    return { count: state.count + 1 };
  }
  return state;
}


21. What is HOC? purpose?

A Higher-Order Component (HOC) in React is a function that takes a component as input and returns a new enhanced component.

✅ Purpose:

Code reusability – Share logic across multiple components.

Enhance components – Add additional functionality without modifying the original.

Example: Wrapping a component with authentication logic.

🚀 Example of HOC:

const withAuth = (Component) => (props) =>
  props.isAuthenticated ? <Component {...props} /> : <p>Please login</p>;


22. sort array without sort method, let arr = [1,5,7,2,3]

You can sort an array without using the sort() method by implementing a sorting algorithm manually, such as Bubble Sort or Insertion Sort.

🚀 Example: Bubble Sort
function bubbleSort(arr) {
  let n = arr.length;
  for (let i = 0; i < n - 1; i++) {
    for (let j = 0; j < n - i - 1; j++) {
      if (arr[j] > arr[j + 1]) {
        [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]]; // Swap values
      }
    }
  }
  return arr;
}

let arr = [1, 5, 7, 2, 3];
console.log(bubbleSort(arr)); // Output: [1, 2, 3, 5, 7]


23. closure? example
A closure in JavaScript is a function that remembers the variables from its outer scope even after the outer function has executed.

🔥 Example Closure Function
function outerFunction(x) {
  return function innerFunction(y) {
    return x + y; // `innerFunction` remembers `x` from `outerFunction`
  };
}

const add5 = outerFunction(5); 
console.log(add5(3)); // Output: 8

✅ Closure retains access to x even after outerFunction finishes. 
✅ Useful for encapsulation, maintaining private variables, and function factories.


24. let, var, const difference
In JavaScript, let, var, and const are used for variable declarations, but they differ in scope, mutability, and hoisting:

✅ var – Function-scoped, can be redeclared and updated, hoisted but uninitialized. 
✅ let – Block-scoped, cannot be redeclared, but can be updated, hoisted but uninitialized. 
✅ const – Block-scoped, cannot be reassigned or redeclared, must be initialized.

Ex: 
var a = 10; // Function-scoped
let b = 20; // Block-scoped
const c = 30; // Block-scoped, immutable

25. What is Hoisting?

Hoisting in JavaScript is the process where variable and function declarations are moved to the top of their scope before execution.

✅ Function hoisting – Allows calling a function before its declaration. 
✅ Variable hoisting – var is hoisted but initialized as undefined,
while let & const are hoisted but not initialized (cause errors if accessed before declaration).

temporal dead zone: it is zone where it belong.

26. function test(){
  var x = 10;
  var x;
  var x = 40;
  console.log("x is" + x);
}

test();
40

27. Explain the scope of temporal dead zone?
{
  //TDX starts
  const func = () => console.log(letVar);
  // TDZ
  let letVar = 3; // end TDZ
  func();
}

28. why var hoisiting is present in javascript?
var hoisting is present in JavaScript due to its interpreted nature and execution model.

🚀 Reasons for var Hoisting: 
✅ Historical Design Choice – JavaScript was originally designed for quick scripting, and var hoisting made it more flexible. 
✅ Function Execution Flexibility – Allows variables to be declared anywhere within a function but still accessible at the top. 
✅ Compilation Phase Handling – During execution, JavaScript hoists declarations (moves them to the top of their scope) before executing code.

29. Pure functions: Those functions that are deterministic in nature.

function areaofRectangle(length, width){
  return length * width;
}

areaofRectangle(10,20);
areaofRectangle(10,20);
areaofRectangle(10,30);
areaofRectangle(40,20);

30. Impure functions - those functions that are non-determinstic in nature.

function test(length, width){
  const temp = Math.floor(Math.random() * 10);
  return length * width * temp;
}
test(10, 20);

31. what is console.log('hello world') ; //logging , debugging.

console.log() is function.

32. shallow copy:  copy by reference

deep copy: copy by value

33. A shallow copy duplicates only the reference to nested objects, meaning changes to the copy affect the original. 
A deep copy creates an independent copy of all nested objects, ensuring no link to the original data.

🚀 Example in JavaScript: ✅ Shallow Copy (using Object.assign() or spread operator ...)
const obj1 = { name: "Vijay", details: { age: 30 } };
const shallowCopy = { ...obj1 }; 
shallowCopy.details.age = 35; 
console.log(obj1.details.age); // ❌ Changes original object (shallow copy)


✅ Deep Copy (using JSON.parse(JSON.stringify()) or structuredClone)

const obj2 = { name: "Vijay", details: { age: 30 } };
const deepCopy = JSON.parse(JSON.stringify(obj2)); 
deepCopy.details.age = 35; 
console.log(obj2.details.age); // ✅ Original remains unchanged (deep copy)


================================================

34. Can you provide an example of a complex React.js project you worked on and explain your role in its development?

In a recent project, I played a significant role in developing a complex React.js feature for a flight ticket booking system. 
One of the challenges involved resolving issues related to account setup. 
To tackle this, I utilized Postman to interact with multiple APIs and successfully unlock accounts, ensuring smooth user experience. 
I also documented this process for team reference, promoting efficiency and collaboration. Moreover, I have experience in managing weekly releases,
effectively addressing any backend blockers to maintain a seamless UI. 
his hands-on experience in addressing complex challenges showcases my ability to contribute effectively to React.js projects.

35. How do you ensure the scalability and performance optimization of React.js applications you work on?

In my React.js development work, I prioritize scalability and performance optimization by leveraging important tools and techniques. 
For instance, I implement the use of useMemo and useCallback hooks to efficiently memoize values and minimize recalculations. 
Additionally, I utilize code splitting and lazy loading to ensure that resources are loaded only when needed, enhancing the application's
overall performance. Moreover, I focus on optimizing assets and images to reduce load times. By strategically applying these methods, 
I have consistently improved the performance of React.js applications, ensuring a smooth and responsive user experience

36. In your opinion, what are the key differences between React.js functional components and class components, and when would you choose one over the other?

React.js provides two main types of components: functional components and class components. 
The key difference lies in their syntax and usage. 
Class components are defined as a class that extends the 'Component' class from React and uses lifecycle methods for actions like mounting, 
updating, and unmounting. On the other hand, functional components are implemented as plain JavaScript functions. 
With the introduction of hooks in React 16.8, functional components now support state management and side effects through hooks like useState, 
useEffect, useCallback, useRef, and useMemo. 
It's important to note that both types can be used effectively, but functional components are currently favored due to the simplicity and 
reusability offered by hooks. This allows for clearer and more concise code.

=======================================================================
Technical Round - 45 min to 1hr

1. ReactJS
2. JavaScript
3. CSS3
4. HTML5

ReactJS

1. Explain redux and its architecture

Redux is a state management library for JavaScript applications, often used with React to manage global state in a predictable way.

Redux Architecture:
Store – Holds the application’s state.

Action – A plain object that describes what happened (e.g., { type: 'INCREMENT' }).

Reducer – A pure function that takes the current state and an action, and returns a new state.

Dispatch – Sends actions to the store.

Subscriber – Components subscribe to the store to receive updates.

Data flow is unidirectional:
Component → Dispatch Action → Reducer → New State → UI Update

2. What is Virtual DOM and how does it work?

Virtual DOM is a lightweight copy of the real DOM. 
When the state changes, React creates a new Virtual DOM, compares it with the old one (diffing), and updates only 
the changed parts in the real DOM for better performance.

3. What is Reconciliation?

✅ Reconciliation – React compares Virtual DOM changes with the real DOM. 

4. Have you worked on class component or functional?

"Yes, I have experience working with both class and functional components in React. 
Initially, I used class components for state management and lifecycle methods, but with the introduction of hooks, 
I transitioned to functional components for their simplicity and reusability. 
Functional components, along with hooks like useState and useEffect, have allowed me to write cleaner, more maintainable code. 
While I can work with class components when needed, I primarily use functional components in newer projects to align with modern React practices.


5. what are hooks in react and why are they used?

Hooks in React are functions that let you use state and lifecycle features in functional components, without needing class components.

Why are they used?
Manage state: useState allows state management in functional components.

Side effects: useEffect handles data fetching, subscriptions, and other effects.

Performance optimization: useMemo and useCallback help prevent unnecessary re-renders.

Custom logic reuse: Custom hooks enable sharing logic across components.

6. how do you setup routing in react application?

Use React Router for routing:

Install it: npm install react-router-dom

Wrap the app in <BrowserRouter>

Use <Routes> and <Route> to define paths

Use <Link> for navigation

7. What technique can be used to optimize react application?

Optimizing a React app: 
Use React.memo, useCallback, and useMemo to prevent unnecessary re-renders. 
Apply lazy loading, code splitting, and virtualization for efficient rendering. 
Optimize state management, minimize useEffect dependencies, and use SSR/SSG for faster load times.

javascript
---------------
1. What is closure in Javascript? what is lexical scope?

Closure allows a function to remember and access its parent’s variables even after execution.

Lexical scope determines variable accessibility based on where functions are declared in the code.

2. what is hoisting in javascript? 

Hoisting is JavaScript's behavior of moving variable and function declarations to the top of their scope before execution. 

Functions are fully hoisted, while var variables are hoisted but remain undefined until assigned. 
let and const are hoisted but inaccessible until initialized.

3. what are callback, promises and async-await?

Callback: A function passed as an argument to another function, executed later. 

Promise: An object representing a pending, fulfilled, or rejected asynchronous operation. 

Async/Await: A way to write asynchronous code more cleanly, making it look synchronous. 

All three help manage async tasks like API calls and file handling.


4. what are the ES6 feature?

ES6 features:

Let & Const: Block-scoped variables.

Arrow Functions: Shorter function syntax (() =>).

Template Literals: String interpolation (${}) and multi-line strings.

Destructuring: Unpacking values from arrays/objects.

Default Parameters: Default values for function parameters.

Rest & Spread: Handle arrays/objects (...).

Classes: OOP syntax for creating classes.

Modules: import and export for modular code.

Promises: Asynchronous operations handling.

Iterators & Generators: Custom iteration with for...of and yield.



5. What is Event Loops in JS?

Event Loop in JavaScript is a mechanism that handles asynchronous operations. 
It allows the JavaScript engine to execute non-blocking code (like I/O operations) by using the call stack, callback queue, and event queue.

Call Stack: Where the functions are executed.

Callback Queue: Stores the callback functions that need to be executed after the call stack is clear.

Event Loop: Continuously checks if the call stack is empty, and if so, moves the first event from the callback queue to the stack for execution.

6. What is ES6 Array methods - map(), filter()

map(): Creates a new array by applying a function to each element of the original array.

const arr = [1, 2, 3];
const newArr = arr.map(x => x * 2); // [2, 4, 6]

filter(): Creates a new array with all elements that pass the condition in the provided function.

const arr = [1, 2, 3, 4];
const evenArr = arr.filter(x => x % 2 === 0); // [2, 4]




CSS3:

1. Explain the Box Model in CSS?

The CSS Box Model describes how elements are structured on a page. It includes:

Content – The actual text or image.

Padding – Space around the content.

Border – Wraps around the padding.

Margin – Space outside the border, separating elements.

2. What is difference between position Absolute & Relative?

position: relative moves an element relative to its normal position.
position: absolute removes the element from the normal flow and positions it relative to the nearest positioned ancestor.

3. What is the difference between rem and px?

px is an absolute unit — it defines a fixed size in pixels.
rem is a relative unit — it scales based on the root element’s (<html>) font size.

Example: If root font size is 16px, then 1rem = 16px.

4. What is Flex box?

Flexbox is a CSS layout model that makes it easy to align, space, and distribute items in a container, even when their size is unknown.

It uses properties like display: flex, justify-content, align-items, and flex-direction to create responsive layouts.

5. What is Grid Layout?

CSS Grid Layout is a 2D layout system used to design web pages in rows and columns.

It allows precise control over placement using properties like display: grid, grid-template-columns, grid-template-rows, and grid-gap.


HTML5:

1. What is Semantic Elements in HTML?
Semantic elements in HTML clearly describe their meaning to both the browser and developer.
Examples include <article>, <section>, <header>, and <footer>. They improve readability, accessibility, and SEO.

2. What is purpose of meta tag in HTML?

The meta tag in HTML provides metadata about the web page, such as character encoding, author, description, and 
viewport settings. It's mainly used for SEO and browser behavior control

3. What is block level and inline element?

Block-level elements take up the full width and start on a new line (e.g., <div>, <p>, <h1>).
Inline elements take up only as much width as needed and do not start on a new line (e.g., <span>, <a>, <strong>).


4. What is local storage vs Session Storage
Local Storage stores data with no expiration time — it persists even after the browser is closed.
Session Storage stores data only for the duration of the page session — it clears when the tab or browser is closed.

==========================================================================================================================

technical interview questions
-----------------------------------------

1. tell me about yourself?

2. which version of react.js are using? React v18.2.0

3. what is async await?
async and await are JavaScript keywords used to handle asynchronous operations in a cleaner, more readable way compared 
to traditional Promises and callbacks

"async/await is a syntax in JavaScript that makes it easier to work with Promises. 
async makes a function return a Promise, and await pauses execution until the Promise resolves, 
 asynchronous code to be written in a more readable, synchronous-like way."

4.  what is synchronous vs asychronous?

Synchronous code runs one task at a time, blocking the next task until the current one finishes.
Asynchronous code allows multiple tasks to run without waiting—like handling network requests—so the 
program stays responsive.

5. how to call multiple api calls simunatenously?
To make multiple API calls at the same time, I use Promise.all(). 
It takes an array of Promises and waits until all of them are resolved or any one fails.

async function fetchAllData() {
  const [userData, postsData] = await Promise.all([
    fetch('/api/user'),
    fetch('/api/posts')
  ]);

  const user = await userData.json();
  const posts = await postsData.json();

  console.log(user, posts);
}

// This runs both API calls at the same time and waits for both to complete.

6. what is controlled and uncontrolled components?

In React, controlled components are form elements whose values are managed by React state. 
Uncontrolled components manage their own state internally using the DOM, often accessed via ref.

Controlled: React is the single source of truth.

Uncontrolled: DOM handles the form data.

7. what is Debouncing ?

Debouncing is a technique used to limit how often a function is called.
It ensures the function runs only after a specified delay once the last event (like typing or scrolling) has stopped. 
It’s commonly used to optimize performance in search inputs, resize, or scroll events.

8. What is useEffect hook? How Does useEffect Work?

The useEffect hook in React is used to handle side effects in functional components, like data fetching, 
subscriptions, or manually changing the DOM. It runs after the component renders.

✅ How useEffect Works:


useEffect(() => {
  // Side effect logic here (e.g., API call)

  return () => {
    // Optional cleanup (e.g., clear timer, unsubscribe)
  };
}, [dependencies]);
The first argument is a function with your side effect logic.

The second argument is a dependency array that controls when the effect runs.



9. did you work on custom hooks?
Yes, I’ve worked with custom hooks in React to encapsulate reusable logic and keep components clean. 
For example, I created a custom hook for form handling, another for API data fetching with loading and error states, 
and one to manage debounced input values. This helped maintain separation of concerns and made my code more modular 
and testable.

10. how to make api call without useEffect?

You can make an API call without using useEffect by triggering it through user actions like a button click,
form submission, or any other event handler.

11. What is promise.All() and race?

Promise.all(): Waits for all Promises to resolve or for any to reject.

Promise.race(): Resolves or rejects as soon as one Promise resolves or rejects.


12. How do you integrate 2 API in front end with useEffect?
To integrate two APIs in the frontend using useEffect, 
you can either call them simultaneously with Promise.all() or sequentially.

Simultaneous: Both APIs are called in parallel.

Sequential: One API is called after the other.

13. How Do Uncontrolled Components Work?
Uncontrolled components in React manage their own state via the DOM, not React state. You access the values using refs.


14. redux architecture?

Redux architecture consists of three key parts:

Store: Holds the entire application state.

Actions: Plain objects that describe what happened.

Reducers: Functions that update the state based on the action.

Data Flow:
Actions are dispatched.

Reducers process the action and return a new state.

Store updates and re-renders subscribed components.


15. what is == vs ===? Which One Should You Use?

== (Loose Equality): Compares values after type coercion (converts the types before comparing).

=== (Strict Equality): Compares both value and type without type coercion.

Always use === for strict equality to avoid unexpected results from type coercion.

== should be avoided unless you specifically want type coercion.

16. can you explain your implementation

17. have you worked as a LEAD?


18. what is return and commit in JSX?

return in JSX is used to return the JSX that represents the UI in React components.

Example:

function MyComponent() {
  return <div>Hello</div>;
}
commit is not a standard React/JSX concept. 
It might refer to operations in third-party libraries or custom implementations, often related to finalizing changes 
or state updates.

19. What is map()? and reduce()?


map(): Creates a new array by applying a function to each element of the original array.

[1, 2, 3].map(num => num * 2); // [2, 4, 6]

reduce(): Accumulates a single value by applying a function to each element, with an accumulator.

[1, 2, 3].reduce((acc, num) => acc + num, 0); // 6


20. what is the output of map()?

The output of map() is a new array with transformed elements based on the function provided.

Example:
[1, 2, 3].map(num => num * 2); // [2, 4, 6]

====================================================================

30 minute interview

Senior React.js Developer Interview Question and Answers.

1. Tell me about yourself?


2. React Hooks: 
Hooks are functions that enable functional components to manage state and lifecycle features, 
providing a more concise and expressive way to handle component logic.

3. What are the popular hooks in react and explain it's usage?

useState: Manages state in functional components.
useEffect: Manages side effects in functional components.
useContext: Consumes context in functional components.
useReducer: Manage state with a reducer function, For More complex state management.
useRef: Accesses DOM elements or stores mutable values.
useCallback: performance improvement usecase
useMemo: performance improvement usecase.

4. How can you Optimize Performance in React application?
1. Memoization with useMemo and useCallback:  Use this hooks to memoize values and, reducing unnecessary recalculations.
2. Optimizing Renders with React.Fragment: Use it to avoid unnecessary wrapper elements that could cause additional DOM nodes.
3. Lazy loading with React.lazy: Use it to load components lazily, reducing the intial bundle size and imporving intial loading performance.
4. Code splitting: Employ code splitting to divide your application into smaller chunks that are loaded on demand, improving initial load times.
5. Optimizing Images and Assets:  Compress and optimize images, use responsive images and leverage lazy loading for images to reduce network and rendering overhead.


5.  Difference between virtual DOM and real DOM?
Suppose line of code is changed , processing is done on particular line. 
It will process the whole code in real DOM. Virtual DOM is faster.

6. Redux is a predictable state container for JavaScript applications. 
It helps to you write applications, run in different environments and easy to test. 
And simply we called as Redux is a state management tool.
Components in redux
Actions -->Input Parameters Ex: Deposit and Withdraw money from ATM
Store --> Main Server
Reducers --> Business Logic
Dispatch --> Request
Subscribe --> Response
State --> Store Component Data

7. What is state management in react application? 3rd party module, with redux.
Redux? We have redux thux, redux saga.
What is redux thunx, redux saga? Inorder to manipulate the store Actions(request, response).
Redux thunx is an outdated library.
Saga is Advanced library.

Why Saga? In sagas debouncing is available by default.

8. Explain React lifecycle methods?

React component lifecycle has three categories – Mounting, Updating and Unmounting.
Mounting – Birth of your component
Update – Growth of your component
Unmount – Death of your component

React Component LifeCycle Hooks

        1. constructor
        2. componentWillMount()
        3. render()
        4. componentDidMount()
        5. componentWillReceiveProps()
        6. shouldComponentUpdate()

        // component kill methods

        7. componentWillUpdate()
        8. componentDidUpdate()
        9. componentWillUnmount()

Recently Added LifeCycle Hooks

Context API, useEffect, useState --- Newly added version by version

Explanation:

# Constructor()

        constructor will execute at booting time of component --constructor will execute only once
        Define state in constructor

# componentWillMount()

        componentWillMount() will execute after constructor
        componentWillMount() will execute only once
        in general we will do the initial modifications in state
        in general we will set global parameters like width, height

# render()

        after componentWillMount() automatically render() function will execute
        render() is mandatory lifecycle hook(main lifecycle hook)
        in general, we will place presentation logic in render()
        when ever change detected in state or props automatically this lifecycle hooks will execute

# componentDidMount()

        after render function immediately componentDidMount() life cycle hook will execute
        in general we will make asynchronous calls in ComponentWillMount()
        this is recommended state to change the state of component

# componentWillReceiveProps()

        when component will receive props from redux

# shouldComponentUpdate()

        if we want to update the state return "true" else "false"

# UNSAFE_componentWillUpdate()

        death method --> perform cleanup operations

# componentDidUpdate()

        if we integrate any third party UI elements
        plugin logic will write here

# componentWillUnmount()

        Before killing the component componentWillUnmount is executed.
        death method --> perform cleanup operations


9. Call() -- if we want to create second memory location will interact with 1st memory location.

Apply – if we want to pass array instead of independent parameter

Bind() - merge memory location 1 and memory location 2 -->merge 2 memory locations-->new memory location.

What is the USE? Call function advanced function APPLY, call and apply advanced version is bind().
Purpose is same. Call, bind, apply –used to access 2 objects in different memory location

10. What is the current ES version? ES6 -2015, ES9, JS24

11. What are different positions in CSS ?
The position property specifies the type of positioning method used for an element.

There are five different position values:

static: HTML elements are positioned static by default.

relative: An element with position: relative; is positioned relative to its normal position.

fixed: An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. 
The top, right, bottom, and left properties are used to position the element.

absolute: An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

sticky: An element with position: sticky; is positioned based on the user's scroll position.


12. What is shallow copy and deep copy? 

A shallow copy creates a new object with references to the same memory locations as the original object for nested properties. 
This means changes to nested objects in the copy will affect the original object.

javascript example: 
const originalObject = { a: 1, b: { c: 2 } };
const shallowCopy = { ...originalObject };

shallowCopy.b.c = 3;
console.log(originalObject.b.c); // Output: 3

Deep Copy
A deep copy creates a new object with new memory locations for all nested properties, ensuring changes to the copy don't affect the original object.

JavaScript Example:

javascript
const originalObject = { a: 1, b: { c: 2 } };
const deepCopy = JSON.parse(JSON.stringify(originalObject));

deepCopy.b.c = 3;
console.log(originalObject.b.c); // Output: 2

===============================================================================================

First Round: 30 minute React and Javascript.

1. current Project?

2. advantages of react?
    * Simple to build Single Page Application(by using Components - component based architecture).
    * React is cross platform and open source(Free to use)
    * Lightweight and very fast(Virtual DOM)
    * Large Community and Ecosystem.
    * Testing is easy.

3. hooks? some examples useState, useEffect?

    * React Hooks are inbuilt functions provided by React that allow functional components to useState and lifecycle features.
    * Before Hooks, class components lifecycle methods were used to maintain state in React Applications.
    * To use React hook first we first have to import it from React Library.

The useState hook enables functional components to manage state.
useState() working: useState() function accept the initial state value as the parameter and returns an array with 2 elements:
1. The first element is the current state value(count in this code).
2. Second element is the function that is used to update the state(setCount in this code).
The concept of assign array elements to individual variables is called array destructing.

The useEffect Hook in React is used to perform side effects in functional components.
For example, data fetching from API, subscriptions or any other operation that needs to be performed after the component has been rendered.

4. what is redux?

//state management(centralized store)
Redux is a predicatable state container for JavaScript apps. 
Redux acts as centralized store for state management in your application.
Advantages:
Single Source of Truth: The State of the application is stored in a single object.
State is Read-Only: The only way to change the state is to emit an action, an object describing what happened.
Changes are made with Pure Functions: Reducers are pure functions that take the previous state and an action, return the next state.

5. what is synthetic event?

a synthetic event is a cross-browser wrapper around the browser's native event. 
It combines the behavior of supported events of different browsers into one API, ensuring that events work identically across all browsers.

6. Event delegation?
Event delegation is a technique in JavaScript where a single event listener is attached to a parent element to handle events for
all of its child elements. 
Instead of attaching individual event listeners to each child, the parent element "delegates" the handling of events to its children. 
This approach leverages event bubbling, where an event on a child element propagates up the DOM tree to its parent elements. 


7. Why is javascript is synchronous not asynchronous?
JavaScript is primarily synchronous, running one piece of code at a time. 
However, it can handle asynchronous tasks using callbacks, promises, and async/await. 
This allows JavaScript to remain responsive by doing other work while waiting for time-consuming operations to finish.

8. What is the current ES version? ES6 -2015, ES9, JS24

9. object methods?
object.keys
object.values
object.freeze - we can't modify or delete from object
object.seal - we can modify but can't delete or add.

10. how to add properties to object?
object.assign()

11. suppose car has color, model and features, add some more properties of basic car?

12. create a object in javascript in jsfiddle?

const city ={
    name: 'austin',
    population: '10million',
}
city.street = '';

13. object.prototype?

14. coding question:
const fruits = [{name: 'apples', quantity: 500},
{name: 'bananas', quantity: 500},
{name: 'oranges', quantity: 150},
{name: 'kiwi', quantity: 150}];

show output: [[apples, bananas], [oranges, kiwi]];


//hint: use reduce

15. how browser knows javascript? JavaScript is preinstalle in browser.
if you write in typescript? it will convert the typescript to javascript.

use TS compiler

16. hoisting?

Hoisting is a behavior in JavaScript where variable and function declarations are moved to the top of their respective scopes during 
compilation phase, before the code is executed. This means that regardless of where variables and functions are declared in the code, 
they are treated as if they are declared at the beginning of their scope.

example:
console.log(x); //output: undefined
var x = 5;
console.log(x); //output: 5

the declaration of x is hoisted to the top, but not its initialization. That's why the first `console.log outputs undefined.

let and const declarations are hoisted but not initialized. This leads to a "temporal dead zone" where accessing the variable before its declaration results in a ReferenceError.

console.log(y);
// throws ReferenceError: Cannot access 'y' before "initialization"
let y = 10;



17. async/ await

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

18. event bubbling? event capturing?

DOM elements are HTML Element. Parent , Child, Subchild.

Click Subchild -->Subchild, Child, Parent will execute.

The Events are propagating from down to top is called Event Bubbling.


What is Event Capturing? If I click parent only parent will execute. If I click child -->parent, child will execute. 
Propagation of Events from top to bottom is called Event Capturing.

React.js interview

19. what total experience in react.js till now? 12+

20. Which redux? redux-Toolkit:

Redux is a predicatable state container for JavaScript apps. Redux acts as centralized store for state management in your application.

Redux Toolkit is an offical, opinionated toolset for efficient Redux development.
It simplifies store setup, reduces boilerpate, and includes useful tools like createSlice and createAsyncThunk.

import {configureStore} from '@reduxjs/toolkit'; //import
const store = configureStore({
    reducer:{
        //pass all reducers
    },
});

export default store;

===============================================================================

Interview Question and answers

1. Tell me about yourself.

2. Which version of react? v16.8

3. How to optimize performance in react ?

1. Memoization with useMemo and useCallback:  Use this hooks to memoize values and, reducing unnecessary recalculations.
2. Optimizing Renders with React.Fragment: Use it to avoid unnecessary wrapper elements that could cause additional DOM nodes.
3. Lazy loading with React.lazy: Use it to load components lazily, reducing the intial bundle size and imporving intial loading performance.
4. Code splitting: Employ code splitting to divide your application into smaller chunks that are loaded on demand, improving initial load times.
5. Optimizing Images and Assets:  Compress and optimize images, use responsive images and leverage lazy loading for images to reduce network and rendering overhead.


4. What is difference between Promise.all() and race?

Promise.all() waits for all promises to settle (either resolve or reject), and resolves with an array of all resolved values or rejects as soon as one promise rejects.

Promise.race() resolves or rejects as soon as the first promise settles (either resolves or rejects).

5. difference between useMemo and useCallback?

Key Differences:

    useMemo: Memoizes the result of a computation (value). It helps with performance optimization by avoiding recalculating expensive values.

    useCallback: Memoizes the function itself, ensuring the function reference remains the same between renders unless its dependencies change. 
    It's mostly useful when passing functions as props to avoid unnecessary re-renders in child components.

6. Have you used async/await? use?

async: Declares a function that will always return a Promise.

await: Pauses the execution of the async function until the Promise resolves or rejects.

7. What are hooks in react? use?

useState: Manages state in functional components.
useEffect: Manages side effects in functional components.
useContext: Consumes context in functional components.
useReducer: Manage state with a reducer function, For More complex state management.
useRef: Accesses DOM elements or stores mutable values.
useCallback: performance improvement usecase
useMemo: performance improvement usecase.

8. did you work on custom hooks?

Custom Hooks in React are JavaScript functions that allow you to reuse stateful logic across multiple components.
They enable you to extract and share common logic without repeating code, promoting code reusability and separaration concerns.

c1, c2, c3, c4, c5--> one custom hooks --> state
Advantages:
Code Reusability: Custom hooks allow you to reuse stateful logic without duplicating code.
Separation of Concerns: They help spearate the logic from the component's structure, making the code more modular and easier to maintain.
Cleaner Code: By Moving common logic into custom hooks, components become cleaner and more focused on their core responsibilites.

9. Can we useHelp() hook instead of custom hook?

If useHelp() is a custom hook you've created or imported, then yes, you can use it just like any other hook.

Custom hooks don't replace built-in hooks; they are for organizing reusable logic. You can still use built-in hooks inside your custom hooks if needed.

10. what is callback?

Passing "one function" to "another function" as an argument called as "CallBack"

11. what is callback hell?

Callback hell" refers to a situation in programming where multiple asynchronous operations are handled using nested callback functions,
creating a complex and difficult-to-read code structure, often resembling a pyramid shape; 
to avoid it, use techniques like Promises and the async/await syntax to manage asynchronous operations in a more linear fashion,
making your code cleaner and easier to maintain. 

12. have you worked on NodeJS?

Node.js is commonly used for backend development, APIs, real-time applications (like chat apps), and more. 
It leverages non-blocking, event-driven architecture, making it ideal for I/O-heavy tasks like handling HTTP requests, reading files, and querying databases.

I can help with many aspects of Node.js development, including:

    Creating web servers using frameworks like Express.js.

    Working with databases (like MongoDB, MySQL, PostgreSQL) through libraries like mongoose or sequelize.

    Building APIs (RESTful APIs, GraphQL, etc.).

    Managing asynchronous operations (with callbacks, promises, and async/await).

    Implementing middleware for routing and error handling.

    Integrating third-party services (like payment gateways, email services, etc.).

    Optimizing performance (using clustering, worker threads, etc.).

    Deploying Node.js applications (on cloud platforms like AWS, Heroku, etc.).

13. difference between fetch and axios module?

fetch is a built-in JavaScript API that returns a Promise. It is native to the browser and doesn't require installing any additional libraries.

axios is a third-party library that also returns a Promise. It needs to be installed via npm or yarn (e.g., npm install axios).

Fetch Example:

fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));

Axios Example:

axios.get('https://api.example.com/data')
  .then(response => console.log(response.data))
  .catch(error => console.error('Error:', error));


14. call api in react syntax?

axios.get('https://api.example.com/data')
  .then(response => console.log(response.data))
  .catch(error => console.error('Error:', error));

15. what is hoisting? explain with example?

console.log(a); // Uncaught ReferenceError: a is not defined
let a; 

console.log(a); // Uncaught ReferenceError: a is not defined
let a = 10;

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


16. What is promise?

 - Promises Establishes the communication between "producer" and "consumer".
 
        - Promises also called as "special javascript objects".
 
        - we will create Promises by using "Promise" class constructor.
 
        - Promises have 3 states
 
            1) success  (resolve)
 
            2) error    (reject)
 
            3) pending
 
        - we will consume promises by using "then()"

/*
    let promise1 = new Promise((resolve,reject)=>{
        resolve("tomorrow i will discuss async & await keywords");
    });
    promise1.then((posRes)=>{
        console.log(posRes);
    },(errRes)=>{
        console.log(errRes);
    });     //tomorrow i will discuss async & await keywords
*/

17. What is synchronous and asynchronous calls?

Synchronous calls block the program until the current task finishes. Everything happens in sequence.

Asynchronous calls allow the program to continue executing while waiting for a task to complete, preventing it from freezing or being blocked.

18. What operations did you perform in NodeJS?

    HTTP Server: Set up basic web servers to handle requests and responses.

    REST APIs: Created APIs for handling CRUD operations using Express.

    File Operations: Used the fs module to read, write, and manipulate files.

    Database Integration: Worked with databases (e.g., MongoDB) using libraries like Mongoose.

    Event-driven: Utilized the EventEmitter for event-driven programming.

    Asynchronous Programming: Managed asynchronous operations using Promises and async/await.

    Middleware: Built custom middleware in Express for additional functionality (e.g., logging, authentication).

Node.js offers a robust environment for developing scalable, event-driven applications and handling backend services, APIs, and tasks efficiently.

19. callback hell resolve?

Callback Hell can be mitigated by:

    Modularizing code: Break down tasks into smaller functions.

    Using Promises: Chain asynchronous operations and handle errors in a clean way.

    Using Async/Await: Write asynchronous code that looks synchronous, improving readability.

    Using Libraries like Async.js: Manage complex flows in a more elegant and concise way.

    Using Event Emitters: For managing more complex workflows that involve multiple events.

The async/await approach is generally the most modern and readable method, and it resolves the deep nesting of callbacks effectively, improving code quality and maintainability.

20. What is a closure in JavaScript?

    - if any inner function holding the outer function data, then such scenario called as closure.

21. can we write application in redux instead of redux-saga?

Yes, you can write applications using Redux without using Redux-Saga. Redux itself is a state management library, 
while Redux-Saga is a middleware used for handling side effects (like async actions such as fetching data from an API, interacting with external services, etc.).

22. what is difference redux, redux-thunk, redux-saga?

Redux is for managing the state of your application.

Redux-Thunk is a simple middleware for managing simple async logic like API calls or timeouts.

Redux-Saga is a middleware that handles complex side effects using generator functions, making it ideal for handling advanced async logic
(e.g., canceling tasks, running multiple tasks in parallel, and managing retries).

23. explain how redux architecture works? example?

Redux Data Flow

    User Interaction or Events trigger an action.

    The action is sent to the store using the dispatch function.

    The store forwards the action to the appropriate reducer.

    The reducer computes a new state based on the action.

    The store updates the state with the new value.

    The updated state can be accessed by React components or any part of the app.

This process follows the unidirectional data flow in Redux, where actions trigger state updates, and the components re-render based on the updated state.

24. what is react 19 features?

The New Additional Hooks in React 19:-

1. useFormStatus
-Tracks form submission status dynamically.
-Eliminates manual state tracking for pending operations.

2. useActionState
-Combines form actions and states into one seamless hook.
- Perfect for server-side rendered applications.

3. useOptimistic
-Supports optimistic Ul updates for async operations.
- Makes rollbacks smooth if operations fail.

4. use
-Brings promises and async context handling directly into components.
-Enhances Suspense for better async rendering.

25. what is useRef() hook?

The useRef hook is used to access and interact with DOM elements directly and to persist mutable values across renders without causing re-renders.



26. useLayoutEffect? useLayoutEffect fires before the browser repaints the screen. You can measure layout here.

useLayoutEffect: Synchornous Side effects.

27. what is synchronous vs asynchronous call?

Synchronous Call:

    A synchronous call means that the code is executed in a sequential, blocking manner. 
    The program executes each statement one after another, waiting for the previous one to finish before moving on to the next.

    In other words, each operation must complete before the next one begins.

Asynchronous Call:

    An asynchronous call allows certain tasks to run in the background while the program continues executing other code. 
    It doesn't block the rest of the program, and the operation may complete at a later time.

    Common asynchronous operations include fetching data from an API, setTimeout, Promises, or async/await syntax.


React

performance opt

Javascript



=========================================

Es6 features
ES6 is ECMAScript 6. It is nothing but Javascript Version.
ES6 allows let and const for variable declaration.
	 we have 8 types of functions  (ES6-ES11)
	     1) Named Functions
	     2) Anonymous Functions / Arrow Functions  (ES6)
	     3) Rest Parameters in Functions
	     4) Default Parameters in Functions
	     5) Optional Parameters in Functions
	     6) IIFE (Immediate Invokable Functional Expressions) (ES9) (2019)
	     7) Generator Functions
    8) Constructor Functions.



    Promises
    --------
        - Promises Establishes the communication between "producer" and "consumer".
 
        - Promises also called as "special javascript objects".
 
        - we will create Promises by using "Promise" class constructor.
 
        - Promises have 3 states
 
            1) success  (resolve)
 
            2) error    (reject)
 
            3) pending
 
        - we will consume promises by using "then()"
*/
 
 
 
/*
    let promise1 = new Promise((resolve,reject)=>{
        resolve("tomarrow i will discuss async & await keywords");
    });
    promise1.then((posRes)=>{
        console.log(posRes);
    },(errRes)=>{
        console.log(errRes);
    });     //tomarrow i will discuss async & await keywords
*/
 
	3. What is Functional Component?
A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.

A class component requires you to extend from React.Component and create a render function which returns a React element. 

=========================================================================
200 React JS Interview Q & A

React Basics-1
Q1. What is React? What is the Role of React in software development?
React is open source Javascript Library.
React is used for building user interfaces(UI).
React Simplifies the creation of SPA by using reusable components.

Q2 what are the key Features of React?
7 key features:
1. Virtual DOM
2. Component based architecture
3. Reusability & Composition
4. JSX (Javascript XML)
5. Declarative Syntax
6. Community & Ecosystem
7. React Hooks.
Virtual DOM: React utilizes a virtual representation of the DOM, allowing efficient updates by minimizing direct manipulation of the actual DOM, resulting in improved performance.

Component-Based Architecture: React structures user interfaces as modular, reusable components, promoting a more maintainable and scalable approach to building applications.

Reusability & Composition: React enables the creation of reusable components that can be composed together, fostering a modular and efficient development process.

JSX(JavaScript XML): JSX is a syntax extension for JavaScript used in React, allowing developers to write HTML like code within JavaScript, enhancing readbility and maintainability.

Declarative Syntax: React have a declarative programming style(JSX), where developers focus on "what" the UI should like and React handles the "how" behind the scenes. This simplify the code.

Community & Ecosystem: React benifits from a vibrant and extensive community, contributing to a rich ecosystem of libraries, tools and resources, fostering collaborative development and innovation.

React Hooks: Hooks are functions that enable functional components to manage state and lifecycle features, providing a more concise and expressive way to handle component logic.



Q3 what is DOM? What is the difference between HTML & DOM?

DOM(Document Object Model) represents the web page as a tree-like structure which allows Javscript to dynamically access and manipulate the content and structure of a web page.


Q4 What is virtual DOM ? Difference between DOM & Virtual DOM?

React uses a virtual DOM to efficently update the UI without re-render the entire page, which helps improve performance and make the application more responsive.

Reconciliation (React Libraries)

DOM                                                 Virtual DOM
1. DOM is actual representation of the webpage.      1. Virtual DOM is lightweight copy of the DOM.
2. Re-renders the entire page when updates occur.    2. Re-render only the changed parts efficently.
3. Can be slower, especially with frequent updates.  3. Optimized for faster rendering.
4. Suitable for static websites and simple applications 4. ideal for dynamic and complex single-page applications with frequent updates.


Q5 What are React Components? What are the main elements of it?

In React, a component is a reusable building block for creating user interfaces.

//1. Import the React Library
import React from "react";

2. Define a functional component
function Component(){
    //3. Return JSX to describe the component's UI
    return(
        <div>
            <h1>i am a react reusable component</h1>
        </div>
    );
}
//4. Import the component to make it available
//for use in other files
export default component;

Q6 What is SPA (Single Page Application)?

A Single Page Application(SPA) is a web application that have only one single web page.
whenever user do some action on the website, then in response content is dynamically updated without refreshing or loading a new page.

Q7 What are the 5 advantages of React?

1. Simple to build Single Page Application(by using Components - component based architecture).
2. React is cross platform and open source(Free to use)
3. Lightweight and very fast(Virtual DOM)
4. Large Community and Ecosystem.
5. Testing is easy.

Q8 What are the disadvantages of React?
React is not a good choice for very small applications.

Q9 What is the role of JSX in React? (3 points)

1. JSX stands for JavaScript XML.
2. JSX is used by React to write HTML-Like code.
3. JSX is converted to Javscript via tools like Babel.(Because browsers understand JavaScript not JSX.)


Q10 what is the difference between Declarative & Imperative Syntax?

Declarative                                                         
1. Declarative syntax focuses on describing the desired result without specifying the step-by-step process.
2. JSX in React is used to write declarative syntax.

Imperative
1. Imperative syntax involves step by step process to achieve a particular goal.
2. Javascript has an imperative syntax.

React Basics-2 
Q11 What is Arrow Function Expression in JSX?

The arrow function expression syntax is a concise way of defining functions.

//Arrow function Expression
const ArrowFunc = (props) => {
    return (
        <div>
            <h1>{props.name}</h1>
        </div>
    );
};

export default ArrowFunc;


Q12 How to Setup React first project?

1. Install Node.js from link. nodejs.org

2. Install code editor for writing the code. VS Code link --> download

3.  Open VS Code --> terminal --> npx create-react-app my-app --> takes 5-6 minutes

4. VS code --> file --> open folder --> MY-APP --> open terminal --> npm start


Q13 What are the Main files in React project?

        Request    
Browser  ---->      index.html --> Single Page

                       ^ >        
          <-----      index.js--> entry point(JS)
        Display             ^
comp1.js, comp2.js, comp3.js -----App.js ==> Root Component

Q14 How React app Load & display the components in browser?

index.html --> Single page which loads index.js by React libraries.

index.js --> Replace root element of index.html file by App component

App.js --> Root Component which is the container of all the child components.

child component.js --> custom child components placed over app component.


Q15 What is the difference between React & Angular?

React                                                                   Angular
React and Angular both are used to create single page UI applications using components.
1. React is a Javascript Library.                                   1. Angular is a complete Framework.
2. React uses virtual DOM which makes it faster.                    2. Angular uses a real DOM.
3. React is smaller in sixe and lightwight and therefore faster sometime.  3. Angular is bigger because it is a complete framework.
4. React depends on external libraries for many complex features, so      4. Since Angular is a complete framework, therfore it provide built-in support for features like routing, forms, validation and HTTP requests.
developer has to write many lines of code for complex functionalities

5. React is simple to learn and more popular than Angular.              5. Angular is slightly difficult to learn as it has Typescipt, OOPS concept and many more thing.


Q16 What are the other 5 JS frameworks other than React?

Angular
Vue.js
AngularJS
Backbone.js
Ember.js

Q17 Whether React is Framework or Library? what is the difference?

Library: Developers import the libraties at the top and then used it functions in components.
React is commonly reffered to as a Javscript Library

Framework: Developers need to follow a specific structure or pattern defined by the framework.
Angular is a framework.

@Component({
    selector:'app-root',
    templateUrl: './app.component.html',
    styleUrls:['./app.component.css']
})
export class AppComponent{
    title = "Hello World";
}


Q18 How React provide Reusability & Composition?
React provides Reusability and Composition through its component-based architecture.
Reusability: once you create a component, you can re-use it in different parts of your application or even in multiple projects.
Composition: Composition is creating new and big components by Components by combining existing small components. Its advantage is, change to one small component will not impact other components.


Q19 What are State, Stateless, Stateful and state management teams?

"State" refers to the current data of the component.

Stateful or state management means when a user performs some actions on the UI, then the React application should be able to update and re-render the data or state on the UI.


Q20 What are Props in JSX?
Props(properties) are way to pass data from a parent component to a child component.

React Basics-3 
Q21 What is NPM? What is the role of node_module folder?
NPM(Node Package Manager) is used to manage dependencies for your React project, including the React Library itself.

node_modules folder contains all the dependencies of the project, including the React libraries.



Q22 What is the role of public folder in React?
Public folder contains static assets that are served directly to the user's browser, such as images, fonts, and the index.html file.



Q23 What is the role of src folder in React?

src folder is used to store all the source code of the application which is then responsible for the dynamic changes in your web application.


Q24 What is the role of index.html page in React?

index.html file is the main HTML file(SPA) in React application.
here the div with id="root" will be replaced by the component inside index.js file.


Q25 What is the role of index.js file & ReactDOM in React?

ReactDOM is a Javascript library that renders components to the DOM or browser.

The index.js file is the javascript file that replaces the root element of the index.html file with the newly rendered components.


Q26 What is the role of App.js file in React?

App.js file contain the root component(App) of React Application.

App Component is like a container for other components.

App.js defines the structure, layout, and routing in the application.


Q27 What is the role of function & return inside App.js?

1. The function keyword is used to define a JavaScript function that represent your React component.
2. function is like a placeholder which contains all the code or logic of component.
3. The function takes in props as its argument(if needed) and return JSX.
return is used to return the element from the function.

Q28 Can we have function without a return inside App.js?

Yes, a function without a return statement is possible.
In that case, your component will not render anything in UI.
The common use case is for logging purpose.

Using arrow function

const FuncWithoutReturn = ()=>{
    console.log("no return");
}

Q29 What is the role of export default inside App.js?
Export statement is used to make a component available for import using "import" statement in other files.

import React from "react";

const AppChild = (props) =>{
    return <h1>hi</h1>
}

export default AppChild;


Q30 Does the file name & component name must be same in React?

No, the file name and the component name don't have to be the same.
However, it is recommended to keep the same for easier to organize and understand your code.

React -4 JSX

Q31 What is the role of JSX in React? (3 points)

1. JSX stands for JavaScript XML.
2. JSX is used by React to write HTML-Like code.
3. JSX is converted to Javscript via tools like Babel.(Because browsers understand JavaScript not JSX.)

function App(){
    return(
        <div className="App">
            <h1>Hello!</h1>
        </div>
    );
}

Q32 What are the 5 Advantages of JSX?

1. Improve code readability and writability
2. Error checking in advance(Type safety)
3.support JavaScript expressions
4. Improved performance
5. code Reusability.


Q33 What is Babel?

Babel in React is used to transpile JSX syntax into regular Javscript which browser can understand.


Q34 What is the role of Fragment in JSX?

In React, a fragment is a way to group multiple children's elements.
Using a Fragment prevents the addition of unnecessary nodes to the DOM.

<Fragment>
<div>vijay</div>
<div>reactjs</div>
</Fragment>

Q35 What is Spread Operator in JSX?

The Spread operator(...) is used to expand or spread an array or object.

function App() {
    const props = {name: "vijay", id:1};
    return (
        <ChildComponent {...props}/>
    );
}

function ChildComponent(props){
    return <div>{props.name},{props.id}</div>;
}


Q36 What are the types of Conditional Rendering in JSX?

Conditional Rendering

1. If /else statements 

2. Ternary Operator

3. && operator  - returns truthy value.

4. Switch statement


Q37 How do you iterate over a list in JSX? What is map() method?

map() method allows you to iterate over an array and modify its elements using a callback function.


Q38 Can a browser read a JSX file?

No, browsers cannot directly interpret or understand JSX files. 
Babel takes JSX and converts it into equivalent Javascript code that browsers can understand.


Q39 What is Transpiler? What is the difference between Compiler & Transpiler?

A Transpiler is a tool that converts source code from one high-level programming lanaguage(JSX) to another high-level programming language(JavaScript).
Ex: Babel.

A Compiler is a tool that converts high-level programming language (Java) into a lower-level language(machine code or byte code).


Q40 Is it possible to use JSX without React? 

Yes, it's possible to use JSX without React by creating your own transpiler like Babel.
However, this is not recommended since JSX is tightly integrated with React and relies on many React-specific features.


React- 5 Components-Functional/Class

Q41 What are React Components ? what are the main elements of it?

In React, a component is a reusable building block for creating user interfaces.

//1. Import the React Library
import React from "react";

//2. Define a functional component
function Component(){
    //3. Return JSX to describe the component's UI
    return(
        <div>
            <h1>react reusable component</h1>
        </div>
    );
}

//4. Export the component to make it available
// for use in other files
export default Component;

Q42 What are the Types of React Components? What are Functional Components?

Types of Components

1. Functional Components: They are declared as a JavaScript function. 
They are stateless component, but with the help of hooks, they can now manage state also.

2. Class Components

Q43 How do you pass data between functional components in React?

props(properties) are a way to pass data from a parent component to a child component.

Q44 What is Prop Drilling in React?
Prop drilling is the process of passing down props through multiple layers of components.


Q45 Why to Avoid Prop Drilling? In how many ways avoid Prop Drilling?
1. Maintenance: Prop drilling can make code harder to maintain as changes in data flow require updates across multiple components.
2. Complexity: It increases code complexity and reduces code reability.
3. Debugging: Debugging becomes challenging when props need to be traced through numerous components.

5 ways to avoid Prop Drilling

1. Using Context API
2. using Redux
3. using Component Composition
4. using Callback Functions
5. Using Custom Hooks

Q46 What are class components in React?

1. Class Components are defined using JavaScript classes.
2. They are stateful components by using the lifecycle methods.
3. The render method in a class component is responsible for returning JSX.


import React, {Component} from 'react';

class AppClass extends Component{
    render(){
        return<h1>hello</h1>;
    }
}
export default AppClass;


Q47 How to pass data between class components in React?

this.props can be used in child component to access properties/data passed from parent component.


class ParentComponent extends Component{
    render(){
        const dataToSend = "hello from parent";
        return(
            <div>
                <ChildComponent message={dataToSend} />
            </div>
        );
    }
}
export deault ParentComponent;



class ChildComponent extends Component{
    render(){
        return(
            <div>
                <p>Message:{this.props.message}</p>
            </div>
        );
    }
}

export default ChildComponent;

//output: Message: hello from parent



Q48 What is the role of this keyword in class components?

this keyword is used to refer to the instance of the class.


Q49 What are the 5 differences btw Functional components & class components? 

Functional Component                                                     Class Component

1. Syntax: Defined as JS function.                                      1. Defined as a JS(Es6) class.
2. State: Orginally stateless but can now maintain state using hooks.   2. Can Manage local state with this.state.
3. Lifecycle methods: No                                                3. Yes
4. Readbility: more readable & Concise.                                 4. Verbose(complex).
5. this keyword: No                                                     5. Yes(Access props using this.props)
6. Do not have render method.                                           6. have render method.


React- 6 Routing

Q50 What is Routing and Router in React?
Routing: Routing allows you to create a single-page web application with navigation, without the need for a full-page refresh.
React Router: React Router is a library for handling routing and enables navigation and rendering of different component based on the URL.


Q51 How to implement Routing in React?
Command to install router:
npm install react-router-DOM

Step1: Install React Router
Step2: Create navigation
Step3: Create Routes


Q52 What are the roles of <Routes> & <Route> component in React Routing?
The <Routes> Component is used as the root container for declaring your collection of routes.
The <Route> component is used to define a route and specify the component that should render when the route matches.
for example, if user enter websitename.com/about in url then matching "About" component will be rendered.

Q53 What are Route Parameters in React Routing?
Route parameters in React Router are a way to pass dynamic values(data) to the component as part of the URL path.

// userId is the route parameters
<Route path="/users/:userId" component={userProfile}/>


Q54 What is the role of Switch Component in React Routing?
Switch component ensures that only the first matching<Route> is rendered and rest is ignored.
Example: Switch is commonly used to handle 404 or not found routes.

Q55 What is the role of exact prop in React Routing?
exact prop is used with the <Route> component to match exactly to the provided path.

//with exact
//only match about
<Route path="/about" exact component={About} />     note: not supporting "/anout/team, /about/contact 


React- 7 Hooks -useState/useEffect

Q56 What are React Hooks? What are the Top React Hooks?
1. React Hooks are inbuilt functions provided by React that allow functional components to useState and lifecycle features.
2. Before Hooks, class components lifecycle methods were used to maintain state in React Applications.
3. To use React hook first we first have to import it from React Library.

//import React, {UseState} from "react":
useState: State
UseEffect: side effects
useContext: Context
useReducer: Complex State
useCallback: Memoization
useMemo: Performance
useRef: Refs  
useLayoutEffect: Synchornous Side effects.


Q57 What are State, Stateless, Stateful and State Management terms?
"state" refers to the current data of the component.
Stateful or statemanagement means, when a user performs some actions on the UI, then the React application should be able to update and re-render that data or state on the UI.


Q58 What is the role of useState() hook and how it works?

The useState hook enables functional components to manage state.
useState() working: useState() function accept the initial state value as the parameter and returns an array with 2 elements:
1. The first element is the current state value(count in this code).
2. Second element is the function that is used to update the state(setCount in this code).
The concept of assign array elements to individual variables is called array destructing.

import React, {useState} from "react";
function UseState(){
    //array destructing
    const [count, setCount] = useState(0);
    const increment = () =>{
        setCount(count + 1);
    }
}

return (
    <div>
    <p>Count:{count}</p>
        <button onClick={increment}>Click</button>
    </div>
);
export default UseState;


Q59 What is the role of useEffect(). How it works & what is its use?

The useEffect Hook in React is used to perform side effects in functional components.
For example, data fetching from API, subscriptions or any other operation that needs to be performed after the component has been rendered.

Q60. What is useEffect() hook and when to use it?
useEffect()  is called after the component renders. Example: side effects.
useEffect() function will accept 2 parameter: (Effect function, dependency array)

Q61 What is Dependency Array in useEffect() hook?
Dependecies array(optional) act as triggers for useEffect to rerun;meaning if any of the dependencies values change, the code inside useEffect() will be executed again.
Ex: userId --> due to multiple dependencies

Q62 What is the meaning of the empty array[] in the useEffect()?
An Empty array[] indicates that the effect function should only run once.

React- 8 Hooks -useContext/useReducer

Q63 What is the role of useContext() hook?
useContext in React provides a way to pass data from parent to child component without using props.
avoid prop drilling.


Q64 What is createContext() method? what are Provider & Consumer Properties?
createContext() function returns an object with Provider and Consumer properties.
The Provider property is responsible for providing the context value to all its child components.
useContext() method or Consumer property can be used to consume the context value in child components.


Q64 When to use useContext hook instead of props in real application?
Use useContext instead of props when you want to avoid prop drilling and access context values directly within deeply nested components.

Props are good from component 1 --> component 2
useContext is good for multiple components  Ex: Comp1--> Comp2--> Comp3 -->Comp4

Advantages:
1. Theme Switching(Dark/Light): you can centralize and pass the theme selection of the application from the parent to all the deep child components.
2. Localization(language selection): you can centralize and pass the language selection of the application from the parent to all the child components.
3. Centralize Configure settings: Common configuration settings like API endpoints can be centralized and change in the parent component will pass the setting to all its child components.
4. User Preferences: Any other user preferences apart from theme and localization can also be centralized.
5. Notification System: Components that trigger or display notifications can access the notification state from the context.

React- 11 Component LifeCycle Method-1 

Q65 What are component life cycle phases? 3

Component Life cycle Phases.
1. Mounting Phase. (Component creation started) - This phase occurs when an instance of a component is being created and inserted into the DOM.
2. Updating Phase (Component updates): This phase occurs when a component is being re-rendered as a result of changes to either its props or state.
3. Unmounting Phase(Removal from the DOM): This phase occurs when a component is being removed from the DOM.


Q66 What are component life cycle methods?

Component lifecycle methods are special methods that get called at various stages of a component's life.
Mounting Phase:
=====================
1. constructor()
2. getDerivedStateFromProps()
3. render()
4. componentDidMount()

Updating Phase
====================
render()
componentDidUpdate()
getDerivedStateFromProps()
shouldComponentUpdate()
getSnapshotBeforeUpdate()

Unmounting Phase
========================
componentWillUnmount()



Q67 What are constructors in class components ? when to use them?

Mounting Phase
===============
Constructor()

constructor is a special method that is called when an instance of the class is created.
Constructor is used to intializing the component's state or performing any setup that is needed before the component is rendered.

Q68 What is the role of super keyword in constructor?

super keyword is used in the constructor of a class component to call the constructor of the parent class.
This is necessary to ensure that the initialization logic of the parent class is executed.

class ConstructorExample extends Component{
    constructor(props){
        super(props);

        //Initalize the State
        this.state = {
            count: 0,
        ;}
    }
    render(){
        return(
            <h2> Count:{this.state.count}</h2>
        );
    }
}

export default ConstructorExample;


Q69 what is the role of render() method in component life cycle?

Mounting Phase, Updating Phase -- render()

Render() method returns the React elements that will be rendered to the DOM.


Q70 How the state can be maintained in a class component?

Two step process to maintain state:

1. this.setState() method is used to update the state.
2. this.state property is used to render the update state in DOM.

class StateComponent extends Component{
    constructor(props){
        super(props);
        this.state = {
            count: 0; //initializing the state
        };
    }
    render(){
        return(
            <div>
                <h2>Counter: {this.state.count}</h2>
                <button onClick={this.handleInc}>Increment</button>
            </div>
        );
    }
    handleInc = () =>{
        this.setState((prevState)=>({
            count: prevState.count + 1,
        }));
    };
}

export default StateComponent;

Q71 What is the role of componentDidMount() method in component life cycle?

ComponentDidMount() lifecycle method in React is the part of mounting phase and is called after a component has been rendered to the DOM.
Mostly used for side effects. For example, external data fetching or setting up subscriptions.

Mounting Phase
===============
componentDidMount()

1. Rendered after constructor intialization.
2. Rendered after componentDidMount() to run side effects(ex: loading data from external API) and then call render() method of updating phase again.


React- 13 Controlled & Uncontrolled Components

Q72 What are controlled components in React?
A controlled component is a component whose form elements(like input fields or checkboxes) are controlled by the state of the application.


Q73 What are the differences btw Controlled & Uncontrolled components?

Controlled Components                                               Uncontrolled Components
1. Values are controlled by React State.                            1.Values are not controlled by React State.
2. Event handlers update React state.                               2. No explicit state update; values can be accessed directly from the DOM.
3. Don't depend on useRef()                                         3. Commonly uses useRef() to access form element values.
4. Re-renders on state changes.                                     4. Less re-rendering since values are not directly tied to React state.
5. A recommended and standard practice for form handling in React.  5. useful in certain scenarios but less commonly considered a best pratice.


Q74 What are characteristics of controlled components?

characteristics of controlled components:
1. State Control: The value of the form element is stored in the component's state.
2. Event Handling: Changes to the form element trigger an event(e.g., onChange for input fields)
3. State Update: The event handler updates the component's state with the new value of the form element.
4. Re-rendering: The Component re-renders with the updated state, and the form element reflects the new value.

Q75 What are the advantages of using controlled components in React forms?

Top 3 benefits of using controlled components in React forms:
1. In controlled components, form elements have their values managed by React State, ensuring a single source of truth.
2. This approach facilitated predicatable and synchronized updates, making it easier to implement features such as form validation, and dynamic rendering, and seamless integration with React's lifecyle methods.
3. Controlled Components offer better control and maintainability compared to uncontrolled components, making them the best pratice for handling forms in React applications.


Q76 How to handle forms in React?
The preferred and recommended approach for handling forms in React is by Using controlled components.


Q77 How can you handle multiple input fields in a controlled form?
Maintain separate state variables for each input field and update them individually using the onChange event.


Q78 How do you handle form validation in a controlled component?
By using conditional rendering based on the state and validate input values before updating the state.

Q79 In what scenarios might using uncontrolled components be advantageous?
Uncontrolled components can be beneficial when integrating with non-React libraries, or when dealing with forms where controlled components are not possible.


*** React- 14 Code Splitting 

Q80 What is code splitting in React?
Code splitting is a technique to split the JavaScript bundle into smaller chunks, which are loaded on-demand.

Q81 How to implement code splitting in React?
3 steps for code splitting in React:
1. Use React.lazy() to lazily import components.
2. wrap components with Suspense to handle loading.
3. Configure your build tool(e.g webpack) for dynamic imports.

Q82 What is the role of Lazy & Suspense methods in React?
React.lazy is a function that allows you to load a component lazily.
It enables code splitting by allowing you to import a component asynchronously/dynamically, meaning component is loaded only when needed only.

The Suspense component is used to display a fallback UI while the lazily loaded component is being fetched.


Q83 What are the Pros & Cons of code splitting?

5 Pros of Code Splitting:
1. Faster Initial Load Time:  Code splitting reduces the initial load time of your application by only loading the necessary code for the current view or feature. Good for performance.
2. Optimized Bandwidth Usage: By Loading only, the code needed for a specific page, it reduces the amount of data transferred over the network. Good for slow network.
3. Improved caching: Smaller, more focused code chunks are more likely to be cached by the browser.
4. parallel loading: Multiple smaller chunks can be loaded simuntaneously, leading to faster overall loading times.
5. Easier Maintenance: Code splitting can make your codebase more modular, independent and easier to maintain.

5 Cons of code splitting:
1. Complexity: Implementing code splitting introduces additional complexity to your application. This complexity can make the development process slow.
2. Tooling Dependecies: Proper code splitting often requires specific build tools and configurations, such as Webpack and Babel. Managing these tools is challenging.
3. Potential for Runtime Errors: Dynamically loading code at runtime can introduce the possibility of runtime errors. careful testing is necessary to catch such issues.
4. Increased Number of Requests: Code splitting may increase the number of HTTP requests needed to fetch all the necessary chunks. This can impact performance.
5: Learning Curve: Developers who are new to code splitting may need time to understand the concepts and best practices. This can be a challenging.


Q84 What is the role of the import() function in code splitting?
The import() function returns a promise that allow dynamic loading of modules.

Q85 What is the purpose of the fallback prop in Suspense?
The fallback prop provides a loading indicator or UI while the dynamically imported component is being loaded.

Q86 Can you dynamically load css files using code splitting in React?
Yes, using dynamic import() for CSS files allows you to load styles on-demand along with the corresponding components.

Q87 How do you inspect & analyze the generated chunks in React application?
Use tools like Webpack Bundle Analyzer to analyze the size and composition of chunks.

*** React- 15 Others

Q88 What is a higher-order component in React?
A Higher-Order Component is a component which takes another component as an argument and adds extra features to another component.
HOC can be used for providing logging functionality to all the components in a reusable way.


Q89 What are the 5 Ways to Style React components ? Explain inline styles?

we use separate style sheets.
5 ways to style React components
1. Inline styles
2. CSS Stylesheets
3. CSS-modules
4. Global Stylesheets
5. CSS Frameworks


Q90 What are the difference between React & React Native?

React                                                           React Native
1. React is a library.                                          1. React Native is a framework.
2. React is used for building web interfaces.                   2. React native is used for building mobile applications.
3. Run on web browsers.                                         3. Run on IOS and Android platforms.
4. HTML and CSS are used for UI.                                4. Native UI Components(e.g., View, Text) are used for UI.
5. Deployed as web applications.                                5. Deployed through app stores(e.g., App store, Google Play)


Q91 What is GraphQL?
GraphQL is a query language for APIs(Application Programming Interfaces) and a runtime for executing those queries with your exisitng data.
GraphQL and React are often used together. React components can use GraphQL queries to fetch the data required for rendering.

Q98 What are the Top 3 ways to achieve state management? when to use what in React?
1. useState Hook: 
    When to use: Simple component-level state.
    Reason: Ideal for applications having small components and isolated state because it is Lightweight and built into React only.
2. Context API:
    When to use: Prop drilling avoidance for sharing global data.
    Reason: Simplifies data passing through the component tree, reducing the need for manual prop drilling.
3. Redux:
    When to use: Large-scale applications with complex state.
    Reason: Centralized store and actions provide a predicatable state management pattern, aiding in debugging and scalability.

Q92 How can you implement authentication in a React application?

Front-end/Client-side                                               Middleware/server-side/backend(node.js, asp.net, django)

browser                     1. POST:{username, password}           2. authenticate & create JWT Token
                            3. Return Response {JWT token}
4. Store JWT token at local storage
                            5. Request Data{JWT token: Header}     6. Validate token signature

                            7. Send Data
8. Display data on browser

Q93 What is the use of React Profiler?
React Profiler is a set of tools in React that allows developers to profile(analyze) the performance of a React application.


Q94 What is the difference between Fetch & Axios for API calls in React?

Fetch                                                                                                   Axios
1. fetch is a built-in JS function, so doesn't require any additional libraires.                        1. Axios is a third-party library, that simplifies the process of making HTTP requests.
2. fetch returns Promises, making it easy to work with asynchromous code using async/await syntax.      2. Axios allows you to use interceptors, which can be good for tasks like request/response logging, authentication, and error handling.
3. If you want to keep http requests simple, fetch is a good choice.                                    3. If you want to intercept http request/response or improve error handling then Axios has more features to do it.


Q95 What are the popular Testing Libraries for React?

Jest
React Testing Library
Enzyme
Cypress

Q96 How can you Optimize Performance in React application?
1. Memoization with useMemo and useCallback:  Use this hooks to memoize values and, reducing unnecessary recalculations.
2. Optimizing Renders with React.Fragment: Use it to avoid unnecessary wrapper elements that could cause additional DOM nodes.
3. Lazy loading with React.lazy: Use it to load components lazily, reducing the intial bundle size and imporving intial loading performance.
4. Code splitting: Employ code splitting to divide your application into smaller chunks that are loaded on demand, improving initial load times.
5. Optimizing Images and Assets:  Compress and optimize images, use responsive images and leverage lazy loading for images to reduce network and rendering overhead.


Q97 Explain Reactive Programming with example?
Reactive programming is a programming paradigm that focuses on reacting to changes and events in a declarative and asynchronous manner.
Ex: Google search type --> gives hints --> events are captured.

Declarative means a programming style where you write the code for what you want to achieve, rather than specifying step-by-step how to achieve it.
For Ex: JSX in React has declarative syntax.

Asynchronously means an action that doesn't block other actions.

Q98 In how many ways can we implement Reactive Programming in React?

1. State and Props: Reacting to changes in local component state and passing data reactively through props.
2. React Hooks: Leveraging useState and useEffect hooks for managing state and side effects in functional components.
3. Event Handling: Reacting to user interactions through event handling and updating state accordingly.
4. Context API: sharing and managing global state reactively across components using the Context API.
5. Redux: using state management libraries like Redux for managing complex application state reactively.
6. Component LifeCycle Methods: Using class components and lifecycle methods for handling side effects and updates.
7. Async/await: utilizing async/await syntax for handling asynchronous operations reactively.
8. RxJS and Observables: Levering RxJS for handling aysnchronous operations and data streams in a reactive manner.

Q99 How to pass data from child component to parent component in React?
Parent provides a callback function to child and then child component can then invoke this callback to pass data back to the parent.


======================================================================================================================================

ReactJS Interview Question and Answers

1. What is react.js?
   React is an open-source Javascript library developed for building user interfaces, particularly for single-page applications.

2. What are the major features of react?
   Virtual DOM: React uses a virtual DOM to improve performance by minimizing direct DOM manipulations.
   JSX: JSX stands for Javascript and XML, which allow writing HTML in React components.
   Components: React is Component-based, meaning the UI is built using reusable components.
   One-way Data Binding: Data flows in one direction, making the application easier to understand and debug.
   High Performance: React Optimizes updates by using a virtual DOM and efficently re-rendering components.
   Undirectional Data Flow: Data flows in a single direction, which provides better control over the entire application.

3. What is Virtual DOM and how it works?

Virtual DOM is a lightweight, in-memory representation of the real DOM elements generated by React Components.
React keeps a copy of the actual DOM structure in memory, called the virtual DOM, and uses it to optimize updates and rendering.

Rendering -----> Updating ----> Diffing Algorithm -----> Batch Updates -----> Reconciliation

4. What are components in react?
Components are the building blocks of a React application. They are reusable pieces of UI that can be nested, managed, and handled independently.
Class Based Components 
Functional Components

5. Explain Class components with example?

class nameofComponent extends component then render method return JSX.

import React, {Component} from 'react;
class ClassComponentExample extends Component {
    render(){
        return <h1>Hello</h1>;
    }
}
export default ClassComponentExample;

4. Explain functional components with example?

2-ways

import React from 'react';

function FunctionalComponent() { // function keyword
    return <h1>Hello</h1>
}
export default FunctionalComponent;

import React from 'react';
const FunctionalComponent = () => { //const arrow function
    return <h1>hello</h1>
}
export default FunctionalComponent;

5. What is JSX?
JSX stands for Javascript XML.
It allows us to write HTML elements in Javascript and place them in the DOM without using methods like createElement() or appendChild().

6. How to export and import components?
we can export components using export default or named exports, and import them using import.
inorder to reuse a component we need to export.

exportcomponent1.js

import react from "react";

const Home = () =>{
    return <h1>Home!</h1>;
};

export default Home;


=================

importcomponent1.js

import React from "react";
import Home from "./home";

const App = () =>{
    return (
        <div>
        <Home />
        </div>
    );
};

export default App;

7. How to use nested components?

Header component --> common for layout. <Menu /> is nested inside header.
App Component --> nested <Header /> component

8. What is state in react ?

button --> counter value  1-->2 --> 3 value is stored in state.

In React, state is an object that represents the parts of the app that can change. 
Each component can have its own state, which can be managed within the component and used to render the UI.
When the state changes, React re-renders the component to reflect the new state.

9. What is state in react?

import React, {Component} from "react";
//class based component
class Counter extends Component {
    constructor(props){
        super(props);
        //Initializing state
        this.state ={
            count: 0;
        };
    }
    render() {
        return(
        <h1>Count: {this.state.count}</h1>
        );
    }
}
export default Counter;


-----------------------------
//functional based component
import React, {useState} from "react";  //useState
function Counter(){
    //Initializing state using useState Hook
    const [count, setCount] = useState(0);  //update state with setCount

    return (
        <h1>Count: {count}</h1>
    );
}
export default Counter;

=========================================
//class component
import React, {Component} from "react";
class Counter extends Component {
    state = {
        count: 0
    }
    render(){
        return(
            <h1> Count: {this.state.count}</h1>
        )
    }
}
export default Counter; toow  


10. How to update state in react?
State in React is updated using the setState method in class components or the useState hook in functional components.
// class
this.setState({count: this.state.count + 1})

//functional
const [count, setCount] = useState(0);

11. What is setState Callback?
The setState method can accept a callback function as the second argument, which is executed once the state has been updated and the component has re-rendered.

12. Why you should not update state directly, explain wiht example?
Updating state directly does not trigger a re-render of the component, leading to inconsistencies in the UI.
Instead, always use setState (class-based) or state(functional-based) hooks.

13. What are props in react?
Props(properties) are used to pass data and event handlers to child component.(communicate b/w components)
props ensure a one-way data flow, from parent to child.
props cannot be modified by the child component that receives them. (read-only)

Example:
import React from "react";

//child component
function Greeting(props){
    return <h1>hello, {props.name}!</h1>
}

//parent component
function App(){
    return(
        <div>
        <Greeting name="vijay" />
        <Greeting name="krishna" />
        </div>
    );
}

export default App;
==============================

14. What is difference between state and props ?

       state                                            
    State is built-in object used to store data that may change over the lifecycle of a component.
    It is managed within the component itself.

    State is mutable. 
    It can be updated using the setState method in class components or the useState hook in functional components.

    State is local to the component and cannot be accessed or modified by child components.

    Props
    Props(properties) are used to pass data from a parent component to a child component.
    They are read-only and immutable within the child component.

    Props are immutable. Once passed to child component, they cannot be modified by the child.

    Props are passed from parent component to a child component and can be accessed by the child.


15. What is lifting state up in react?
Lifting State Up is a pattern in React where state is moved up to the closest common ancestor of components that need to share that state.
Single Source of Truth: By managing the state in the parent component, you can ensure that the state is consistent across multiple child components.
Simplified State Management: The state logic is centralized, making it easier to maintain and debug.

Parent <----- child (button). Manage state in single parent component.

16. What is children prop in react?
The children prop is a special property in React used to pass the content that is nested inside a component.

Child Component --> {props.children}
Parent Component --> App() <h1> <p><h2><button>

17. What is defaultProps in React?
defaultProps is used to set default values for the props in a component.

Greeting.defaultProps ={
    name: "Guest",
}
//usage
<Greeting /> //renders "hello, guest"

18. What are fragments in react and its advantages?
Fragments allow you to group multiple elements without adding extra nodes to the DOM.
<React.Fragment>
<li>Item, 1</li>
<li>Item 2</li>
</React.Fragment>
<>
</>

19. How to use styling in react.js?
we can ise inline styles, CSS stylesheets, or CSS-in-JS libraries like styled-components.

inline styles
function StyledComponent(){
    return(
        <div
        style={{
            color: "blue",
            backgroundColor: "lightgray"
        }}>
        This is Styled Component.
        </div>
    );
}


styles.css
.container{
    color: blue,
    backgroundColor: lightgray
}
import "./styles.css"
function StyledComponent(){
    return <div className = "container"> this is styled component</div>;
}

20. How can you conditionally render components in React?
We can use Javascript conditional operators (like if, &&, ?:) to conditionally render components.

21. How to render list of data in react?
we can use the map function(ES6) to iterate over an array and render each item.

22. What is Key prop?
The key prop is a unique identifier for each element in a list, used by React to identify which items have changed, are added, or removed.


23. Why indexes for keys are not recommended?
Using indexes as keys can lead to performance issues and unexpected behavior when list items are reordered or removed.
Keys should be unique and stable.

24. How to handle buttons in react?

25. How to handle inputs in react?
we can use controlled components where form data is handled by the component's state.

26. Explain lifecycle methods in react?
Lifecycle methods in React are special methods that get called at different stages of component's lifecycle.
Mounting: When a component is being inserted into the DOM.
Updating: When a component's state or props change.
Unmouting: when a component is being removed from the DOM.

class LifecycleDemo extends React.Component{
    componentDidMount(){
        console.log("component mounted"); //render once only.
    }
    componentDidUpdate(prevProps, prevState){ //gives prevProps and prevState
        console.log("component updated"); 
    }

    componentWillUnmount(){
        console.log("component will unmount"); //cleanup things
    }

    render(){
        return <div> Lifecycle method</div>
    }
}

27. What are the popular hooks in react and explain it's usage?

useState: Manages state in functional components.
useEffect: Manages side effects in functional components.
useContext: Consumes context in functional components.
useReducer: Manage state with a reducer function, For More complex state management.
useRef: Accesses DOM elements or stores mutable values.
useCallback: performance improvement usecase
useMemo: performance improvement usecase.

28. What is useState and how to manage state using it?

import React, {useState} from 'react';

function Counter(){
    const [count, setCount]= useState(0);

    return(
        <div>
        <p> you clicked {count} times</p>
        <button onClick={()=>setCount(count+1)}>Click Me</button>
        </div>
    );
}
export default Counter;

29. What is useEffect hook and how to manage side effects?
useEffect is a hook that manages side effects like data fetching(prevState), subscriptions, or manually changing the DOM.

import React, {useEffect, useState} from 'react';

function DataFetcher(){
    useEffect(()=>{}, [], []); //Empty array means this effect runs only once.

    useEffect(()=>{}, [dependency]); //run if dependency value changes.

  useEffect(()=>{
    return ()=>{};

  }, []) //cleanup method.
  retunr <div></div>;
}
export default Counter;


30. How to implement data fetching in react.js?
ask interviewer question--> how to implement onClick on page load?

31. How to manage loading state?
const [loading, setLoading] = useState(false);

32. What is prop drilling and how to avoid it? What is ContextAPI?
Prop drilling occurs when you pass data through many layers of compoments.
It can be avoided using the Context API or state management libraries like Redux.

A ---> B, C--> D, A-->D.

33. What is Context API in React, and why is it used?
Context API in React provides a way to share values(like data or functions) between components without having 
to pass props through every level of the component tree. It is used to avoid the prop drilling.

import React, {createContext} from 'react';

//create a Context
const MyContext = createContext();

//Provider component

//wrap context in root component.

// A, B, C, D
global state

34. How do you consume context using the useContext hook?
The useContext hook allows functional components to access context values directly.

35. How can you update context values?
//create context
//provider component
//pass context name
//update value by onClick() function.

36. How do you use multiple contexts in a single component?
//we need to wrap multiple context
//useContext(firstContext) and secondContext.

37. What are the advantages of using the Context API over prop drilling?
Context API reduces the need for prop drilling, making the code more readable and maintainable.
It allows for easy sharing of state and functions across the component tree without passing props through every level.

//without Context API(prop drilling)
<Parent>
<Child>
<GrandChild value={value} />
</Child>
</Parent>


//with Context API
<MyProvider>
    <GrandChild />
</MyProvider>


38. What is the useReducer hook, and when should you use it?
The useReducer hook is used for state management in React. 
It is suitable for handling more complex state logic compared to useState.

useReducer alternate of useState.

import React, {useReducer} from 'react';

const[state, dispatch] = useReducer(reducer, initialState);
//dispatch action with type property


39. Can you useReducer with complex state objects?
yes.

40. how do you pass additional arguments to the reducer function?

whenever we dispatch action using payload.

dispatch({type: 'update', payload:{value:42}});

41. How to do you handle side effects with useReducer?
Yes
we can useEffect inside the API call with data action.payload.

42. What is useRef Hook?

The useRef hook is used to access and interact with DOM elements directly
and to persist mutable values across renders without causing re-renders.


43. How can useRef be used to store mutuable values?
useRef can store any mutuable values, and changes to the ref do not cause re-renders.

44. What is forwardRef and when would you use it?
forwardRef is a function that allows you to pass refs through components to access DOM elements or child component instances.

45. How to manage forms in react?
Forms in React can be managed using controlled components where form data is handled bu the component's state.

//create JSX structure with form.

46. What are Custom Hooks and why do We Need Them?

Custom Hooks in React are JavaScript functions that allow you to reuse stateful logic across multiple components.
They enable you to extract and share common logic without repeating code, promoting code reusability and separaration concerns.

c1, c2, c3. c4.c5--> one custom hooks --> state
Advantages:
Code Reusability: Custom hooks allow you to reuse stateful logic without duplicating code.
Separation of Concerns: They help spearate the logic from the component's structure, making the code more modular and easier to maintain.
Cleaner Code: By Moving common logic into custom hooks, components become cleaner and more focused on their core responsibilites.

47. Implement useFetch custom hook/Custom hook example?

48. Implement useWindowResize custom hook?


49. What is React Router DOM and why is it used?

React Router DOM is a routing library built on top of React Router. 
It enables dynamic routing in web applications, allowing you to define routes and naviagte between different components without reloading the page.

Routing Version 6 latest.
moving 1 page to another page --> routing.

50. How do you create a basic route in React Router DOM?
A basic route is created using the Route component, which maps a URL path to a specific element.
<Route path = "/home" element = {<Home />} />

51. How to implement basic routing using react router dom?

file --> index.js

import {BrowserRouter, Routes, Route} from 'react-router-dom';

const App = () => (
    <BrowserRouter>
        <Routes>
            <Route path="/home" element={<Home />} />
            <Route path="/login" element={<Login />} />
        </Routes>
    </BrowserRouter>
);

export default App;

52. How to create a link to another route using React Router DOM?
Use the Link component to create navigation links.
import {Link} from 'react-router-dom';

<Link to="/home">Home</Link>
<Link to="/about">About</Link>

53. How do you use URL parameters/ Dynamic routing in React Router DOM?

/product list
1, 2,3, 4,5
<Route path="/user/:userId" element={<User />} />

54. How can you perform a redirect in React Router DOM?
use the Navigate component to perform a redirect.
<Navigate to="/home">;
//use navigate and to property


import {Navigate} from 'react-router-dom';

const Login = ()=>{
    const isLoggedIn = true;
    if(isLoggedIn){
        return <Navigate to="/home">;
    }
    return <div> please login</div>;
}

export default Login;

55. What is a Routes component on React Router DOM?
The Routes component is used to define a set of routes, where only the first matching route is rendered.

<Route path="/home" element={<Home />}

56. How do you handle nested routes in React Router DOM?

<Routes>
    <Route path="/dashboard" element={<Dashboard />}>
    <Route path="/home" element={<Home />}
</Routes>

57. How can you handle 404 errors (not found) in React Router DOM?
Use a Route without a path prop inside Routes to catch all unmatched routes.

const NotFound = () => <h1> 404-not found</h1>;

<Route path="*" element={<NotFound />}/>

58. How do you programtically naviagte using React Router DOM?
Use the useNavigate hook to navigate programtically within your components.

import {useNavigate} from 'react-router-dom';

const navigate = useNavigate();
navigate('/home');

59. Explain useCallback hook with example?
//callback function
The useCallback hook is used to memoize callback functions. 
This means that the function provided to useCallback will only be recreated if one of it dependencies has changed.
This is particularly useful when passing callbacks to child components that are optimized with React.memo, as it can prevent unnecessary renders.

60. Explain useMemo hook with example?
The useMemo hook is used to memoize expensive calcualtions so that they are not recalculated on every render.
It takes a function to compute a value and an array of dependencies, and it onlyy recomputes the value when one of the dependencies has changed.

//value

61. Explain React.memo with example?
React.memo is a higher-order component that memoizes the result of a component.
It prevents the component from re-rendering unless the props have changed. 
This is useful for optimizing performance by avoiding unecessary renders of pure components.

62. Explain the Reconciliation process in React and how it works?
Reconciliation is the process React uses to update the DOM efficiently.
It involves comparing the new Virtual DOM with the previous one and determining the minimum number of changes needed to update the actual DOM.

63. What are Pure Components?
PureComponent is a base class in React that implements shouldComponentUpdate with a shallow prop and state comparison.
It helps prevent unnecessary re-renders by ensuring that the component only re-renders when there are actual changes in props or state.

class childComp extends PureComponent{
    //class based components
}

64. Explain higher order component with example?
A Higher-Order Component (HOC) is a function that takes a component and returns a new component with added functionality.
HOCs are used for reusing component logic and enhancing components with additional behavior.

65. What is redux, explain core principles?
//state management(centralized store)
Redux is a predicatable state container for JavaScript apps. Redux acts as centralized store for state management in your application.
Advantages:
Single Source of Truth: The State of the application is stored in a single object.
State is Read-Only: The only wat to change the state is to emit an action, an object describing what happened.
Changes are made with Pure Functions: Reducers are pure functions that take the previous state and an action, return the next state.

66. What are actions in Redux, explain with example?
Actions are plain JavaScript objects that describe what happened in the application.
They must have a type property that indicates the type of action being performed.

//action.js
export const increment = () => ({type: 'INCREMENT'});
export const decrement = () => ({type: 'DECREMENT'});

67. Explain Reducers in Redux with an example?
Reducers are pure functions that take the current state and an action , and return a new state based on the action type.

const counterReducer = (state = intitialState, action)=>{
    switch(action.type){
        case 'INCREMENT':
        return {count: state.count +1};
        case 'DECREMENT':
        return {count: state.count - 1};
        default:
        return state;
    }
}

68. What is the role of the Redux Store?
The Store holds the whole state tree of the application. 
It allows access to the state via getState(), dispatching actions via dispatch(action), and registering listeners via subscribe(listener).


69. How do you connect React components to Redux store using connect?
The connect function connects a React component to the Redux store.
It maps state and dispatch to the component's props.

import { connect } from 'react-redux';

const mapStateToProps = (state) => ({count: state.count});
const mapDispatchToProps = {increment};

export default connect(mapStateToProps, mapDispatchToProps)(Counter);

70. How do you use the useSelector and useDispatch hooks in a functional React component?
useSelector is used to access the Redux state,
const count = useSelector((state)=>state.count)

useDispatch is used to dispatch actions in functional components.

const disptach = useDispatch();

71. What is Redux Toolkit?
Redux Toolkit is an offical, opinionated toolset for efficient Redux development.
It simplifies store setup, reduces boilerpate, and includes useful tools like createSlice and createAsyncThunk.

72. How to configure store in redux toolkit?
Redux Toolkit is an official, opinionated toolset for efficient Redux development.
It Simplifies store setup, reduxes biolerplate, and includes useful tools like createSlice and createAsyncThunk.

import {configureStore} from '@reduxjs/toolkit'; //import
const store = configureStore({
    reducer:{
        //pass all reducers
    },
});

export default store;

73. Explain createSlice in Redux Toolkit with an example?
createSlice is a function that generates action creators and action types, and create a reducer based on a object of "slice" reducers.

import {createSlice} from '@reduxjs/toolkit';

74. What are controlled components in React?
Controlled components are React components where the form data is handled by the React state.
The input's value is always driven by the React state.

75. What are uncontrolled components in React?
Uncontrolled components are React Components where the form data is handled by the DOM itself.
The input's value is not driven by the React state.

76. How do you optimize performance in React applications?
    Using useMemo and useCallback to memoize expensive calculations and functions.
    Implementing shouldComponentUpdate or using React.memo for Pure Components.
    Code Splitting and lazy loading.

77. What is code splitting in React?
Code splitting is a feature supported by React that allows you to split your code into various bundles which can then be loaded on demand.

import React, {Lazy, Suspense} from 'react';

<Suspense> provides fallback

78. What are render props in React? give an example?
Render props are a technique for sharing code between React components using a prop whose value is a function.
This function returns a React element and is used by the component to render part of its output.

79. What are portals in React?
Portals provide a way to render children into a DOM node that exists outside the DOM hierarchy of the parent component.
This is useful for things like modals, tooltips and overlays.

80. How do you implement lazy loading in React?
Lazy loading in React can be implemented using the React.lazy and Suspense components.
This allows you to load components on demand, improving initial load times.

81. How do you define props for a functional component in Typescript?

interface Props{}
const MyComponent: React.FC<Props>=({title, count}=>{})

82. How do you use the useState hook with Typescript?
We can define the type of the state variable by specifying it in the useStata generic.

const [count, setCount]= useState<number>(0);

83. How do you type event handlers in React with Typescipt?

const [value, setValue] = useState<string>('');

const handleChange = (e: React.changeEvent<HTMLInputElement>)=>{}
                                           <TextField> <Selectfield>


84. How do you handle optional props in React components with Typescript?
In Typescript, you can handle optional props by using the ? operator in the props interface or type alias.

interface Props{
    subtitle?: string;
}

85. How do you use the useReducer hook with Typescript?

86. How do you type the context API in React with Typescript?

87. How do you write a simple test in Jest?
Jest is a JavaScript testing framework maintained by Facebook. 
It is commonly used with React because it provides a simple and powerful testing solution with features like 
snapshot testing, coverage reporting, and built in assertions.

//JEST, RTL

test() or it() callback function.

88. How do you render a component for testing using React Testing Library?

import {render} from '@testing-library/react';
import MyComponent from './MyComponent';
test('renders MyComponent', ()=>{
    render(<MyComponent />);
});

89. How can you find elements in the DOM using the React Testing Library?

You can find elements in the DOM using React Testing Library by using query functions like:

getByText – Finds elements by visible text

getByRole – Finds elements by their ARIA role

getByLabelText – Finds form inputs by associated label

getByPlaceholderText – Finds inputs by placeholder

getByTestId – Finds elements using a data-testid attribute

90. How do you simulate user events in React Testing Library?

You simulate user events in React Testing Library using the userEvent utility (from @testing-library/user-event). 
It allows you to mimic real user interactions like clicking, typing, or selecting:

91. How can you test component props with React Testing Library?
You can test component props with React Testing Library by rendering the component with the desired props and asserting the 
expected output or behavior using queries like getByText, getByRole, etc. Props are tested indirectly through their effect on the UI.

92. create a Controlled Input Component?

93. Implement toggle Visibility of a component?

94. Fetch Data from an API and Display it, along with loading state?

95. Create a Reusable Button Component with Props?

96. Build a Component that Uses and Effect to Perform Cleanup.

97. Implement a context with a Reducer for Global State Management?

98. Build a Component with Conditional Rendering Based on Props.

99. Implement a simple form Component?

100. how to handle error in simple form component?

To handle errors in a simple React form, use useState to track form values and errors. 
Validate inputs on submit, update the errors state, and conditionally display error messages. 
This ensures form fields are validated and feedback is shown to users.

101: 
React.js drawbacks:

Steep learning curve for beginners due to its ecosystem.

Boilerplate and config overhead for setup.

Frequent updates can break code.

JSX may feel unnatural to some.

Performance issues if not optimized.

Lacks built-in solutions (routing, state management).

SEO limitations without SSR tools like Next.js.

Debugging complexity in large apps.

Large bundle sizes if not managed.

Not a full framework, relies on third-party tools.

======================================================

 Frontend (Angular, TypeScript, CSS/SASS)
1. What are key differences between Angular services and components?
    Answer:
    Components control views and handle user interactions, while services contain business logic and reusable code. Services are injected using Angular’s DI system and help with separation of concerns (e.g., data fetching or caching logic).

2. How do you manage shared state across components in Angular?
    Answer:
    Using a shared service with RxJS subjects/observables or NgRx for complex state management. For example:


    private userSubject = new BehaviorSubject<User | null>(null);
    user$ = this.userSubject.asObservable();

3. What’s the benefit of OnPush change detection?
    Answer:
    OnPush improves performance by limiting change detection to when input references change or observables emit. This prevents unnecessary DOM updates in large applications.

4. How do you organize large-scale Angular apps?
    Answer:
    I use feature modules, lazy loading, shared/core modules, and leverage Nx monorepo for workspace organization, shared libraries, and incremental builds/testing.

Backend (Node.js + NestJS + GraphQL)
5. How is NestJS different from Express?
    Answer:
    NestJS is a higher-level framework built on Express (or Fastify), following Angular-style architecture (modules, DI, decorators). It enables cleaner structure, scalability, and built-in support for GraphQL, WebSockets, and validation.

6. How do you handle authentication in NestJS?
    Answer:
    Using @nestjs/passport with JWT strategy:

    Create an auth module.

    Use guards like JwtAuthGuard for protected routes.

    Inject Request.user using custom decorators.

7. How does a GraphQL resolver work in NestJS?
    Answer:
    Resolvers act like controllers in REST. They use decorators like @Query(), @Mutation(), and @ResolveField() to define schema behavior. DTOs define the types, and services contain the business logic.

8. What’s the difference between Query and Mutation in GraphQL?
    Answer:

    Query is for fetching data (read-only).

    Mutation is for writing or updating data (state-changing operations).

AWS / Cloud Infrastructure
9. How do you deploy a Node.js app using AWS ECS Fargate?
    Answer:

    Dockerize the app.

    Push image to ECR.

    Create ECS Task Definition.

    Use Fargate to run containerized service.

    Load balance via ALB; configure logs to CloudWatch.

10. When would you use Lambda vs Fargate?
    Answer:

    Lambda: Short-lived, event-driven tasks (e.g., image resize, API handlers).

    Fargate: Long-running services (e.g., backend APIs) that require container orchestration without managing EC2.

11. How do you implement caching using Redis (Elasticache)?
    Answer:
    Use Redis for storing frequently accessed data (e.g., user sessions or computed results):

    const cached = await redis.get('user:123');
    if (cached) return JSON.parse(cached);
    Fallback to DB and set Redis if not found.

12. What’s your approach to cost-tagging and cost optimization in AWS?

    Answer:

    Use cost allocation tags per environment/team.

    Schedule non-prod resources to shut down off-hours.

    Use CloudHealth or Cost Explorer to analyze usage.

    Prefer Lambda + S3 for static content/API when possible.

    Observability (Logging & Monitoring)


13. How do you implement observability in your applications?
    Answer:

    Structured logging using Winston or NestJS Logger.

    Logs shipped to Splunk using HTTP forwarders or Lambda log processors.

    Monitor metrics using CloudWatch or Datadog, and set up alarms.

    Instrument critical flows using tracing tools (like AWS X-Ray or OpenTelemetry).

    Monorepo Tooling (Nx)

14. What are the benefits of using Nx in a full-stack project?
    Answer:

    Efficient builds and caching.

    Code sharing across apps/libs (e.g., interfaces, utils).

    Dependency graph visualization.

    Supports both Angular frontend and NestJS backend in a single repo.

    General/Behavioral

15. How do you debug a full stack issue?
    Answer:

    Reproduce the issue locally.

    Use browser/network tools for frontend issues.

    Trace backend logs (e.g., in CloudWatch or Splunk).

    Use API Gateway/Lambda logs for serverless.

    End-to-end tracing if observability is set up.

    ==========================

1) Can you quickly introduce yourself and your skills?

I am a core UI Developer with 12+ years of experience building .com websites for different organizations using HTML5, CSS3, JavaScript, Angular 18, React.js, and Redux. 
In the past 2 years, I worked on the React migration team, where I converted the .net pages to react on united.com. 
Frontend is React, and used ATMOS (Own library) components used company wide.

Worked on Security features for users where they can manage there account like Forgot password, Forgot MileagePlus number, 
security questions, Sign-in features, Miles-Pooling, United Club pass,  Recent Activity, dashboard updates and 
KTN(Known Traveler Number), Accessibility guidelines features on united.com.

used middleware such as redux-saga to handle asynchronous tasks such as API calls, data fetching, and impure actions in a more organized and efficient way.

The new initiative worked on Miles-Pooling( points you get after traveling), TSA Precheck, Account security and management features, and Under18.

Previously worked with Accelerator team for Visa Inc. remediation of MBDA modules like Application Management, Account Management, Portfolio Management, Analytics, Recurring billing, Virtual Terminal, etc for bank users like Wells Fargo,  Bank of America, etc

Capital Group worked on DAVIS Project. Davis stands for Data visualization where we build different highcharts using react and integrate into the AEM., the backend is Java. Previously I worked on Creative Workbench, a writing tool where articles are published on capital group websites.

At Cerner Corporation worked on the medical examination forms.

In Office Depot worked on black Friday reporting.

Satinos Technologies created a tax portal and a schoomin website for the Vignan schools.

2) What versions of Angular have you worked on?
Answer:
I've worked with Angular 16, which includes features like standalone components, environment injector improvements, and better performance for large apps using hydration and signals.

3) What's the difference between JavaScript and TypeScript?
Answer:
TypeScript is a superset of JavaScript that adds static typing, interfaces, and advanced tooling support. 
It helps catch errors at compile-time and enables better code organization for large-scale apps.

4) Can you tell me the features of Angular 8?
Answer:

Differential loading for modern browsers

Lazy loading with dynamic imports

Builder APIs for custom CLI commands

Support for web workers

Improved TypeScript 3.4 compatibility

Opt-in Ivy preview

5) What are the building components of an Angular application?
Answer:

Modules (@NgModule)

Components (@Component)

Templates (HTML with Angular syntax)

Services (@Injectable)

Directives

Pipes

Routing configuration

6) What are the different types of directives in Angular?
Answer:

Component Directive: Has a template (e.g., @Component)

Structural Directives: Change DOM structure (e.g., *ngIf, *ngFor)

Attribute Directives: Change appearance or behavior of an element (e.g., ngClass, ngStyle, custom directives)

7) What is the purpose of ngOnDestroy?
Answer:
ngOnDestroy is a lifecycle hook used to clean up resources like subscriptions, intervals, or event listeners to prevent memory leaks when the component or directive is destroyed.

8) What is a selector in Angular?
Answer:
A selector is a string that identifies a component in templates. For example:


@Component({
  selector: 'app-user-card',
  ...
})
You use it like <app-user-card></app-user-card> in other templates.

9) Can you write a code snippet in Angular to display different divs based on the selection of radio buttons?
Answer:

html

<label><input type="radio" name="view" [(ngModel)]="selectedView" value="A"> A</label>
<label><input type="radio" name="view" [(ngModel)]="selectedView" value="B"> B</label>

<div *ngIf="selectedView === 'A'">This is View A</div>
<div *ngIf="selectedView === 'B'">This is View B</div>

ts

selectedView = 'A';

10) How can we handle multiple API calls and make another call based on their responses?
Answer:
Using RxJS forkJoin, switchMap, or concatMap:

ts

forkJoin([
  this.api.getUser(),
  this.api.getSettings()
]).pipe(
  switchMap(([user, settings]) => this.api.getDashboard(user.id, settings.theme))
).subscribe(response => {
  // Handle final response
});


11) What is the difference between Observable and Promise in JavaScript?
Answer:

Promise: Handles a single async value, resolves once.

Observable: Handles multiple values over time (streams), supports operators and cancellation.

12) Can you transform a list of employee objects to include only name and ID using RxJS?
Answer:

ts

this.api.getEmployees().pipe(
  map(employees => employees.map(emp => ({ id: emp.id, name: emp.name })))
).subscribe(filteredList => console.log(filteredList));

13) What steps would you take to address performance issues in an Angular application?
Answer:

Use OnPush change detection

Use trackBy with *ngFor

Lazy load modules

Optimize images and bundles

Avoid unnecessary API calls

Use pure pipes

Reduce DOM complexity

Use memoization for expensive calculations

14) How do you handle authentication while routing to another component in Angular?
Answer:
Using Route Guards:

ts
Copy
Edit
canActivate(route: ActivatedRouteSnapshot, state: RouterStateSnapshot): boolean {
  return this.authService.isLoggedIn();
}
Configure in routing module:

ts
Copy
Edit
{ path: 'dashboard', component: DashboardComponent, canActivate: [AuthGuard] }

15) How do you inject services into a component in Angular?
Answer:
Via constructor injection:

ts

constructor(private userService: UserService) {}
Angular injects the singleton instance of UserService if it’s provided in the module or @Injectable({ providedIn: 'root' }).

16) How do you handle communication between two components where actions in one component affect another component?
Answer:

Parent-Child: Use @Input() and @Output() for data flow and event emission.

Sibling/Unrelated: Use a shared service with RxJS Subjects to broadcast data:

ts

// In Service
private subject = new Subject<any>();
broadcast$ = this.subject.asObservable();
emitChange(data) { this.subject.next(data); }


17. What is AOT in Angular?
The Angular ahead-of-time (AOT) compiler converts your Angular HTML and TypeScript code into efficient JavaScript code during the build phase before the browser downloads and runs that code. 
Compiling your application during the build process provides a faster rendering in the browser.


AOT in Angular stands for Ahead-of-Time compilation. It's a compilation mode where the Angular application, including its templates
and components, is compiled into JavaScript code during the build process, before the application is deployed and run in the browser.
This contrasts with Just-in-Time (JIT) compilation, where the compilation occurs in the browser at runtime.



How do you perform routing in an Angular application?

Routing in Angular is done using the Angular Router. You define routes in a routing module using RouterModule.forRoot(), use <router-outlet> to load components, and navigate using routerLink or the Router service. Example:

ts
Copy
Edit
const routes = [
  { path: 'home', component: HomeComponent },
  { path: 'about', component: AboutComponent }
];
In template:

html
Copy
Edit
<a routerLink="/about">About</a>
<router-outlet></router-outlet>


===============================

Angular lifecycle hooks?

import { Component } from '@angular/core';
@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
    constructor(){
        //constructor will execute at booting time.
        //constructor will execute only once.
        //in general we will use constructor for dependency injection purpose
        //Ex. creating the objects to the services
        //we can use constructor for initializing the instance members
        console.log("in constructor");
    };

    ngOnChanges(){
        //after constructor Angular Framework gives the priortity to ngOnChanges life cycle hook.
        //when ever change detected on "@Input() properties", automatically this life cycle hook will execute
        //this life cycle hook may execute more than once based on Parent Component Changes.
        console.log("ngOnChanges");
    };

    ngOnInit(){
        //this life cycle hook is main life cycle hook
        //this life cycle hook will execute only once
        //this life cycle hook also called as first life cycle hook of component
        //this life cycle hook is used to write the main business logic
        //Ex.  making the subscriptions of Observables
        //     usage of directives
        console.log("ngOnInit");
    };


    ngDoCheck(){
        //when ever change detected in component properties at background, at that this life cycle hook will execute
        //this life cycle hook will execute more than one time.
        //this life cycle hook priority goes to after ngOnInit
        console.log("ngDoCheck");
    };

    ngAfterContentInit(){
        //when ever component receives the external data and renders with the help of directives, then this life cycle hook will execute
        //ngAfterContentInit life cycle hook will execute after ngDoCheck life cycle hook
        console.log("ngAfterContentInit");
    };

    ngAfterContentChecked(){
        //if external data verifies and renders successfully on Component , then this life cycle hook will execute
        console.log("ngAfterContentChecked");  
    };

    ngAfterViewInit(){
        //in general, we will use this life cycle hook to convert one data structure to another data structure for easy manipulations in Component
        console.log("ngAfterViewInit");
    };

    ngOnDestroy(){
        //before killing the component by angular framework then this life cycle hook will execute
        //in general, we will place clean up operations like unsubscribing the services, nullifying the variables
        console.log("ngOnDestroy");
    };

}




