# 📘 ReactJS Interview Questions & Answers

This repo is my personal collection of ReactJS interview Q&A.  
Each question is answered briefly and clearly to help with interview prep and revision.

### Table of Contents

| No. | Question                                                                           |
| --- | ---------------------------------------------------------------------------------- |
| 1   | [What is React?](#what-is-react)                                                   |
| 2   | [What is Single Page Application (SPA)?](#what-is-single-page-application-spa)     |
| 3   | [What are features of React?](#what-are-features-of-react)                         |
| 4   | [What is DOM (Document Object Model)](#what-is-dom-document-object-model)          |
| 5   | [What is Virtual DOM?](#what-is-virtual-dom)                                       |
| 6   | [What are React Components?](#what-are-react-components)                           |
| 7   | [What is npm?](#what-is-npm)                                                       |
| 8   | [What is role of node_modules folder?](#what-is-role-of-node_modules-folder)       |
| 9   | [What is babel?](#what-is-babel)                                                   |
| 10  | [What is role of public folder in React app?](#what-is-role-of-public-folder-in-react-app)        |
| 11  | [What is role of src folder in React app?](#what-is-role-of-src-folder-in-react-app)              |
| 12  | [What is role of index.html page in React app?](#what-is-role-of-index.html-page-in-react-app)    |
| 13  | [What is role of App.js in React App?](#what-is-role-of-app.js-in-react-app)                      |
| 14  | [How to create Components in React?](#how-to-create-components-in-react)    |
| 15  | [When to use Function & Class Components?](#when-to-use-function--class-component)    |
| 16  | [What is state & props in React?](#what-is-state--props-in-react)                                  |
| 17  | [How is Data sent from Child Component to Parent Component? What is Lifting State Up or Callback Props?](#how-is-data-sent-from-child-component-to-parent-component-what-is-lifting-state-up-or-callback-props)    |
| 18  | [What is Conditional rendering in JSX?](#what-is-conditional-rendering-in-jsx)                     |
| 19  | [What are Controlled & Uncontrolled Components?](#what-are-controlled--uncontrolled-components)    |
| 20  | [What is Conditional rendering in JSX?](#what-is-conditional-rendering-in-jsx)                     |
| 21  | [What is Prop Drilling?](#what-is-prop-drilling)                     |
| 22  | [What is React Composition?](#what-is-react-composition)                     |
| 23  | [What dependencies are essential for creating a React app?](#what-dependencies-are-essential-for-creating-a-react-app)                     |
| 24  | [What is Bundle?](#what-is-bundle)                     |
| 25  | [What is Webpack?](#what-is-webpack)                     |
| 26  | [What are Class Components in React? What are different ways to define them?](#what-are-class-components-in-react-what-are-different-ways-to-define-them)            |
| 27 | [ What is difference between Class & Functional Component?](#what-is-difference-between-class--functional-component) |
| 28 | [What is difference between Inheritance & Composition in React?](#what-is-difference-between-inheritance--composition-in-react) |
| 29 | [What is constructor & super keywords in React?](#what-is-constructor--super-keywords-in-react) |





1. ### What is React?

   React is an _open sorce_ _js library_, developed by facebook(meta). It is used to build _UI interfaces_ & simplifies creation of _SPA(Single Page Applications)_, using _reusable components_ & _dynamic rendering_. It follows _Component based architecture_.

   **[⬆ Back to Top](#table-of-contents)**

2. ### What is Single Page Application (SPA)?

   Single Page Application has only one web page. Whenever data is updated by user, it gets _dynamically rendered_ on page without a _full reload_. <br/> Note: Multiple SPAs are SPAs only. eg. react app only has one single HTML file (index.html), whereas multipage apps have multiple HTML files.  <br/> eg: When a page is switched via Navbar section on an app developed by react, page changes without reloading the page. here, `<Link>` doesnt reloads page while `<a>` does.

   **[⬆ Back to Top](#table-of-contents)**

3. ### What are features of React?

   1.**High Performance**: React uses Virtual Dom which ensures only part of webpage where data changes gets updated instead of entire page, leading to faster & smoother app. <br/> 2. **One way Data Binding**: Data flow in React is unidirectional, it flows from Parent to Child. This makes app predictable & easy to debug. <br/> 3. **JSX (js XML)**: React used js syntax extension which makes code HTML like, thus writing HTML in js, making code more UI friendly & readable. JSX evaluates everything between `{}`<br/> 4. **Component Based Architecture**: React uses reusable, independent components for rendering UI & logic, making code resuable & modular. <br/> 5. **Server Side Rendering Support**: react supports server-side rendering components thus improving performance & SEO optimisation for the web apps. <br/> 6. **Dedicated Developer Tools**: Chrome has specialised Developer Tools which help in simplifying debugging & performance monitoring.

   **[⬆ Back to Top](#table-of-contents)**

4. ### What is DOM (Document Object Model)?
    DOM is a *browser* feature. It is a *tree like* representation of a web page. It *allows js* to dynamically access elements, thus allowing dynamic creation & updation of webpage contents & its structure. <br/> **DOM Updation** converts static webpage into dynamic ones.

5. ### What is Virtual DOM? **

   Virtual DOM is a *core concept of react* & other *modern Js frameworks*. It is *lightweight representation* of real DOM, created *in memory* used by *Browsers* to *render web pages*. <br/> **How it works?** <br/> 1. **Representation** : V-DOM is a *js object* which mirrors structure of *real DOM*, is faster to create & update as it lacks overheads of **Real Browser Rendering**<br/> 2. **Change Detection** : Whenever a *component's state or prop changes* in React, a *new V-DOM* is created to *represent updated UI*.<br/> 3. **Diffing** : React compares the new V-Dom with previous V-DOM to find out what has been changed using *Diffing algorithm or Reconcilliation*. Basically it identifies changes between these two trees. <br/> 4. **Efficient Updates** : Only *changed parts* of web page are updated in real DOM by React instead of re-rendering entire page which is slower & resource intensive. <br/> 5. **Batching** : Updates to real Dom are batched together to improve performance, & reduce recalculation & repaints.<br/> <br/> Note: <br/>1. Overheads of Real Browser Rendering are - frequent DOM Manipulation, Large DOM Size, Complex CSS Selectors, Js DOM access, initial render updates, Layoutthrashing etc.<br/> 2. React's Diffing Algo has Complexity -  O(n) both Time & space where n - no. of elements in tree.

   **[⬆ Back to Top](#table-of-contents)**

6. ### What are React Components?

   React Components are reusable building blocks for creating UI.

7. ### What is npm?

   npm - *node package manager* is standard package manager for NodeJs. It is used to *install, manage & share* **Js packages & dependencies** for NodeJs project. <br/> In react, npm does Project initialisation, Running & Building Apps, Dependencies Management, Script Execution (define & run custom scripts), Efficient Package Installation, Version Control (package.json), & Collaboration & Code Sharing.  

   **[⬆ Back to Top](#table-of-contents)**

8. ###  What is role of node_modules folder?

   node_modules folder is a directory *automatically created* at root of your project when you *install packages* using npm. It is *storage location* of all *external dependencies* required by your project.

9. ### What is babel?

   Babel is a free & open source Js compiler which converts *new, modern Js code (ECMA Script 2015/ES6 & newer)* into *older* compatible versions, so that they can run in older browsers or Js engines. This allows developers to use latest language features without worrying about *browser compatibility*. It can transpile modern Js as well as supports Typescript & JSX too.<br/> In react, since browser cant directly read JSX file, babel transpiles JSX code into Js. <br/> 
   `function App(){` <br/> 
   `return React.createElement(` <br/>
    `'div',` <br/> 
    `{className: 'app'},` <br/> 
    `React.createElement('h1',null,'Hello")` <br/> 
    `)` <br/> 
    `}` <br/> Note: Transpiler converts source code from one programming language to another.

    **[⬆ Back to Top](#table-of-contents)**

10. ### What is role of public folder in React app?

    It contains all *static assets needed by Browser* & not processed by build tools like **Webpack**.  They are directly accessed by URL, & not processed by build system.

11. ### What is role of src folder in React app?

    It is most important folder in development. It contains all source code & logic of application. It defines structure, behaviour, styling of the app. Only files inside /src are processed by build tools like Webpack.

12. ### What is role of index.html page in React App?

    It is entry point of React app. It is the first page to be loaded by browser for SPAs. It contains 'root' id element wherein entire React app will be rendered directly.

13. ### What is role of App.js in React App?

    It is present inside /src in React app, & is root of main app's component tree.

14. ###  How to create Components in React?

      Components are the *building blocks* of *creating User Interfaces(UI)* in React. There are two ways: <br/> <ol> <li> **Function Component**: This is the simplest way to create a component. Those are *pure JavaScript functions* that accept *props object* as the only parameter and *return React elements (in JSX Format)* to *render the output*: <br/> 
      `function Greeting({ message }) {` <br/> `return <h1>{"Hello, ${message}"}</h1>;`<br/> `}` <br/><br/> <li> **Class Component**: ES6 class can be used to define a component. <br/>
       `class Greeting extends React.Component {`<br/>
       `render() {` <br/> 
         `return <h1>{`Hello, ${this.props.message}`}</h1>;`<br/>
         `}`<br/>
       `}`<br/></ol>

       **[⬆ Back to Top](#table-of-contents)**

15. ### When to use Function & Class Components?

      After addition of Hooks (React v.16.8 onwards) it is recommended to use **Function Components** over **Class** ones, as now with Function C, features which were only available in Class C. like state, lifecycle methods are available here too.<br/> So, use Class C. when a React Functionality is needed whose Function C. equivalent is not present yet (like Err Boundaries) or while working in older versions where state or lifecycle methods are needed. <br/> Use Functional C. mostly as they are simple, readable & follow modern code practices like, use of React Hooks for state & side effects.

      **[⬆ Back to Top](#table-of-contents)**

16. ###  What is state & props in React?

      **Props** are inputs to a React component, passed from a parent component to a child component. They are **immutable** within the receiving component. They are used to **pass data and event handlers** down the component tree, thus making it *dynamic and reusable*. <br/> Note: props are objects which can be *Destructured*. To forward all props, use Spread operator `{...props}`  
      
      ```js 
     function Welcome(props) {
      return <h1>Hello, {props.name}!</h1>;
      }
      // Usage: <Welcome name="Alice" />
      ```

      **State** is a *built-in object* in React components, used to *store data or information of component* which can change over time. They are *mutable*, in reponse to user actions, API responses or other events. It is used for data which needs to be *tracked or updated* within a component. <br/>
      
      ```js 
      function Counter() {
     const [count, setCount] = React.useState(0);
      return (
       <div>
         <p>{count}</p>
         <button onClick={() => setCount(count + 1)}>Increment</button>
       </div>);
      } 
      ``` 
      > When state changes, React automatically re-renders the componet (& all its child Components) to reflect the new state.

      **[⬆ Back to Top](#table-of-contents)**

17. ### How is Data sent from Child Component to Parent Component? What is Lifting State Up or Callback Props?

      Standard Approach is: <br/> <ol> <li> The parent component defines a *callback function*. <li>The parent *passes* this function to the child component *via props*. <li>The child component *calls this function*, *passing the data as an argument*. <li>The parent *receives the data* and *can update its state* or perform other actions. </ol> <br/> Note: This pattern is called **lifting state up** or **callback props**. <br/> <br/> **Parent Component** <br/><br/>  ![ParentComponent](./images/ParentCDataTransfer.png) <br/><br/>  **Child Component** <br/><br/>  ![ChildComponent](./images/ChildCDataTransfer.png) <br/> Note: This maintains unidirectional flow of data.

      **[⬆ Back to Top](#table-of-contents)**

18. ### What is Conditional rendering in JSX?

    It is similiar to syntax in Js but with some changes: <ol><li>**If Statement**: <br/> ![if](./images/IfStatement.png) <li>**Ternary Operator**: <br/> ![if](./images/TernaryOperator.png) <li>**Logical && Operator**: First part of statement has to be true to render second part.<br/> ![if](./images/Logical&&Operator.png)  <li>**Switch Statement**: <br/> ![if](./images/SwitchStatement.png) <li>**Element Variables**: <br/> ![if](./images/ElementVariable.png)</ol>  

19. ### What are Controlled & Uncontrolled Components?

      In React, the main difference lies in how the values of components are managed.<br/> <ol><li>**Controlled Components**: These are React Components where *value* is managed by *state*. React state is *single source of truth* for input's value. e.g.: input in form element.<br/> Here, component recieves *value* & an *Event Handler* as *prop*, which gets trigerred by user action,which may update state & UI will reflect latest state.<br/>React has full control over data, components are predicatable, easy to validate, & it enables real time data sharing between components. <br/> It can cause more re-renders, especially with many inputs or frequent updates. <br/>  <br/> ![ControlledComponent](./images/ControlledC.png) <br/> <br/>                       <li> **Uncontrolled Components**: These are React Components where React does not directly control the input's value. These manage its own state internally, with the DOM maintaining the current value. <br/> Here, the input's value is not tied to React state, but can be accessed directly from the DOM, typically using a *ref*. It uses *defaultValue* to set the *initial value of an input field* when the component is *first rendered*. Any further changes are tracked by **DOM** & not by **React**.<br/>   <br/> ![UnControlledComponent](./images/UncontrolledC.png)   </ol> <br/> Note: This needs fewer re-renders for high frequency inputs. But, it is harder to validate & synchronize with other components. It is also less predictable & state can be changed outside React's knowledge.

      **[⬆ Back to Top](#table-of-contents)**

20. ### What is State, Stateful, Stateless terms?

      **StateFul Component**: It manages its own state. This means it *holds data* that can *change over time* and *affect the component’s output*. When the *state changes (using setState in class components* or *hooks like useState in functional components)*, the *component re-renders* to reflect the new state.

      **Stateless Component**: It is called a "presentational" component, *does not manage its own state*. It *receives all necessary data via props* and renders output based solely on those props. Stateless components are *easier to test and reuse*, as they do not have internal state dependencies.

      some types of States are:
      1. Local State: Managed within a single component using useState or this.setState.
      2. Shared/Global State: Shared between multiple components, managed via Context API or state management libraries like Redux, MobX, or Recoil.
      3. UI State: Controls UI-specific data (e.g., modal visibility, input values). 
      4. Fetch State: Manages data from asynchronous operations like API calls.<br/> <br/>

      > States are modified using updater functions. If new value is relevant to prev Value, It must be modified using prevState to yield up to date values as state updates are usually batched & asynchronous.
      ```js
      setState(prevState => ({
       ...prevState,
      userName: newValue
      }));
      setCount(prev=> prev+1);
      ```

      **[⬆ Back to Top](#table-of-contents)**

21. ### What is Prop Drilling?

      Prop drilling in React is the process of *passing data (props)* from a parent component down through multiple layers of nested components *until it reaches* the component that actually needs it. It means intermediary components *receive and forward props* even if they don't use them themselves.
      It is an issue because it leads to *Code Duplication*, Difficulty in tracking components, props & decreased Maintainability.
      It can be avoided using Global/Shared States.

      **[⬆ Back to Top](#table-of-contents)**

22. ### What is React Composition?

      It is a core concept that involves building complex user interfaces by combining smaller, reusable components together.<br/>
      This pattern promotes code reusability, maintainability, and scalability, as each component is responsible for a specific piece of functionality.<br/> 
      **Composition is favored over inheritance** in React for *code reuse and flexibility*.<br/>
      How is it done?
      1. Children prop: Components can recieve other Components as their Children. It is used when Parent doesnt know what will render inside.
         ```js
         const Card = ({ children }) => <div className="card">{children}</div>;

         // Usage
         <Card>
            <h2>Title</h2>
            <p>Description</p>
         </Card>
         ```
      2. Passing Components as Props: You can pass entire components as props to other components, enabling dynamic rendering and customization.
      3. Compound Components: A pattern where a parent component manages state and shares it with nested child components, via Global States.
      4. Higher-Order Components (HOCs) and Render Props: Advanced composition techniques for sharing logic between components without repeating code.

      **[⬆ Back to Top](#table-of-contents)**

23. ### What dependencies are essential for creating a React app?

      1. Node.js & npm/yarn: Node.js is the JavaScript runtime needed to run development tools, while npm or yarn are package managers for installing dependencies.
      2. React & ReactDOM: The core libraries for building user interfaces (react) and rendering them to the DOM (react-dom).
      3. Babel: A JavaScript compiler that transforms modern JavaScript (including JSX) into browser-compatible code.
      4. Webpack: A module bundler that compiles JavaScript, CSS, images, and other assets into optimized bundles for the browser (explained in detail below).
      5. Create React App (CRA): A popular tool that sets up a React project with sensible defaults, including Webpack and Babel configurations. Other ways are using Vite.
      6. Development Tools: Tools like ESLint (for code linting), React Developer Tools (for debugging), and testing libraries (e.g., Jest, React Testing Library).

      **[⬆ Back to Top](#table-of-contents)**

24. ### What is Bundle?

      A bundle is the output file (or files) **generated by Webpack** or similar bundlers. It contains all the code and assets your application needs, **combined and optimized** for the browser. <br/>
      Role: The bundle ensures that the browser can **load your React app quickly and efficiently**, with all dependencies resolved.

      **[⬆ Back to Top](#table-of-contents)**

25. ### What is Webpack?

      Webpack is a powerful traditional **module bundler** for JavaScript applications. Its primary role is to:
      1. **Bundle all your JavaScript files and dependencies** (including CSS, images, fonts, etc.) into one or more optimized files for the browser.
      2. **Transform code** using **loaders** (e.g., converting JSX to JS with Babel).
      3. **Optimize assets for production**, such as minifying code and splitting bundles for faster loading.<br/><br/>
      Webpack **automates** the process of managing dependencies and assets, ensuring your React app runs efficiently in development and production environments.<br/>
      **During Developemnt**, Webpack uses features like **Hot Module Replacement (HMR)**, allowing you to see changes instantly without a full page reload.<br/>
      **For Production**, It produces optimised bundles, reduce load times, improve performance By minifing code, removing unused code (tree shaking), splitting code( for faster initial loads).<br/><br/>
      It is **not available in Vite**. Vite has **Rollup** instead for production buildup & very fast HMR using **native ES modules** for Development phase.

      **[⬆ Back to Top](#table-of-contents)**

26. ### What are Class Components in React? What are different ways to define them?

      **Class components** are one of the main ways to define components in React (the other being function components). Before React v16.8 and the *introduction of Hooks*, class components were the primary way to *manage state* and use *lifecycle methods* in React apps.

      A class component
      1. Is a **JavaScript class*** that *extends React.Component* (or Component if imported directly).
      2. Must include a *render() method*, which **returns the JSX** to display.
      3. Can **manage its own state** and *respond to lifecycle events* like *mounting, updating, and unmounting*.
      >React.Component is a parent class featured by React lib & class ("Car") inherits its features. 

      **Defining Class Component:**

      ```js
      //ES6 Class Syntax
      class Car extends React.Component {
            render() {
              return <h2>Hi, I am a Car!</h2>;
            }
      }
      //Usage: <Car/>

      //Directly importing Component
      import { Component } from 'react';
      class Greeting extends Component {
         render() {
            return <h1>Hello, {this.props.name}!</h1>;
         }
      }

      // With a Constructor (for State or Binding)
      // if state or bind methods are to be used
      class Car extends React.Component {
         constructor(props) {
            super(props);
            this.state = { color: "red" };
         }
      render() {
         return <h2>I am a {this.state.color} Car!</h2>;
            }
      }

      // With Static Properties: features like context
      class Button extends React.Component {
         static contextType = ThemeContext;
            render() {
            const theme = this.context;
            return <button className={'button-' + theme}>{this.props.children}</button>;
            }
      }
      ```
      >`static` means `contextType` is a property that `belongs to the class itself`, not to instances of the class.

      **[⬆ Back to Top](#table-of-contents)**

27. #### What is difference between Class & Functional Component?

      | Aspect                | Class Component                                           | Functional Component                                         |
      |-----------------------|----------------------------------------------------------|--------------------------------------------------------------|
      | **Definition**        | Uses ES6 class syntax, extends `React.Component`         | Plain JavaScript function that returns JSX                   |
      | **Syntax**            | More verbose, requires `render()` method                 | Simpler, less boilerplate                                    |
      | **State Management**  | Uses `this.state` and `this.setState`                    | Uses React Hooks (e.g., `useState`) for state                |
      | **Lifecycle Methods** | Has built-in lifecycle methods (e.g., `componentDidMount`) | Uses `useEffect` hook to handle lifecycle events             |
      | **`this` Keyword**    | Must use `this` to access props, state, methods          | No need for `this`                                           |
      | **Performance**       | Slightly less efficient due to more overhead             | Generally more efficient and lightweight                     |
      | **Best Use Case**     | Legacy codebases, Error Boundaries, complex lifecycle    | Modern React apps, most use cases                            |
      | **Composition**       | Supports inheritance                                     | Encourages composition (preferred in modern React)           |


28. ### What is difference between Inheritance & Composition in React?

      **Composition** and **inheritance** are two *approaches* for **structuring and reusing code**, but React strongly favors composition for building user interfaces.

      **Composition** is the practice of building complex UIs by combining smaller, reusable components. Components are nested, and data or behavior is shared via props and children.  

      **Inheritance**: It is when one class component extends another, *inheriting its properties and methods*—an approach borrowed from object-oriented programming. It creates a base component & extend it for specialized components.
      ```js
      class Button extends React.Component { /* ... */ }
      class SubmitButton extends Button { /* ... */ }
      ```
      It leads to **tightly coupled, hard-to-maintain code** which is **less flexible** for UI composition and code reuse.
      Better Alternatives are **composition, HOCs, render props**.

29. ### What is constructor & super keywords in React?

      **constructor**: It is a special *method in JavaScript classes* that is called when a new instance of the class is created. It is used to *initialize the object’s properties*. 
      ```js
      class Car {
            constructor(brand) {
            this.brand = brand;
            }
      }
      ```

      **super**: It is used in a *subclass (a class that extends another class)* to call the constructor of its parent class. 
      `super()` is to be called in the **constructor of a derived class** before using `this`.<br/>This ensures the **parent’s properties and methods** are initialized before the child adds its own.<br/> 
      `super` can also be used to call methods from the parent class inside child class methods.
      ```js
      class Vehicle {
      constructor(type) {
            this.type = type;
      }
      }

      class Car extends Vehicle {
      constructor(type, brand) {
            super(type); // Calls the parent (Vehicle) constructor
            this.brand = brand;
        }
      }
      ```     

30. ### What is role of this keyword in React? **

      In React, the `this` keyword is used to refer to the *current instance* of a **component class**. It allows you to *access the component's props, state, event handlers and methods* within its class definition. <br/> e.g. using `this.state`(to get or set C.'s state),<br/> `this.props`(accessing properties passed from parent C.), <br/> `this.handleClick`(passing as *callback functions*) or <br/> `this.methodName()`(call other methods in same class) inside Class Component.<br/>
      > C - Component

      While passing class methods as **event handlers**  (e.g., onClick={this.handleClick}), it must be ensured that `this` refers to the **correct component instance**. Otherwise, this may be *undefined* or refer to the *global object*, leading to errors (Losing `this` Context).
      1. It can be fixed by **binding the method** in constructor

            ```js
            constructor(props) {
            super(props);
            this.handleClick = this.handleClick.bind(this);
            }
            ```
      2. Also. **Arrow functions** automatically bind this to the class instance.

            ```js
            class Counter extends Component {
            constructor(props) {
                  super(props);
                  this.state = { count: 0 };
            }

            // Arrow function ensures 'this' refers to the component instance
            increment = () => {
              this.setState({ count: this.state.count + 1 });
            };

            render() {
              return (
                  <div>
                     <p>Count: {this.state.count}</p>
                     <button onClick={this.increment}>Increment</button>
                  </div>
                  );
                }
            }
            ```

      In **Functional Components**:
      1. In React functional components, `this` is not used. State and props are accessed directly via **hooks** and **function parameters**, not through this.<br/>

      2. If you use `this` in a functional component, it refers to the **global object (or is undefined in strict mode)**, not the component instance.
       > An instance is a specific, live version of your class component, created and managed by React, with its own state and behavior. **Arrow functions** help make sure that when you use this inside your component methods, it always refers to the correct instance.

31. ### What are Component Life Cycle Methods in React?

      React components have a **"lifecycle"** (a series of stages from creation to removal) that you can tap into using special methods called **lifecycle methods**. These are most relevant for **Class-based Components**, as **functional components use hooks** for similar behavior. <br/> React mostly has 3 methods:
      1. **Mounting**: Component is **created** and **inserted** into the DOM.
      2. **Updating**: Component is **re-rendered** due to changes in props or state.
      3. **Unmounting**: Component is removed from the DOM.

      1. **Mounting Methods**: These methods are called when a component is being inserted into the DOM:

            1. **constructor(props)**: Initializes state and binds methods. Not strictly required unless you need to set up state or bindings.

            2. static **getDerivedStateFromProps(props, state)**: Rarely used, allows state updates based on props before rendering.

            3. **render()**: The only required method; returns the JSX to render.

            4. **componentDidMount()**: Runs after the component is mounted. Used for side effects like data fetching or subscriptions.<br/>

            > The initial render in React occurs during the Mounting phase of the component lifecycle.
            When a component is first created and inserted into the DOM, React triggers the **initial render** by calling the component’s **render() method**, which determines what should appear on the screen. 
            This process happens after any initialization (like setting up state in the constructor) and before the component is fully mounted and componentDidMount() is called. So, sequence is Initialization (e.g., constructor runs), Mounting (initial render occurs here, using render()) ,componentDidMount (runs after the initial render and DOM insertion)

      2. **Updating Methods**: Called whenever the component is re-rendered due to state or prop changes:

            1. static getDerivedStateFromProps(props, state): Also called during updates.

            2. shouldComponentUpdate(nextProps, nextState): Lets you optimize performance by preventing unnecessary renders.

            3. render(): Called again to update the UI.

            4. getSnapshotBeforeUpdate(prevProps, prevState): Lets you capture information (like scroll position) before the DOM is updated.

            5. componentDidUpdate(prevProps, prevState, snapshot): Runs after updates are flushed to the DOM, good for side effects that depend on the DOM.

      3. **Unmounting Method**: Called just before the component is removed from the DOM:

            componentWillUnmount(): Used for cleanup, such as cancelling timers or unsubscribing from services.







