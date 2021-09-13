# Passing Functions as Props

<img src="https://i.ytimg.com/vi/szmS_M-BMls/mqdefault.jpg" alt="react" width="500"/>

**Lists and Keys**

we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

## example
```
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);console.log(doubled);
```
---

## Map Methode :
**`Map`** method is a loop that iterate over an array and modify its elements using a callback function.

Instead of manually iterating over the array using a loop, you can simply use the built-in **`.map()`** method.

**`.map()`** method returns a new array that has the same length of the iterated array and each element being the result of the callback function.
 
 
## Rendering Multiple Components 
You can build collections of elements and include them in JSX using curly braces {}.

```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>  <li>{number}</li>);
```


1.  What does .map() return?

function to take an array of numbers and double their values. We assign the new array returned by map()
   
2.  If I want to loop through an array and display each value in JSX, how do I do that in React?

 we loop through the numbers array using the JavaScript map() function. We return a `<li>` element for each item
   
3.  Each list item needs a unique key.

4. What is the purpose of a key?
Keys help React identify which items have changed, are added, or are removed

## The Spread Operator

   - What is the spread operator?

   In JavaScript, spread syntax refers to the use of an ellipsis of three dots to expand an iterable object into the list of arguments.
   
   - List 4 things that the spread operator can do.

      * Copying an array
      * Concatenating or combining arrays
      * Using Math functions
      * Using an array as arguments
      

 - Give an example of using the spread operator to combine two arrays.


```
const fruits = [' 🍍 ' ,' 🍉  ', '🍏 ']
const moreFruits = [...fruits];
console.log(moreFruits) 
fruits[0] = ' 🍊 '
console.log(...[...fruits,'...',...moreFruits]) 
```

- Give an example of using the spread operator to add a new item to an array.

here is the example:
```
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) 
```


- Give an example of using the spread operator to combine two objects into one.

```
const fewFruit = [' 🍊 ', '🍏 ']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) 
```

---

**Passing Functions Between Components:**

+ In the video, what is the first step that the developer does to pass functions between components?

in this video he created function called increament to to pass in a person object

+ In your own words, what does the increment function do?
it adds one to the value. 
    
+ How can you pass a method from a parent component into a child component?
    we can pass it so in the person object we can put increment name inside it `this.increment` that's a reference to an increment function  

+ How does the child component invoke a method that was passed to it from a parent component?
we call that method like this: `this.props.increament()`