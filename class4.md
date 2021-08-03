# React and Forms

## React Docs - Forms

1. What is a ‘Controlled Component’?
**The React component that renders a form also controls what happens in that form on subsequent user input**
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
**Update the state with their responses as soon as they enter them. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.**
3. How do we target what the user is entering if we have an event handler on an input field?
**When we need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.**

## The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?
**It does the same exact thing of if statment in just one line of code.**
2. Rewrite the following statement using a ternary statement:

   `if(x===y){`
     `console.log(true);`
     `} else {`
     `console.log(false);`
   `}`

    `x===y?console.log(true);console.log(false);`
  
## Things I want to know more about

1. How to implement the form in react.
2. use the Ternary Operator inside code.

### Resources used in this resding note

 1. <https://reactjs.org/docs/forms.html>
 2. <https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff>
 3. <https://react-bootstrap.github.io/components/forms/>
 4. <https://reactjs.org/docs/conditional-rendering.html>

