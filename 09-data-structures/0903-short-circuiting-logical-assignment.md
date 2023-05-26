# Data Structures, Modern Operators, and Strings
## Short Circuiting and Logical Assignment

### 04/13/23
2023-04-13 27a short circuit- if first value of OR statement is truthy, the first value is immediately returned, if first value is falsey, they second is returned even if its also falsey
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-27a.png)

2023-04-13 27b if multiple values, the first truthy value is returned and the rest go unevaluated
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-27b.png)

2023-04-13 28a instead of using ternary operator, can use short circuiting to define a value
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-28a.png)

2023-04-13 28b neither method works if actual number is zero because that is also falsey, so if you're trying to check if something exists at all and return that number, 0, it will return the next truthy value instead
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-28b.png)

2023-04-13 29 and operator short circuits when first value is falsey, without evaluating rest of statement and returns the first falsey item or the last item, even if it's also truthy
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-29.png)

2023-04-13 30 and operator short circuiting can replace if statement by checking if a method exists, and then applying that method only if it does, and if it doens't, it won't even try to
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-30.png)

2023-04-13 31 to fix the instance where 0 returns falsey instead of the number 0, use two question marks, aka the nullish coalescing operator, which only considers null and undefined as falsey, but 0 or empty string are truthy
![alt](../images/09-data-structures/0901-destructuring/2023-04-13-31.png)
