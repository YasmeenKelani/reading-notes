# State and Props

**What are component lifecycle events?**
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

**What is the very first thing to happen in the lifecycle of React ?**
To understand React we should first know it's lifecycle. So the first thing happen in React lifecycle is Mounting, which consists of the code and React’s internals(Constructor), is then inserted into the DOM.
So Constructor is the very first thing happen in React lifecycle.

* In React, components go through a lifecycle of events:
<img src="https://miro.medium.com/max/1838/1*4C2RG1f8GY-84HSyCzyGfQ.png" alt="react" width="500"/>

**Props Vs State :**

- Props:
Think of props as arguments to a function.Typically when you have a piece of code that you would like to reuse, you can place that code into a function and any dynamic values that code used before can be accepted as argument.
Example:

```
const five = add(2, 3)
```
The same is true of a piece of JSX, except instead of calling it like a normal function you use JSX syntax

```
<Add n1={2} n2={3} />
```
So in props we can pass any type of data from parent to the child.

- State:
State is data that changes over time, so precisely what React state is intended to be used for tracking data values over the lifetime of the component.

```
So whenever the state changed we re-render the application.
```
**Source :**
- [Kentcdodds](https://kentcdodds.com/blog/props-vs-state)
- [LogRocket](https://blog.logrocket.com/react-lifecycle-methods-tutorial-examples/)
