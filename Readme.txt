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
