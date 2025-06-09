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


1. ### What is React?

   React is an _open sorce_ _js library_, developed by facebook(meta). It is used to build _UI interfaces_ & simplifies creation of _SPA(Single Page Applications)_, using _reusable components_ & _dynamic rendering_. It follows _Component based architecture_.

2. ### What is Single Page Application (SPA)?

   Single Page Application has only one web page. Whenever data is updated by user, it gets _dynamically rendered_ on page without a _full reload_. <br/> Note: Multiple SPAs are SPAs only. eg. react app only has one single HTML file (index.html), whereas multipage apps have multiple HTML files.  <br/> eg: When a page is switched via Navbar section on an app developed by react, page changes without reloading the page. here, `<Link>` doesnt reloads page while `<a>` does.

3. ### What are features of React?

   1.**High Performance**: React uses Virtual Dom which ensures only part of webpage where data changes gets updated instead of entire page, leading to faster & smoother app. <br/> 2. **One way Data Binding**: Data flow in React is unidirectional, it flows from Parent to Child. This makes app predictable & easy to debug. <br/> 3. **JSX (js XML)**: React used js syntax extension which makes code HTML like, thus writing HTML in js, making code more UI friendly & readable. <br/> 4. **Component Based Architecture**: React uses reusable, independent components for rendering UI & logic, making code resuable & modular. <br/> 5. **Server Side Rendering Support**: react supports server-side rendering components thus improving performance & SEO optimisation for the web apps. <br/> 6. **Dedicated Developer Tools**: Chrome has specialised Developer Tools which help in simplifying debugging & performance monitoring.


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

   Babel is a free & open source Js compiler which converts *new, modern Js code (ECMA Script 2015/ES6 & newer)* into *older* compatible versions, so that they can run in older browsers or Js engines. This allows developers to use latest language features without worrying about *browser compatibility*. It can transpile modern Js as well as supports Typescript & JSX too.

10. ### What is role of public folder in React app?

   It contains all *static assets needed by Browser* & not processed by build tools like **Webpack**.  They are directly accessed by URL, & not processed by build system.

11. ###  What is role of src folder in React app?

   It is most important folder in development. It contains all source code & logic of application. It defines structure, behaviour, styling of the app. Only files inside /src are processed by build tools like Webpack.

12. ### What is role of index.html page in React App?

   It is entry point of React app. It is the first page to be loaded by browser.

