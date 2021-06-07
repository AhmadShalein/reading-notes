# Read 02: State and Props:

## Component Lifecycle Events:

**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**
Render will happen before the componentDidMount.

**What is the very first thing to happen in the lifecycle of React?**
Mounting is the first phase which begins with the constructor.

**Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates?**
It all happens in this order: **constructor**, **render**, **React Updates**, **componentDidMount**, **componentWillUnmount**.

**What does componentDidMount do?**
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here.

--------------------------------------------------------------------

## State Vs Props:

**What types of things can you pass in the props?**
Any type of data can be passed throught the props.

**What is the big difference between props and state?**
Props passes data from the parent component to it's child, but the child can't alter this data. But on the other hand, state passes data from the parent component to the child, where you can then alter data and manipulate it inside the child only.

**When do we re-render our application?**
When we change the state of that component, the comopnent gets re-rendered.

**What are some examples of things that we could store in state?**
Inside forms, like checkboxes, inputs etc...

---------------------------------------------------------------------

### Things I want to know more about:
- Big deeper into the titles.
- How to use props and states.
