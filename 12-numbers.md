# Numbers, Dates, Intl, and Timers

## 6/26/23

- because js (and some other languages, ex php, ruby) operates in binary, base 2, some fractions are difficult to represent and can lead to unexpected math results
![alt](images/12-numbers/2023-06-26-1.png)

- convert strings to numbers with number object constructor or just by putting plus sign in front
![alt](images/12-numbers/2023-06-26-2.png)

#### Number.parseInt
- parseInt will pull a number out of a string, even with spaces, as long as the string starts with the number
- parseInt takes a second parameter, the radix, which is the base of the numeral system (usually 10)
![alt](images/12-numbers/2023-06-26-3.png)

#### Number.parseFloat
- parseInt only pulls out the integer part of a number, while parseFloat pulls the whole number, including decimal
![alt](images/12-numbers/2023-06-26-4.png)

- parseInt and parseFloat are global functions, meaning that they will both work without the Number object constructor specified, but it is better practice to use the number object, which provides a "namespace"

#### Number.isNaN
- isNaN works with number constructor to identify what is and is not a number (NaN)
![alt](images/12-numbers/2023-06-26-5.png)

#### Number.isFinite
- use isFinite can sometimes be better to check if something is or is not a number (instead of a string) because of the idiosyncrasies of isNaN (ex, Infinity
![alt](images/12-numbers/2023-06-26-6.png)

#### Number.isInteger
- isInteger checks if input is an integer number

#### Roots of Numbers
- use sqrt Math method (square root only) or exponentiation to a fractional root to get square, cube, etc roots

#### maximum/ minimum
- Math.max and Math.min will automatically perform type coercion, so that if some of the number inputs are written as strings, they will be automatically converted to numbers for the max/mincalculation
- Math.max/min does not parse numbers from strings that include other characters though
![alt](images/12-numbers/2023-06-26-7.png)

#### Rounding
- Math.trunc simply removes any numbers after decimal point
- Math.round will actually round up or down
- Math.ceil (ceiling) will automatically round up
- Math.floor will automatically round down
- all of these math rounding methods will also automatically do type coercion on string inputs
![alt](images/12-numbers/2023-06-26-8a.png)
- with negatives, trunc still just removes after decimal, but rounding is more negative for floor, and less negative for ceiling
![alt](images/12-numbers/2023-06-26-8b.png)
- toFixed allows you to specify number of decimal places, but returns a string, not a number, so convert to number with number constructor or plus sign
- toFixed converts to a string because it is a primitive and (similar to string methods), and primitives can't have methods, so first it is converted to string via boxing, before performing the operation
![alt](images/12-numbers/2023-06-26-8c.png)

#### Remainder (modulo)
- percentage sign is symbol for remainder operator, returns the remainder only of the division of two numbers
![alt](images/12-numbers/2023-06-26-9.png)

#### Numeric Separators
- Numeric separators- underscores(_) (like comma in math) separate numbers, to make the code easier to read, but they are not logged in the console
![alt](images/12-numbers/2023-06-27-1a.png)
- be mindful that because the underscore is not really part of the number and only for ease of reading that regardless of where it is placed, it will really be the same number, even though in one case you might use it like a comma to indicate thousands, and in another like a period to indicate cents
![alt](images/12-numbers/2023-06-27-1b.png)
- numeric separator can only be placed between numbers (ex: not number and decimal, not two in a row, not at beginning, not at end of number)
![alt](images/12-numbers/2023-06-27-1c.png)
-number separate also doesn't work when converting with number object operator- js won't be able to parse the number correctly from the string
- also doesn't work with parseInt because only first part before the underscore will be pulled
![alt](images/12-numbers/2023-06-27-1d.png)

#### BigInt Primitive Data Type 
- 64bit limit: there are 64 0's or 1's to represent any given number
- only 53 bits are allowed for the numerals themselves, the other 11 are for decimals, sign, etc
- because of this, the largest number js can represent is 2 (for 0 or 1- base 2) raised to the 53 power (minus 1 because count starts at 0, not 1
- this information is also stored in the MAX_SAFE_INTEGER in the number static data property
- any integer larger than the max safe integer is not safe, meaning it cannot be accurately represented
![alt](images/12-numbers/2023-06-27-2a.png)
- add an "n" to the end of large numbers to indicate that they are "Bigint"
- or use "BigInt" constructor function to indicate big integer- can be problematic because first js has to interpret the large number before adding n to end
![alt](images/12-numbers/2023-06-27-2b.png)
- BigInt can be combined with other BigInt, but not regluar numbers because the BigInt cannot be converted to a regular number
![alt](images/12-numbers/2023-06-27-2c.png) 
- As a workaround, use the BigInt constructor function on the regular number first
![alt](images/12-numbers/2023-06-27-2d.png) 
 

