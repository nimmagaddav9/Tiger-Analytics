# Tiger Analytics Interview

# Introduction

**Can you quickly introduce yourself and your skills?**

I am a core UI Developer with 12+ years of experience building .com websites for different organizations using HTML5, CSS3, JavaScript, Angular 18, React.js, and Redux.

In the past 2 years, I worked on the React migration team, where I converted the .NET pages to React on united.com.  
Frontend is React, and used ATMOS (own library) components used company-wide.

Worked on security features for users where they can manage their account like Forgot Password, Forgot MileagePlus number,  
security questions, Sign-in features, Miles-Pooling, United Club pass, Recent Activity, dashboard updates and  
KTN (Known Traveler Number), Accessibility guidelines features on united.com.

Used middleware such as redux-saga to handle asynchronous tasks such as API calls, data fetching, and impure actions in a more organized and efficient way.

The new initiatives I worked on include Miles-Pooling (points you get after traveling), TSA Precheck, Account security and management features, and Under18.

Previously worked with the Accelerator team for Visa Inc. remediation of MBDA modules like Application Management, Account Management, Portfolio Management, Analytics, Recurring billing, Virtual Terminal, etc. for bank users like Wells Fargo, Bank of America, etc.

---

## 2. What is the architecture you followed in united?

_(Answer here)_

---

## 3. Why did you choose React.js?

We chose React.js because it offers a component-based architecture, making it easy to build reusable and maintainable UI components.  
Its virtual DOM improves performance, especially for dynamic and data-driven interfaces.  
React also integrates well with other libraries and tools, supports server-side rendering, and has a large community and ecosystem,  
which helped us deliver scalable, modern web applications faster.

---

## 4. Did you work on production related bugs?

Yes, I actively worked on production-related bugs. This included triaging issues reported by users or monitoring tools,  
reproducing them in lower environments, and providing quick yet stable fixes. I used tools like Chrome DevTools, Postman, and  
application logs (via CloudWatch or console logs) to debug issues. After identifying the root cause, I would implement fixes,  
test thoroughly, and push changes through the CI/CD pipeline to production with minimal downtime.  
I also updated Confluence documentation and communicated changes with QA and product teams to ensure smooth releases.

---

## 5. What is a State?

In React.js, state is a built-in object that stores dynamic data specific to a component.  
It allows components to respond to user input, server responses, or internal events by updating the UI when the data changes.

### Why Do We Need State?

We need state in React to:

- Track dynamic data: such as form inputs, API responses, UI toggles (like modals or dropdowns), etc.
- Enable interactivity: like incrementing a counter, switching tabs, or filtering data.
- Trigger re-renders: When state changes, React automatically re-renders the component to reflect the new data in the UI.

---

## 6. What is HTTP and HTTPS protocol?

**HTTP (HyperText Transfer Protocol)** is a protocol used for transferring data between a web browser (client) and a web server.  
It is the foundation of any data exchange on the web and operates over port 80 by default.

- It's stateless – each request is independent.
- It transfers data in plain text, which is not secure.

**What is HTTPS?**

HTTPS (HyperText Transfer Protocol Secure) is the secure version of HTTP.  
It uses SSL/TLS encryption to secure the communication between the browser and the server. It operates over port 443.

- Encrypts data to protect it from hackers.
- Ensures data integrity and authentication (via SSL certificates).
- Used for secure transactions, like banking, logins, and e-commerce.

---

## 7. What is autodeploy.com/admin URL?

The URL `autodeploy.com/admin` likely refers to an internal deployment admin dashboard or portal used by your team or organization to:

- Trigger deployments
- Monitor pipeline statuses
- Manage environments (Dev, QA, Staging, Production)
- Rollback or restart builds
- Review deployment logs and artifacts

This kind of admin interface is commonly seen in custom CI/CD solutions or tools like Jenkins, TeamCity, GitLab CI, or AWS CodePipeline.

---

## 8. How does the data flow into ReactJS?

In React, data flows in one direction — this is called **unidirectional data flow**.

### From Parent to Child (via Props)

Props (short for properties) are used to pass data from parent components to child components.  
Props are read-only in the child component.

```jsx
function Parent() {
  return <Child name="Vijay" />;
}

function Child(props) {
  return <p>Hello, {props.name}</p>;
}
```

## 9. Can you draw the architecture of your application?

**Typical Architecture of United.com:**

User (Customer)
│
▼
[Web Client / Mobile App]
(React/Angular/Next.js frontend)
│
▼
[Content Delivery Network (CDN)]
(e.g., Akamai, Cloudflare)
│
▼
[Web Server / Application Server]
(Load Balanced, Auto-scaled)
│
▼
[API Gateway / Backend Services]
├── Flight Search Service (queries availability, fares)
├── Booking & Reservation Service
├── User Profile & Authentication Service
├── Payment Gateway Integration
├── Loyalty / Mileage Program Service
└── Customer Support & Chatbot Service
│
▼
[Database Layer]
├── Relational DB (Bookings, Users, Flights)
├── NoSQL DB (Sessions, Caching)
└── Analytics DB (User behavior, logs)
│
▼
[Third-Party Integrations]
├── Global Distribution Systems (GDS) like Sabre, Amadeus
├── Payment Processors (Stripe, Visa, Mastercard)
├── Identity Verification Providers
└── External APIs (Weather, Flight Status)

---

## 10. Can you walk me through how your united.com app works?

