# Passing Functions as Props

## lists and keys

1. What does .map() return?**return new array its length equal to the mapped array.**
2. If I want to loop through an array and display each value in JSX, how do I do that in React?`array.map((element)=>{console.log(element)})`
3. Each list item needs a unique **key**.
4. What is the purpose of a key?
**help React identify which items have changed, are added, or are removed.**

## The Spread Operator

1. What is the spread operator? ***spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.***
2. List 4 things that the spread operator can do.
1-Copying an array.2-Concatenating or combining arrays. 3-Adding to state in React. 4-Combining objects.
3. Give an example of using the spread operator to combine two arrays.
`let parts = ['shoulders', 'knees'];`
`let lyrics = ['head', ...parts, 'and', 'toes'];`
`//  ["head", "shoulders", "knees", "and", "toes"]`

4. Give an example of using the spread operator to add a new item to an array.
`let numberStore = [0, 1, 2];`
`let newNumber = 12;`
`numberStore = [...numberStore, newNumber];`

5. Give an example of using the spread operator to combine two objects into one.

     `let job = {`
       `jobTitle: 'JavaScript Developer',`
       `country: 'USA'`
     `};`

     `let location = {`
       `city: 'London',`
       `country: 'England'`
      `};`

      `let remoteJob = {`
         `...job,`
         `...location`
      `};`

        the output:

       `{`
         `jobTitle: 'JavaScript Developer',`
         `country: 'England',`
         `city: 'London'`
       `}` 

## Video Part

1. In the video, what is the first step that the developer does to pass functions between components?
**create a function that needed to be passed.**
2. In your own words, what does the increment function do?
**it will incrment the count by one when we call the function.**
3. How can you pass a method from a parent component into a child component?
**by calling its name directly.**
4. How does the child component invoke a method that was passed to it from a parent component?**create a propertiy for the object and assign to it this.theNameOfTheFunction betweebn curly braces.**

## Things I want to know more about

1. The usage of map()with the states.
2. how to pass a function from child to parent.

### Resources used in this reading note

1. <https://reactjs.org/docs/lists-and-keys.html>
2. <https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab>
3. <https://www.youtube.com/watch?v=c05OL7XbwXU>
4. <https://reactjs.org/tutorial/tutorial.html>