# State and Props

## Component Lifecycle Events:

1. **Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**
Render will happen before the componentDidMount.

2. **What is the very first thing to happen in the lifecycle of React?**
Mounting is the first phase which begins with the constructor.

3. **Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates**
It all happens in this order: constructor, render, React Updates, componentDidMount, componentWillUnmount.

4. **What does componentDidMount do?**
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here.

--------------------------------------------------------------------

## State Vs Props:

1. We can pass any type of data in props eg.(representing function, titles, .. etc), props don't change (data in props stay the same, if we want to make a change it's going to be outside the component).
2. Props you pass into a component and is handled outside the component, and state is handled inside a component.
3. When we change the state ,the section will be re-rendered.
4. In state we store what we want to be updated and re-rendered based on what the user is doing, ex.form of checkbox.
