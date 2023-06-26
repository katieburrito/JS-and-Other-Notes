# Numbers, Dates, Intl, and Timers

## 6/26/23

- because js (and some other languages, ex php, ruby) operates in binary, base 2, some fractions are difficult to represent and can lead to unexpected math results
![alt](images/12-numbers/2023-06-26-1.png)

- convert strings to numbers with number object constructor or just by putting plus sign in front
![alt](images/12-numbers/2023-06-2.png)

#### parseInt
- parseInt will pull a number out of a string, even with spaces, as long as the string starts with the number
- parseInt takes a second parameter, the radix, which is the base of the numeral system (usually 10)
![alt](images/12-numbers/2023-06-3.png)

#### parseFloat
- parseInt only pulls out the integer part of a number, while parseFloat pulls the whole number, including decimal
![alt](images/12-numbers/2023-06-4.png)

- parseInt and parseFloat are global functions, meaning that they will both work without the Number object constructor specified, but it is better practice to use the number object, which provides a "namespace"

- isNaN works with number constructor to identify what is and is not a number (NaN)
![alt](images/12-numbers/2023-06-5.png)

- use isFinite can sometimes be better to check if something is or is not a number because of the idiosyncrasies of isNaN
![alt](images/12-numbers/2023-06-6.png)

