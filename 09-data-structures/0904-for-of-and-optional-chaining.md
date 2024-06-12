# Data Structures, Modern Operators, and Strings
## For of loops and Optional Chaining

- for-of loop breaks up each item of a group of inputs, the item variable is always the current elemnt of each iteration
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-14-1.png)

- the entries method in a for-of loop breaks each item into it's own array of the item index and the item itself
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-14-2a.png)

- the two items of each individual array can then be used in a template literal, for example
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-14-2b.png)

- the individual arrays can also be destructured, so that the two elements of each array can be used separately, with their own variable names
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-14-2c.png)

- simpler, es6 way of writing object methods- remove the function word and the colon, see top method vs bottom in this note
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-1.png)

- compute property names in addition to their values, ex by pulling from an array, can also use destructuring
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-2.png)

- when unsure if a property exists, if you try to request it, it will return an error, so first check if the property exists before accessing it's value or nested properties
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-3.png)

- optional chaining- question mark after uncertain property before a dot and the desired value, so if a property doesnt exist, then returns undef, existence means not-nullish, so 0 and empty str exist, but undef and null do not
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-4.png)

- use optional chaining to access properties within a for of loop
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-5a.png)

- set default property if condition isn't met with or logical operator, but this returns error for sat in this ex bc should be open, but it opens at 0, a falsey value
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-5b.png)

- use nullish coalescing operator instead
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-5c.png)

- use optional chaining for calling methods to check if the method exists before calling it
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-6.png)

- use optional chaining for arrays to check contents or if an array is empty, this replaces if else statement
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-7.png)

- for of loop is for looping through arrays- iterable- but there is also a workaround for looping through objects- not interable- need to determine which part to access, key-property or value or both
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-8a.png)

- this technique turns the list of properties, values, or both into an array, which can then be used to compute how many-length
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-8b.png)

- access values that are inside the object by calling the value instead of the key name
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-9.png)

- access the key value pairs inside an object, use entries, like the entries method previous called from for of loop for an array, but this is not an array method
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-10a.png)

- this basically converts the object into an array, which can then be looped through with a for of loop, producing individual arrays for each item in the object
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-10b.png)

- Using destructring  directly inside the for of loop to assign variables to the parts of the object and then use them in the loop
![alt](../images/09-data-structures/0904-for-of-and-optional-chaining/2023-04-20-10c.png)
- 6/12/24: for more complex destructuring like this, it helps to write out the log sentence first, to determine which properties will be used in the destructuring.
