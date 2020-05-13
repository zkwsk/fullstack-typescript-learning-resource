# Fullstack Typescript and React learning resources

This is a curated list of resources for building a web application in Typescript, React and GraphQL. The aim is to gather good resources for learning how to build a web application using Typescript and React. Here is an outline of the technologies we will cover:

- Typescript
  - ES6+ "Modern" Javascript features
    - Arrow functions
    - Array Iterator functions (map, find, first, reduce)
    - Template literals
  - Webpack
  - Compiling Typescript
  - Creating types
  - Creating classes
- React
  - JSX
  - Components
  - Props
  - State
  - Component API
  - Hooks
    - useState
    - useEffect
  - Redux
  - Immer
  - Storybook
  - Blueprint.js
- Node.JS
  - Eventsourcing
  - TypeORM
- GraphQL/Apollo
- Static analysis
  - ESlint
  - Prettier

## Typescript

Typescript is a superset of Javascript. Since browsers does not run Typescript it must be compiled into Javascript. The main benefit of Typescript is to add strict typing and a Class inheritance model that is more familiar to users of object-oriented languages to Javascript. It still retains all of the features, including features related to functional programming, from Javascript and all of the "modern javascript" features discussed below work in Typescript as well.

Resources:
- [TypeScript Deep Dive](https://basarat.gitbooks.io/typescript/content/docs/getting-started.html): Very comprehensive walkthrough which is probably mostly aimed at a experienced Javascript developer moving onto TypeScript and wanting to understand the language in detail.
- [Devhints, TypeScript cheatsheet](https://devhints.io/typescript): TypeScript cheatsheet that is mostly aimed to be a help when taking a more experimental approach to learning.

### Classic javascript

Before learning Typescript it is very helpful to have a good grasp of "classic javascript" (i.e. ES5 and before) in order to understand how Javascript stands out from most other programming languages. The best in-depth resource is probably Douglas Crockfords book: Javascript: The Good Parts. It is not an absolute must to read the entire book in the context of learning modern javascript and typescript, but it provides good context to understand some of the deeper topics of learning modern javascript and there are a lot of blog posts summarizing this book and referring back to it, so it is worth knowing about.

Resources:
- [Javascript: The Good Parts](https://www.amazon.com/JavaScript-Good-Parts-Douglas-Crockford/dp/0596517742)

### Modern Javascript features (ES6+)

One major pain of Javascript is that it has to be implemented in a wide range of browser in a uniform way. Historically that has caused a notoriously slow release cycle. ES5 was released in 2009, ten years after the release of its previous version and it took another 6 years to come out with another update, ES6. From ES6 onwards, it was decided to release new features yearly, despite some browsers still trying to catch up with the modern features and as a result most developers rely on compiling modern versions of Javascript into ES5 which has the most widespread support. When we are talk about using ES6 in "daily speech", we usually mean ES6+ and are distinguishing between a project that is adding some "modern javascript features" via compiling and one that is executed natively in the browser.

Currently, the latest version is ES10. When you set up a a project to compiler your Javascript you get to choose which versions you want to add support for, but generally compiling takes away the need to worry about cross-browser/legacy compatibility.

Since most frameworks (including React) rely on many of these "modern features" it is critical to be familiar with.

The most important "modern features" to be familiar with when using a framework like React are:

- "Fat arrow" functions, including the fact that they automatically bind `this`
- Array Iterators: 
  - `Array.forEach()`
  - `Array.map()`
  - `Array.find()`
  - `Array.filter()`
  - `Array.findIndex()`
  - `Array.reduce()`
  - `Array.every()`
  - `Array.some()`
- Template literals
- Destructuring assignment (arrays as well as objects)

Resources:
- [ES6 Javascript: The Complete Developer's Guide](https://www.udemy.com/course/javascript-es6-tutorial): An excellent Udemy Course.
- [MDN web docs: Arrow function expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions): Arrow functions - pay special attention to the section about "No binding of arguments"
- [MDN web docs: Javascript Arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array): Start on this page and read the pages linked under "Instance methods", specifically the Array Iterators mentioned above.
- [MDN web docs: Template literals/Template strings](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals): Mozilla docs on template literals
- [MDN web docs: Destructuring assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment): Mozilla docs on Destructuring
