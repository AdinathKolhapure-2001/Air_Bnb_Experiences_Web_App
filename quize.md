Quize 1:

1. What do props helps us accomplish?
--> Make a component more reusable.

2. How do you pass a prop into a component?
--> <MyAwesomeHeader title="???" />



3. Can I pass a custom prop (e.g. `blahblahblah={true}`) to a native
DOM element? (e.g. <div blahblahblah={true}>) Why or Why not?
--> No, because the JSX we use to describe native DOM elements will
    be turned into REAL DOM elements by React. And real DOM elements 
    only have the properties/attributes specified in the HTML specification.
    (Which doesn't include properties like `blahblahblah`)


4. How do I receive props in a component?
function Navbar() {
    return (
        <header>
            ...
        </header>
    )
}
--> By passing the props in the function `Navbar(props)`


5. What data type is `props` when the component receives it?
--> An object



Quize 2:

1. What does the `.map()` array method do?
--> Returns a new array. Whatever gets returned from the callback
    function provided is the placed at the same index in the new array.
    Usually we take the items from the original array and modify them 
    in some way.

2. What do we usually use `.map()` for in React?
--> Convert an array of raw data into an array of JSX elements
    that can be displayed on the page.


3. Why is using `.map()` better than just creating the components 
    manually by typing them out?
--> It makes our code more "self-sustaining" - not requiring 
    additinal changes whenever the data changes.