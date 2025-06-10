# 📘 ReactJS Interview Questions & Answers

This repo is my personal collection of ReactJS interview Q&A.  
Each question is answered briefly and clearly to help with interview prep and revision.

---

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
| 10  | [What is role of public folder in React app?](#what-is-role-of-public-folder-in-react-app)    |
| 11  | [What is role of src folder in React app?](#what-is-role-of-src-folder-in-react-app)    |
| 12  | [What is role of index.html page in React app?](#what-is-role-of-index.html-page-in-react-app)    |
| 13  | [What is role of App.js in React App?](#what-is-role-of-app.js-in-react-app)    |
| 14  | [How to create Components in React?](#how-to-create-components-in-react)    |
| 15  | [When to use Function & Class Components?](#when-to-use-function--class-component)    |
| 15  | [How to create Components in React](#how-to-create-components-in-react)    |
| 15  | [How to create Components in React](#how-to-create-components-in-react)    |
| 15  | [How to create Components in React](#how-to-create-components-in-react)    |




1. ### What is React?

   React is an _open sorce_ _js library_, developed by facebook(meta). It is used to build _UI interfaces_ & simplifies creation of _SPA(Single Page Applications)_, using _reusable components_ & _dynamic rendering_. It follows _Component based architecture_.

2. ### What is Single Page Application (SPA)?

   Single Page Application has only one web page. Whenever data is updated by user, it gets _dynamically rendered_ on page without a _full reload_. <br/> Note: Multiple SPAs are SPAs only. eg. react app only has one single HTML file (index.html), whereas multipage apps have multiple HTML files.  <br/> eg: When a page is switched via Navbar section on an app developed by react, page changes without reloading the page. here, `<Link>` doesnt reloads page while `<a>` does.

3. ### What are features of React?

   1.**High Performance**: React uses Virtual Dom which ensures only part of webpage where data changes gets updated instead of entire page, leading to faster & smoother app. <br/> 2. **One way Data Binding**: Data flow in React is unidirectional, it flows from Parent to Child. This makes app predictable & easy to debug. <br/> 3. **JSX (js XML)**: React used js syntax extension which makes code HTML like, thus writing HTML in js, making code more UI friendly & readable. JSX evaluates everything between `{}`<br/> 4. **Component Based Architecture**: React uses reusable, independent components for rendering UI & logic, making code resuable & modular. <br/> 5. **Server Side Rendering Support**: react supports server-side rendering components thus improving performance & SEO optimisation for the web apps. <br/> 6. **Dedicated Developer Tools**: Chrome has specialised Developer Tools which help in simplifying debugging & performance monitoring.


4. ### What is DOM (Document Object Model)?
    DOM is a *browser* feature. It is a *tree like* representation of a web page. It *allows js* to dynamically access elements, thus allowing dynamic creation & updation of webpage contents & its structure. <br/> **DOM Updation** converts static webpage into dynamic ones.

5. ### What is Virtual DOM? **

   Virtual DOM is a *core concept of react* & other *modern Js frameworks*. It is *lightweight representation* of real DOM, created *in memory* used by *Browsers* to *render web pages*. <br/> **How it works?** <br/> 1. **Representation** : V-DOM is a *js object* which mirrors structure of *real DOM*, is faster to create & update as it lacks overheads of **Real Browser Rendering**<br/> 2. **Change Detection** : Whenever a *component's state or prop changes* in React, a *new V-DOM* is created to *represent updated UI*.<br/> 3. **Diffing** : React compares the new V-Dom with previous V-DOM to find out what has been changed using *Diffing algorithm or Reconcilliation*. Basically it identifies changes between these two trees. <br/> 4. **Efficient Updates** : Only *changed parts* of web page are updated in real DOM by React instead of re-rendering entire page which is slower & resource intensive. <br/> 5. **Batching** : Updates to real Dom are batched together to improve performance, & reduce recalculation & repaints.<br/> <br/> Note: <br/>1. Overheads of Real Browser Rendering are - frequent DOM Manipulation, Large DOM Size, Complex CSS Selectors, Js DOM access, initial render updates, Layoutthrashing etc.<br/> 2. React's Diffing Algo has Complexity -  O(n) both Time & space where n - no. of elements in tree.

6. ### What are React Components?

   React Components are reusable building blocks for creating UI.

7. ### What is npm?

   npm - *node package manager* is standard package manager for NodeJs. It is used to *install, manage & share* **Js packages & dependencies** for NodeJs project. <br/> In react, npm does Project initialisation, Running & Building Apps, Dependencies Management, Script Execution (define & run custom scripts), Efficient Package Installation, Version Control (package.json), & Collaboration & Code Sharing.  

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

10. ### What is role of public folder in React app?

    It contains all *static assets needed by Browser* & not processed by build tools like **Webpack**.  They are directly accessed by URL, & not processed by build system.

11. ### What is role of src folder in React app?

    It is most important folder in development. It contains all source code & logic of application. It defines structure, behaviour, styling of the app. Only files inside /src are processed by build tools like Webpack.

12. ### What is role of index.html page in React App?

    It is entry point of React app. It is the first page to be loaded by browser for SPAs. It contains 'root' id element wherein entire React app will be rendered directly.

13. ### What is role of App.js in React App?

    It is present inside /src in React app, & is root of main app's component tree.

14. ###  How to create Components in React?

      Components are the *building blocks* of *creating User Interfaces(UI)* in React. There are two ways: <br/> <ol> <li> **Function Component**: This is the simplest way to create a component. Those are *pure JavaScript functions* that accept *props object* as the only parameter and *return React elements (in JSX Format)* to *render the output*: <br/> `function Greeting({ message }) {` <br/> `return <h1>{`Hello, ${message}`}</h1>;`<br/> `}` <br/><br/> <li> **Class Component**: ES6 class can be used to define a component. <br/>
       `class Greeting extends React.Component {`<br/>
       `render() {` <br/> 
         `return <h1>{`Hello, ${this.props.message}`}</h1>;`<br/>
         `}`<br/>
       `}`<br/></ol>

15. ### When to use Function & Class Components?

      After addition of Hooks (React v.16.8 onwards) it is recommended to use **Function Components** over **Class** ones, as now with Function C, features which were only available in Class C. like state, lifecycle methods are available here too.<br/> So, use Class C. when a React Functionality is needed whose Function C. equivalent is not present yet (like Err Boundaries) or while working in older versions where state or lifecycle methods are needed. <br/> Use Functional C. mostly as they are simple, readable & follow modern code practices like, use of React Hooks for state & side effects.

16. ###  What is state & props in React?

      **Props** are inputs to a React component, passed from a parent component to a child component. They are **immutable** within the receiving component. They are used to **pass data and event handlers** down the component tree, thus making it *dynamic and reusable*. <br/> Note: props are objects which can be *Destructured*. To forward all props, use Spread operator `{...props}` <br/><br/> `function Welcome(props) {` <br/>
      `return <h1>Hello, {props.name}!</h1>;` <br/>
      `}` <br/>
      `// Usage: <Welcome name="Alice" />` <br/>  <br/>    **State** is a *built-in object* in React components, used to *store data or information of component* which can change over time. They are *mutable*, in reponse to user actions, API responses or other events. It is used for data which needs to be *tracked or updated* within a component. <br/> <br/>`function Counter() {`<br/>
     `const [count, setCount] = React.useState(0);`<br/>
      `return (`<br/>
       `<div>`<br/>
         `<p>{count}</p>`<br/>
         `<button onClick={() => setCount(count + 1)}>Increment</button>`
       `</div>`<br/>
     `);`<br/>
      `}`<br/><br/> Note: when state changes, React automatically re-renders the componet (& all its child Components) to reflect the new state.

17. ### How is Data sent from Child Component to Parent Component? WHat is Lifting State Up or Callback Props?

      Standard Approach is: <br/> <ol> <li> The parent component defines a *callback function*. <li>The parent *passes* this function to the child component *via props*. <li>The child component *calls this function*, *passing the data as an argument*. <li>The parent *receives the data* and *can update its state* or perform other actions. </ol>





