## What is React and why is it used?

[Source](https://devinterview.io/questions/web-and-mobile-development/react-interview-questions/)

React is an open-source, front-end Javascript library for building user interfaces, that focuses on reusable components and virtual DOM for performance.

### Core Concepts

#### Virtual DOM

React's Virtual DOM is a lightweight in-memory representation of the actual DOM elements. When changes occur, React compares the current Virtual DOM with a shadow copy and efficiently updates ony the changed portions in the real DOM.

This mechanism significantly reduces expensive direct DOM manipulations, resulting in improved performance and responsiveness in web applications.

#### Components

React Components encapsulate both the visual and the corresponding logic. They can be either classes or pure functions. This modular architecture and the ability to nest and reuse components make React a powerful UI toolkit.

Components are broken down into two main types:

1. **Class Components**: These are ES6 classes that can hold state and offer lifecycle methods.

2. **Functional Components**: Primarily plain Javascript functions: until the advent of "hooks" they couldn't maintain states.

Key changes, starting from React 16.8:

- Introduction of new hooks API expanded state-management to functional components
- Popular hooks include `useState` for state management and `useEffect` for lifecycle management.

Beyond this foundational structure, hooks offer extensive state, lifecyle, and context APIs, making functional components powerful building blocks.

#### Unidirectional Data-flow

React mandates a one-way data flow, empowering developers to understand and manage data propagation more effectively. This simplifies tracking, debugging, and validating data changes across the application.

While sibling components can communicate indirectly through shared parent components, direct communication among sibling components is typically discouraged.

#### JSX: Syntactic Sugar

JSX empowers developers by offering a more intuitive, HTML-like syntax for embedding JavaScript expressions. This marriage of UI and logic not only renders extensive possibilities but also promotes code organization and readablity.

## Why use React?

### Declarative programming Paradigm

React enables a declartive style of programming: developers define the interface's desired state, and React ensures the DOM reflects that state. This approach is more intuitive and helps in designing clear, maintainable code.

### Strong Community Backing and Ecosystem

React has been gaining momentum with an entusiastic commuinity regularly contributing new solutions, updates and robust third-party libraries. The supportive ecosystem extends to comprehensive toolsets for better development and debugging (like React DevTools).

### Reusablitiy and Composablitiy

React's architecture is built on reusable components, fostering modular, consistent UI elements and logic that cna be redeployed across projects or shared with others.

### Performance Optimization

The Virtual DOM serves as a powerful performance amplifier, and features like providing keys to iterated lists ensure efficient and targeted DOM updates. React is also capable of server-side rendering, blostering app speed and SEO-friendliness

### Effectively Data Management

For application-wide state management, React provides Context API and libraries like Redux. Meanwhile, local state management with hooks like `useState` streamlines state handling within components
