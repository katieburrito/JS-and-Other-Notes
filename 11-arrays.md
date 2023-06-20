# Arrays

## 5/11/23

#### Slice Method
- call the slice method on an array without any indexes to create a shallow copy, like using the spread operator
![alt](images/11-arrays/2023-05-11-1.png)

#### Splice Method
- splice method works like slice, but it DOES change the original array by removing whatever is spliced out, while slice does not change the original
![alt](images/11-arrays/2023-05-11-1.png)

#### Reverse Method
- reverse method mutates original array when reversing
![alt](images/11-arrays/2023-05-11-1.png)

#### Concat Method
- concat method works like spread operator to combine more than one array and also does not mutate the originals
![alt](images/11-arrays/2023-05-11-1.png)

#### At Method
- the at method works like retrieving an array item or string character by its index
![alt](images/11-arrays/2023-05-11-1.png)

- the at method is useful instead of brackets for getting last item in an array of unknown length
![alt](images/11-arrays/2023-05-11-1.png)

#### For Each Loops
- you cannot break out of a for each loop- continue and break statements do not work, instead, for each always loops through entire array, so if that is the desired behavior, use a for of loop instead

- for each method is similar to for of loop method, but simpler, for each is a higher order function with a callback function inside
![alt](images/11-arrays/2023-05-11-1.png)

- to deconstruct, like in for of loop in a for each loop, first parameter is current element, second is the current index, third is the entire array being looped
![alt](images/11-arrays/2023-05-11-1.png)

- in maps for each loops, first parameter is the current value, second is the key, and third is the entire map that is being looped over
![alt](images/11-arrays/2023-05-11-1.png)

- in a set, the key and value parameters are the same because a set doesn't have keys, but the parameter still exists to follow the same pattern as for each loops for other iterables
![alt](images/11-arrays/2023-05-11-1.png)

- replace the "key" variable with an underscore, a throwaway variable
![alt](images/11-arrays/2023-05-11-1.png)

- insertAdjacentHTML takes 2 string inputs- first the position at which to attach the html, second is the string of the html to be inserted
![alt](images/11-arrays/2023-05-11-1.png)

## 5/12/23

#### Map Method
- map method is like for each loop, but takes a function as an input that creates a new array based on the original array, usually with some operation applied to each original array element
- ![alt](images/11-arrays/2023-05-12-1.png)

#### Filter Method
- filter method searches the original array for elements that satisfy a particular condition and puts them into a new array

#### Reduce Method
- reduce method combines all values of original array into one single value, ex by adding all numbers together, or another operation, no new array, only the reduced value

- like for each, map method has access to same 3 parameters- current element, current index, and entire array

- using a method instead of a loop (ex a filter method instead of a for of loop with if statements inside) allows for chaining of methods, so you can condense the code more easily

- unlike other methods that take the current element, the current index, and the entire array as their parameters, the reduce method takes the accumulator as its first parameter before the other three parameters

- pass the initial value of the accumulator into the reduce input, after the function
- ![alt](images/11-arrays/2023-05-12-2.png)

## 5/22/23

#### Chaining Methods
- Methods can be chained together as long as the method returns a new array (ex: filter, map methods) for the next method in the chain to use. 
- No other method can follow reduce method because its output is not a new array/
- The problem with chaining methods is that it is difficult to tell which step produces a bug when it doesn't work as expected.

- use the array parameter that comes with the method to log the entire array when looking for a bug
- the logged array will be the current step's array, meaning the array that was the output of the previous step's method
![alt](images/11-arrays/2023-05-22-1.png)

- Be careful not to overuse chaining. For really large arrays, to continually produce and cycle through new arrays in the chain can create performance issues. For large arrays, try to compress into as few methods as possible.
- Bad practice in js to chain methods that mutate the original array (ex: splice, reverse).

## 5/26/23

#### Find Method
- use find method to retrieve one element of an array based on a condition
- find method accepts a condition and callback function as inputs, then loops over array with the inputs
- find method only returns the first element in the array that meets the condition, not a new array

- prevent default method on an event will prevent its default behavior, in this case a submit button would normally reload the page, so prevent it
![alt](images/11-arrays/2023-05-26-1.png)
- a user hitting enter while the focus is in either the user or pin text input boxes will also trigger the click event

