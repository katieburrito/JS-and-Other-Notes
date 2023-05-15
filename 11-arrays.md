# Arrays

## 5/11/23

- call the slice method on an array without any indexes to create a shallow copy, like using the spread operator
![alt](images/11-arrays/2023-05-11-1.png)

- splice method works like slice, but it DOES change the original array by removing whatever is spliced out, while slice does not change the original
![alt](images/11-arrays/2023-05-11-1.png)

- reverse method mutates original array when reversing
![alt](images/11-arrays/2023-05-11-1.png)

- concat method works like spread operator to combine more than one array and also does not mutate the originals
![alt](images/11-arrays/2023-05-11-1.png)

- the at method works like retrieving an array item or string character by its index
![alt](images/11-arrays/2023-05-11-1.png)

- the at method is useful instead of brackets for getting last item in an array of unknown length
![alt](images/11-arrays/2023-05-11-1.png)

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

- map method is like for each loop, but takes a function as an input that creates a new array based on the original array, usually with some operation applied to each original array element
- ![alt](images/11-arrays/2023-05-12-1.png)

- filter method searches the original array for elements that satisfy a particular condition and puts them into a new array

- reduce method combines all values of original array into one single value, ex by adding all numbers together, or another operation, no new array, only the reduced value

- like for each, map method has access to same 3 parameters- current element, current index, and entire array

- using a method instead of a loop (ex a filter method instead of a for of loop with if statements inside) allows for chaining of methods, so you can condense the code more easily

- unlike other methods that take the current element, the current index, and the entire array as their parameters, the reduce method takes the accumulator as its first parameter before the other three parameters

- pass the initial value of the accumulator into the reduce input, after the function
- ![alt](images/11-arrays/2023-05-12-2.png)

