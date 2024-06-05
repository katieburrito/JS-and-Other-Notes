# Data Structures, Modern Operators, and Strings

## Spread and Rest

### 4/13/23

- for functions with a lot of parameters, you can pass an object into the function, and the function will destructure the object automatically
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-13.png)

- the spread operator is similar to destructuring an array, but does not assign to variables, and can only be used in places where values would be comma-separated
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-14.png)

- the spread operator copies the contents of one array into another, which can be helpful for joining two or more arrays
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-15.png)

- like arrays, strings, maps, and sets are also iterables, and can take the spread operator (Objects are not iterable and cannot take spread operator. Also can't use spread operator for js input template literal becasue its not a place that expects comma separated variables.)
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-16.png)

- use forward slash to escape the apostrope inside of string, so that js doesn't read it as the end of the string
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-17.png)

- use spread operator to insert the contents of an array of prompt results as the arguments in an object method
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-18.png)

- spread operator can also be used to copy objects, and then modify if needed, order of items does not matter, changing copy does not change original
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-19.png)

- spread vs rest behavior determined by which side of assignment operator they appear, rest element must be last listed
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-20.png)

- rest pattern is also three ellipsis dots like spread operator, but with reverse behavior- collects multiple elements and combines into array, called rest because it takes the rest of the remaining elements not explicitly selected
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-21.png)

- assigning spread operator on right to variables declared by rest operator, rest operator collects all elements after last specifically stated, not those before or between, in this case the skipped pasta from main menu
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-22.png)

- using rest operator in objects
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-23.png)

- instead of specifying multiple arguments when calling a function, use rest arguments to combine them first, then call the function on the one whole argument that includes all of the individual items
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-24.png)

- using rest to collect function arguments, when there is nothing for the rest parameter, it returns undefined
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-25.png)

- spread operator is used where we would otherwise write values separated by a comma, rest operator is used where we would otherwise write variable names separated by a comma
![alt](../images/09-data-structures/0902-spread-and-rest/2023-04-13-26.png)