- because assignment operator works from right to left, to set two different variables to the same value, can set them equal to each other with the new value last (to the right) and both will be reassigned in the same line of code
![alt](images/11-arrays/2023-05-26-2.png)

- blur method removes focus from current selected element, in this case the pin input field
![alt](images/11-arrays/2023-05-26-3.png)

## 5/30/23
- it's very common to use prevent default when working with forms because without, the submit button would always reload the page, which often isn't desired

### findIndex method
- find index method is similar to find method but returns that element's index instead of the element itself
- like find, findIndex method can access not just current element, but also index as well as entire array as input parameters

## 5/31/23

### Some and Every methods
- includes method checks for equality- if an array contains an exact value and returns a boolean
- some and every check for conditions
- some returns true if any element in the array satisfies the set condition
- every returns true only if every element in the array satisfies the set condition
- separate the callback function when reusing it with different methods to keep the code dry
![alt](images/11-arrays/2023-05-31-1.png)

### flat and flatMap method
- flat method combines all smaller, nested array elements into one "flattened" array
- flat method does not require a callback function
- By default, the flat method only works for one layer deep of nested arrays (default depth of 1).
![alt](images/11-arrays/2023-05-31-2a.png)
- Passing in a depth argument allows you to set deeper array nesting for flat method on an array
![alt](images/11-arrays/2023-05-31-2b.png)
- It is very common practice to use a map method on an array and then flatten the results, so an entire separate method, flatMap was created for this exact purpose.
- flatMap only goes one level deep in nesting, and cannot be changed like separate flat method

### Sorting Arrays
- By default, sort method organizes array elements alphabetically from A-Z by first character
- Sort method mutates the original array, so the order is permanently changed.
![alt](images/11-arrays/2023-05-31-3a.png)
- With numbers, the sort still organizes by the first character (low to high) rather than the entire number
![alt](images/11-arrays/2023-05-31-3b.png)
- This default is because the sort method treats the elements as strings, rather than numbers.
- The workaround for numbers treated as strings in sort method is to pass a callback function.
- Sort method continues looping over the array and applying the callback function to each consecutive pair of elements to compare them until they are all sorted in ascending
![alt](images/11-arrays/2023-05-31-4.png)
- The simplified version of the if statement to sort ascending/descending is to return either a positive or negative simply by subtracting one number from the previous.
![alt](images/11-arrays/2023-05-31-5.png)
- MDN Explanation of [sort](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)
- A mixed array of numbers, strings, etc isn't a good application for sort method.
- By default, sort modifies the original array, so to prevent this, take a copy of the array with the slice method and chain the sort method to that instead.
![alt](images/11-arrays/2023-05-31-6.png)

## 6/20/23

#### Other Ways of Creating/ Filling Arrays

- using constructor to produce array with only one argument, the number specified is the array length containing the empty elements, not the array contents
![alt](images/11-arrays/2023-06-20-1a.png)
- creating an array with empty elements like this is not very useful- cannot apply methods, as result will be the same because the elements are empty
![alt](images/11-arrays/2023-06-20-1b.png)
- *** the exception here is the fill method can be called on an array of empty elements
- fill method fills the entire array with the argument passed, and mutates the original array
![alt](images/11-arrays/2023-06-20-2a.png)

- first argument passed in fill method is the content- what element to fill with
- second and third arguments passed in fill method are the starting and ending index for the fill (like slice method)
![alt](images/11-arrays/2023-06-20-2b.png)
- fill can also be used on non-empty arrays, and will mutate the original, replacing specified elements with the fill element
![alt](images/11-arrays/2023-06-20-2c.png)

- from method is not applied to an existing array, but directly to the array constructor
- first argument in from method is length object
- second argument in from method is a function that returns the fill element
![alt](images/11-arrays/2023-06-20-3a.png)
- as with some other callback functions, the callback function that is the second argument of the from method also can access the current element, as well as that element's index
![alt](images/11-arrays/2023-06-20-3b.png)
- use an underscore as a placeholder for "throwaway variables." Here, the current element is not needed for the function, but it is automatically the first accessible parameter, so skip it with the underscore
![alt](images/11-arrays/2023-06-20-3c.png)




