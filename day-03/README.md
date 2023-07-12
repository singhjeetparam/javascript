# BOOLEAN
Boolean data type has only two values - true or false. 

```
let isLightOn = true
let isRaining = false
let isHungry = false
let isMarried = true
let truValue = 4 > 3    // true
let falseValue = 4 < 3  // false
```

## TRUTHY VALUE 
- All numbers either positive or negative except 0 .
- All strings except empty string. 
- boolean true

## FALSY VALUE
- 0 
- null 
- undefined 
- NaN
- boolean false 

# UNDEFINED
When we declare a variable but didn't assign any value to it. 

```
let firstName; 
console.log(firstName);
```


# NULL 
null means no value 
```
let empty = null; 
console.log(empty);
```

# OPERATORS

1. Assignment Operator - equal sign is used to assign a value to a variable. 
```
let a = 10;
```

2. Arithmetic Operator - Used for mathematical operators. 
- Addition : +
- Subtraction : -
- Multiplication : *
- Division : /
- Modulus : %
- Eponential : ** 

```
let numOne = 4
let numTwo = 3
let sum = numOne + numTwo
let diff = numOne - numTwo
let mult = numOne * numTwo
let div = numOne / numTwo
let remainder = numOne % numTwo
let powerOf = numOne ** numTwo

console.log(sum, diff, mult, div, remainder, powerOf) // 7,1,12,1.33,1, 64

```

3. Comparison Operator - used for comparison 
 - Equivalent(equal in value only) : ==
 - Exactly equal (equal in value and data type) : ===
 - Greater than :  > 
 - Greater than or equal to : >=
 - Smaller than : <
 - Smaller than or equal to : <=

 ```
 console.log(3 > 2)              // true, because 3 is greater than 2
console.log(3 >= 2)             // true, because 3 is greater than 2
console.log(3 < 2)              // false,  because 3 is greater than 2
console.log(2 < 3)              // true, because 2 is less than 3
console.log(2 <= 3)             // true, because 2 is less than 3
console.log(3 == 2)             // false, because 3 is not equal to 2
console.log(3 != 2)             // true, because 3 is not equal to 2
console.log(3 == '3')           // true, compare only value
console.log(3 === '3')          // false, compare both value and data type
console.log(3 !== '3')          // true, compare both value and data type
console.log(3 != 3)             // false, compare only value
console.log(3 !== 3)            // false, compare both value and data type
console.log(0 == false)         // true, equivalent
console.log(0 === false)        // false, not exactly the same
console.log(0 == '')            // true, equivalent
console.log(0 == ' ')           // true, equivalent
console.log(0 === '')           // false, not exactly the same
console.log(1 == true)          // true, equivalent
console.log(1 === true)         // false, not exactly the same
console.log(undefined == null)  // true
console.log(undefined === null) // false
console.log(NaN == NaN)         // false, not equal
console.log(NaN === NaN)        // false
console.log(typeof NaN)         // number

console.log('mango'.length == 'avocado'.length)  // false
console.log('mango'.length != 'avocado'.length)  // true
console.log('mango'.length < 'avocado'.length)   // true
console.log('milk'.length == 'meat'.length)      // true
console.log('milk'.length != 'meat'.length)      // false
console.log('tomato'.length == 'potato'.length)  // true
console.log('python'.length > 'dragon'.length)   // false
 ```

4. Logical Operator - &&(ampersand) , ||(pipe) and !(negation). The && operator gets true only if the two operands are true. The || operator gets true either of the operand is true. The ! operator negates true to false and false to true.
```
// && ampersand operator example

const check = 4 > 3 && 10 > 5         // true && true -> true
const check = 4 > 3 && 10 < 5         // true && false -> false
const check = 4 < 3 && 10 < 5         // false && false -> false

// || pipe or operator, example

const check = 4 > 3 || 10 > 5         // true  || true -> true
const check = 4 > 3 || 10 < 5         // true  || false -> true
const check = 4 < 3 || 10 < 5         // false || false -> false

//! Negation examples

let check = 4 > 3                     // true
let check = !(4 > 3)                  //  false
let isLightOn = true
let isLightOff = !isLightOn           // false
let isMarried = !false                // true
```

5. Increment Operator - It increases the value. This increment can be post or pre. 
 - Pre Increment 
 ```
 let count = 0
console.log(++count)        // 1
console.log(count)          // 1
```

- Post Increment 
```
let count = 0
console.log(count++)        // 0
console.log(count)          // 1
```
6. Decrement Operator - It decreases the value. This is also post and pre. 
 - Pre Decrement 
 ```
 let count = 0
console.log(--count) // -1
console.log(count)  // -1
 ```

- Post Decrement 

```
let count = 0
console.log(count--) // 0
console.log(count)   // -1
```

7. Ternary Operators -  They allows us to write conditions. Like we do using if and else. 

```
let isRaining = true
isRaining
  ? console.log('You need a rain coat.')
  : console.log('No need for a rain coat.')

isRaining = false
isRaining
  ? console.log('You need a rain coat.')
  : console.log('No need for a rain coat.')
```

# WINDOWS METHODS 
## WINDOWS ALERT
This generates a alert box on our webpage. 
```
alert('My name is Param')
```

## WINDOWS PROMPT
This method generates a prompt box with an input on our browser to take input values and this input value can be stored in a variable. 

```
let number = prompt('Enter number', 'number goes here')
console.log(number)
```

## WINDOW CONFIRM
This displays a dialog box with specific message along with an OK button and cancel button. It seeks permission from user to execute something. 
```
const agree = confirm('Are you sure you like to delete? ')
console.log(agree) // result will be true or false based on what you click on the dialog box
```



# DATE OBJECT 
It is used to get date and time.It has the following objects -  getFullYear(), getMonth(), getDate(), getDay(), getHours(), getMinutes, getSeconds(), getMilliseconds(), getTime(), getDay()

## CREATING A TIME OBJECT 
```
const now = new Date();
console.log(now)
```