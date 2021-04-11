# Read006: Problem Domain, Objects, and the DOM:

## Objects:

They group together a set of variables and functions to create a model of something you would recognize from the real world. In an object, variable become knows as properties, and functions become known as methods.

- You can access a property or method of an object by using the name of the object followed by the property/method tou want to access.

## Document Object Model:
- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes: document nodes,element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or cl ass attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one node, it will always return a Nadel i st.
- From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and child elements that are siblings of each other.
- In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree.
