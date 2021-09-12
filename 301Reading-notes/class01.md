# Introduction to React and Components

**What is React ?**
React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

<img src="https://camo.githubusercontent.com/93d1a921726b3482f425a01005a9d9bd326c3da1e0f1ead8cce623c609d704bd/68747470733a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f7468756d622f612f61372f52656163742d69636f6e2e7376672f3132303070782d52656163742d69636f6e2e7376672e706e67" alt="react" width="500"/>

**What is a Component ?**
UI in React broken down into multiple individual pieces called Components and work on them independently and merge them all in a parent component which will be your final UI.

<img src="https://github.com/Mohammad-Abdul-Ghafour/reading-notes/blob/main/301/IMG/ReactJS-Features-For-Web-and-Mobile.jpg.png?raw=true" alt="react" width="500"/>

**Advantages:**

1. Ease of deployment.
2. Reduced cost.
3. Reusable.
4. Modification of technical complexity.
5. Reliability.
6. System maintenance and evolution.
7. Independent.

**What is props short for ?**
Props is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

* How are props used in React?

- Firstly, define an attribute and its value(data).
- Then pass it to child component(s) by using Props.
- Finally, render the Props Data.

```
import React, { Component } from 'react'; 
import MyComponent from './MyComponent.jsx'; 
class App extends Component { 
   render() { 
       return ( 
           <div> 
               <MyComponent name = "Michael" /> 
               <MyComponent name = "Professor" /> 
           </div> 
       ); 
   } 
} 
export default App;  
```
**What is the flow of props?**
from the parent until the last child so it will be parent ==> 1st-cild ==> 2nd-child ==> 3rd-child==>……==> Nth-child.