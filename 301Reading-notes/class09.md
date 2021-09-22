# FUNCTIONAL PROGRAMMING

## What is functional programming ?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

## What is a pure function and how do we know if something is a pure function ?

So how do we know if a function is pure or not? Here is a very strict definition of purity:

* It returns the same result if given the same arguments (it is also referred as deterministic)

* It does not cause any observable side effects

* It returns the same result if given the same arguments.

* What are the benefits of a pure function?

- **Immediatly testable**.
- **Easier maintaining, refactoring, and testing**.
- **No need for mocking anything**.

* What is immutability?

**Immutability** means that it can't be changed (unchangeable)

* What is Referential transparency*? [source](https://en.wikipedia.org/wiki/Referential_transparency)

**Referential transparency** and *referential opacity* are *properties* of *parts* of **computer programs**. An *expression* is called **referentially transparent** if it can be *replaced* with its corresponding value (and vice-versa) without changing the program's behavior. (**pure** *+* **immutability** *=* **referential transparency**)

## Node JS: Modules and require()

1. *What is a module*? 

**Modules** in **Node.js** are a *set of functionalities* that can be *called* whenever are needed.

- *What does the word ‘require’ do*? 

It **imports** the *data* from a **module**, *given* it's **path**.

- *How do we bring another module into the file the we are working in*? 

We can do that by *using* the word **require** and give it the *path* of the **module**.

- *What do we have to do to make a module available*? 

We can fo that by using `module.exports = what ever we want to make available`. Like that we can export the data which we want to make available.
