# Sets and Maps

- create a set with new Set keywords then pass it an iterable inside the parenthesis
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-1a.png)

- sets are like arrays in that they have individual items, io key-value pairs, but different bc each element is unique, even if passed duplicates and order doesn't matter
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-1b.png)

- strings are also iterable, and so can be passed into a set
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-2.png)

- check size or info contained in a set
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-3a.png)

- add or delete method for sets allows you to change contents
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-3b.png)

- empty the set with clear
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-3c.png)

- this doesn't work- sets do not have indexes like arrays, so there is no way to get data out of a set. It's not necesary to get the data like an array because order doesn't matter and there are no duplicates, so the only thing to check is whether an item is in the set or not using the has method.
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-4.png)

- sets are iterable and so can be looped through
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-5.png)

- the main use for a set is to remove duplicate values from an array
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-6.png)

- because both sets and arrays are iterable, set can be converted to array with spread operator
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-21-7.png)

- 6/14/24: because strings are also iterable, you can use set methods to work with strings too (like size to find the number of unique characters in the string)

- the easiest way to create a map is to create an empty map without passing anything in
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-1a.png)

- and then pass the info with the set method listing key value pairs
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-1b.png)

- the set method automatically returns the updated map with the data that was passed in the method
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-2.png)

- chain each key value setting for the map to the previous with period dot between
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-3.png)

- use get method with key property passed in
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-4.png)

- with booleans as the keys, you can access different data in the map, depending on conditions
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-5.png)

- use has to check if a method contains a certain key and delete with delete method, and size to check how many pairs it contains
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-6.png)

- clear method deletes the map
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-7.png)

- the 1,2 array here is not the same object in the heap from when it was set to when it was called
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-8a.png)

- for js to understand which array you're referencing, store it in a variable first
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-8b.png)

- with this technique- storing info in variable first, objects can be used as map keys
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-24-8c.png)

- instead of using cumbersome set method to populate a map, especially for maps with more data, use an array containing multiple arrays
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-1.png)

- the array of arrays returned in a map is the same structure as calling object entries- this means objects can easily be converted into maps
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-2.png)

- convert an object to a map by passing the object into a new map variable
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-3.png)

- maps are iterable with loops
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-4.png)

- convert a map to a array with the spread operator
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-5.png)

- data sources and storage in js
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-6a.png)

- arrays vs sets
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-6b.png)

- objects vs maps
![alt](../images/09-data-structures/0905-sets-and-maps/2023-04-25-6c.png)
