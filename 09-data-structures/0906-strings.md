# Strings

- parameters input in slice method for string are beginning and ending indexes- the first character included in the slice to but not including the last, if no last, through end of string
![alt](../images/09-data-structures/0906-strings/2023-04-27-3a.png) 

- the substring is a new string - does not change the original, it is impossible to mutate a string, as they are primitive data types, to use, put in new variable
![alt](../images/09-data-structures/0906-strings/2023-04-27-3b.png) 

- in some ways, strings can be accessed and manipulated like arrays
![alt](../images/09-data-structures/0906-strings/2023-04-27-1.png) 

- strings can take methods like arrays, ex for indexes
![alt](../images/09-data-structures/0906-strings/2023-04-27-2a.png) 

- index method is case sensitive, so if an item is not found, its index is -1
![alt](../images/09-data-structures/0906-strings/2023-04-27-2b.png) 

- indexOf methods are useful when you don't know exactly the content of the string, or how long the words are, etc- to get first word start at 0 index through first space as string
![alt](../images/09-data-structures/0906-strings/2023-04-27-4.png) 

- negative index on a slice pulls from end of string
![alt](../images/09-data-structures/0906-strings/2023-04-27-5.png) 

- using slice in a function
![alt](../images/09-data-structures/0906-strings/2023-04-27-6.png) 

- even though strings are primitives, they have methods because js treats them like objects with boxing- behind the scenes js converts the string primitive to a string object- puts it in a box
![alt](../images/09-data-structures/0906-strings/2023-04-27-7a.png) 

- even methods called on string objects will return a string primitive because after the method, which converted from string to object, will always convert back to string before return
![alt](../images/09-data-structures/0906-strings/2023-04-27-7b.png) 

- chain together string methods to use more than one at a time
![alt](../images/09-data-structures/0906-strings/2023-04-27-8.png) 

- use replace method to replace parts of strings, will only replace first occurrence, but can chain together
![alt](../images/09-data-structures/0906-strings/2023-04-27-9.png) 

- use replace method to replace parts of strings, will only replace first occurrence, can chain together or replaceAll or use a global regular expression
![alt](../images/09-data-structures/0906-strings/2023-04-27-10.png) 

- includes, startsWith, endsWith return booleans for strings
![alt](../images/09-data-structures/0906-strings/2023-04-27-11.png) 

- split method allows to break a string into multiple parts based on a divider string, then put the parts into an array
![alt](../images/09-data-structures/0906-strings/2023-04-27-12a.png) 

- join method is opposite of split- merges array items into a string
![alt](../images/09-data-structures/0906-strings/2023-04-27-12b.png) 

- Padding a string - adding characters to a string to reach a certain length, 1st input is total string length, 2nd input is what the padding is
![alt](../images/09-data-structures/0906-strings/2023-04-27-13.png) 

- trick to convert a number to a string is to concatenate an empty string to the number
![alt](../images/09-data-structures/0906-strings/2023-04-27-14.png) 

- Repeat method allows to repeat same string multiple times
![alt](../images/09-data-structures/0906-strings/2023-04-27-15.png) 
