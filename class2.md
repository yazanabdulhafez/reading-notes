# State and Props

## React lifecycle

![reactlifecycle](https://miro.medium.com/max/1000/0*0saPKFiTUk6W3FYp)

* Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? 
`render happens first`

* What is the very first thing to happen in the lifecycle of React?
 `Mounting`

* Put the following things in the order that they happen:

1. `constructor`
2. `render`
3. `componentDidMount`  
4. `React Updates`
5. `componentWillUnmount`

* What does componentDidMount do?

`This method is useful for performing network requests after a change has occurred.`

## States and Props

* What types of things can you pass in the props?
`All the data types in javascript`

* What is the big difference between props and state?

1. `Components receive data from outside with props, whereas they can create and manage their own data with state`
2. `Props are used to pass data, whereas state is for managing data`
3. `Data from props is read-only, and cannot be modified by a component that is receiving it from outside`
4. `State data can be modified by its own component, but is private (cannot be accessed from outside)`
5. `Props can only be passed from parent component to child (unidirectional flow)`
6. `Modifying state should happen with the setState ( ) method`

* When do we re-render our application?
`React components automatically re-render whenever there is a change in their state or props.`

* What are some examples of things that we could store in state?
`counters, stop watches,values`

## Things I want to know more about

1. how to use state and props inside the code.

### Resources used in this reading note

1. <https://medium.com/edonec/state-in-react-an-overview-a182675cee2c>
2. <https://www.freecodecamp.org/news/where-do-i-belong-a-guide-to-saving-react-component-data-in-state-store-static-and-this-c49b335e2a00/>
3. <https://www.freecodecamp.org/news/react-js-for-beginners-props-state-explained/>
