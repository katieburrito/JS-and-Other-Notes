# Data Structures, Modern Operators, and Strings

## Destructuring Arrays and Objects

### 4/13/23
- destructure an array buy setting the variables you'd like to assign to each item in array equal to the array itself, note original array is still intact and accessible as well
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-1.png)

- array items are matched to variables in order, skip an item by leaving a blank between commas
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-2.png)

- clunkier method to switch array items by first reassigning to a temporary variable to store the value while switching
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-3a.png)

- easier method to switch placement-order of array items with destructuring by just reassigning
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-3b.png)

- create a method inside an object, then call that method, and access the arrays inside the object to create a new array
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-4a.png)

- destructure the array to assign variables to the individual array elements inside the object, allows you to receive more than one variable from just one function call
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-4b.png)

- use destructing to access nested array contents
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-5a.png)

- or destructure nested array at same time as parent array with additional square brackets
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-5b.png)

2023-04-13 6 assign default values to destructed array variables before equating them to the array, so that in the case that there is no matching array item, it does not just equal undefined
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-6a.png)

2023-04-13 6 unlike destructuring arrays, in objects, order doesn't matter, so you don't need to leave blanks with commas to skip parts, instead specify the property keys as the variables
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-6b.png)

2023-04-13 7 to change the variable names of object items, reference the property names first followed by a colon and the new name, this is especially useful when using 3rd party data, like from APIs
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-7.png)

2023-04-13 8 like with arrays, you can assign default values for the variables, in case a desired property is not in the original object to avoid undefined result, combine rename with default with colon and equals sign
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-8.png)

2023-04-13 9 cant start w const bc changing values, nor let bc the let is already declared before for a and b, cant start a line w curly braces bc js expects a code block, so wrap all in parenthesis when mutating variables in an object
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-9.png)

2023-04-13 10a destructure nested objects
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-10a.png)

2023-04-13 10b destructure nested objects and rename the variables
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-10b.png)

2023-04-13 11 define default values within the object parameters, in case the argument does not have an assigned value
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-11.png)

2023-04-13 12 the spread operator, written with three ellipsis dots, allows you to expand an array into all of its elements at once, instead of doing it manually, can then insert into new array, or access the entire array contents outside of the array
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-12.png)