- User lands on **united.com**, the frontend loads via CDN.
- React SPA (Single Page Application) renders based on route (e.g., /signin, /book).
- API requests are triggered through `axios` or `fetch` to backend microservices via API Gateway.
- Services handle business logic (auth, booking, flight data) and interact with the database.
- Redux-Saga manages async state (API calls, loading spinners, error handling).
- Auth tokens, session info are stored in cookies/localStorage.
- Features like KTN, Miles Pooling, U18 are displayed based on user profile and role.
- Errors are logged in CloudWatch; accessibility is handled as per WCAG.

---

## 11. What is MVC architecture? What is View?

**MVC (Model-View-Controller)** is a design pattern that separates the application logic into three components:

- **Model**: Manages data and business logic (e.g., DB queries, validation).
- **View**: The UI that displays the data (HTML, JSX).
- **Controller**: Handles input, manipulates model, and updates view.

**View** is the presentation layer. In React, your JSX templates and components act as Views.

---

## 12. Is React MVC architecture?

React itself is **not** an MVC framework.  
It mainly provides the **View** part.  
You can combine React with other tools like Redux (Model) and React Router (Controller-like behavior) to follow MVC principles.

---

## 13. Suppose 100 lines of code, how does change happen?

- On a change in **state** or **props**, React triggers a re-render.
- React creates a new **virtual DOM** and compares it to the previous one (diffing).
- Only the changed elements are updated in the actual DOM — this is called **reconciliation**.
- Result: Efficient, minimal DOM updates even with large codebases.

---

## 14. What is DOM?

**DOM (Document Object Model)** is a tree-like structure representing the HTML of a webpage.  
It allows JavaScript to access, modify, or update elements on the page dynamically.

---

## 15. What is parent?

A **parent component** is one that renders another component inside it and may pass data via props.

Example:

````jsx
function Parent() {
  return <Child name="Vijay" />;
}



### 16. What is child?
A child component receives data from the parent via props.

**Example:**
```jsx
function Child(props) {
  return <p>Hello, {props.name}</p>;
}
````

---

### 17. How state works in Redux? Example

Redux uses a centralized store.  
Data flows in this cycle:

- Dispatch an action: `store.dispatch({ type: "INCREMENT" })`
- Reducer updates state based on action type.
- UI gets re-rendered with new state from store.

**Example:**

```js
const initialState = { count: 0 };

function counterReducer(state = initialState, action) {
  switch (action.type) {
    case "INCREMENT":
      return { count: state.count + 1 };
    default:
      return state;
  }
}
```

---

### 18. What kind of state React supports?

- **Local state** (`useState`)
- **Global state** (via Redux or Context API)
- **Server state** (API responses)
- **Form state** (input values)
- **Navigation/URL state** (React Router params)

---

### 19. Username, password — where does the data go?

- Collected via form inputs on the frontend.
- Sent to backend over HTTPS.
- Backend verifies credentials.
- If valid, session token or JWT is returned.
- Token is stored (cookie/localStorage) and used for authentication in future requests.

---

### 20. Have you used Azure, AWS for deployment of the code?

Yes.

**AWS:** S3 (static hosting), CloudFront (CDN), Lambda, API Gateway, CodePipeline (CI/CD), CloudWatch (logs).  
**Azure:** Azure DevOps pipelines, Azure Blob Storage, Azure App Service.

---

### 21. Why did you use redux-saga? Purpose? What side effects did you handle?

**Purpose of redux-saga:**

- Handle asynchronous side effects in Redux using generator functions.
- Better management of API calls, delays, debounce, retries, race conditions.

**Side effects handled:**

- API requests (fetch user data, post booking details).
- Authentication flows.
- Form validation + debouncing.
- Token expiration and refresh handling.

---

### 22. What is parent and child? With example?

```jsx
// Parent Component
function Parent() {
  const greeting = "Welcome!";
  return <Child message={greeting} />;
}

// Child Component
function Child({ message }) {
  return <h1>{message}</h1>;
}
```

- **Parent:** Passes `greeting` to Child.
- **Child:** Receives `message` as prop.

---

### 23. Why is React unidirectional?

React uses one-way data flow:

- Data flows from parent → child via props.
- State is updated using hooks like `useState` or `dispatch`.

**Benefits:**

- Predictable flow.
- Easier to debug.
- Better control of how data changes.

---

### 24. Did you work on backend also?

Yes, I’ve collaborated with backend teams and worked on:

- Writing APIs in Node.js / NestJS.
- Integrating GraphQL queries/mutations.
- Working with MongoDB, PostgreSQL.
- AWS services like Lambda, API Gateway.

---

### 25. Have you used cloud deployments like AWS, Azure?

Yes.

**AWS:** For hosting frontend in S3, backend in Lambda/API Gateway, with CI/CD via CodePipeline.  
**Azure:** App Service, Blob Storage, Azure DevOps for build + release pipelines.

---

### 26. Redux architecture — how did you implement it in your previous company?

- **Actions:** Defined event types (e.g., `FETCH_USER`).
- **Reducers:** Updated state immutably based on actions.
- **Redux-Saga:** Handled API calls and async logic.
- **Store:** Created using `configureStore` or `createStore`.

**Connected to React using:** `Provider`, `useSelector`, `useDispatch`.

**Modular structure:**

```plaintext
/redux
  /user
    - user.actions.js
    - user.reducer.js
    - user.saga.js
    - user.types.js
```

---

### 27. How do you deploy your code? Which application?

**Code Commit:** GitHub or Azure Repos  
**CI/CD Tools:** GitLab CI, Azure DevOps, AWS CodePipeline  
**Build Process:** Webpack or Vite bundles app

**Deploy To:**

- AWS S3 (static files)
- Azure App Service
- Netlify or Vercel for React SPAs

**Deployment includes:**

- Linting
- Unit Tests
- Build
- Upload to environment (Dev, QA, Prod)
- Post-deploy monitoring/logging via CloudWatch or Application Insights
