# Read 04: React and Forms:

## React Docs - Forms:

**What is a ‘Controlled Component’?**

- We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

- We update the responses as soon as they are entered, because when usingthe controlled component, the component state is the single source of truth.

**How do we target what the user is entering if we have an event handler on an input field?**

- By using event.target.stateName.

--------------------------------------------------------------------

## The Conditional (Ternary) Operator Explained:

**Why would we use a ternary operator?**

- To write conditional statements in one line of code.

**Rewrite the following statement using a ternary statement:**

if(x===y){
console.log(true);
} else {
console.log(false);
}

(x === y) ? >='true':'false';

---------------------------------------------------------------------

### Things I want to know more about:

- Using forms and Controlled Component with React.
