# CONSOLE LOG
It is used to  display the output. We pass an argument to it as input data, and this function displays the data. 

```
console.log("Hello, World");
```

We can also pass multiple arguments to it too. 

```
console.log("Hello", "World". "My" "Name" "is" "Param");

```

We can use single quotes, double quote or even backticks in console.log to display data
```
console.log("Hello, World");
console.log('Hello, World');
console.log(`Hello, World`);
```

We can also do arithmetic using console.log.

```
console.log(1+2);
console.log(1-2);
console.log(1/2);
console.log(1*2);
console.log(1**2);
console.log(1%2);
```

# COMMENTS
They are used to add remarks or similar kind of text to our code. This code is not compiled by the compiler. 

## SINGLE LINE COMMENT 
```
// THis is a single line comment.
```

## MULTILINE COMMENT

```
/*
This is a multiline comment.
*/
```

# SYTAX ERROR
Every programming language has it's own syntax. We have to write according to it. Otherwise we will face errors. 
Such errors that occurs due to syntax are called syntax errors. 

```
console.log("Hello, World'); // Quotes are not similar
console.log("Hello, World); // No closing quote
console.log("Hello World"  // No closing paranthesis
```


# ADDING JS TO WEBPAGES 

1. Inline Script
2. Internal Script
3. External Script

## INLINE SCRIPT
This is an example of inline JS
```
<!DOCTYPE html>
<html lang="en">
<head>
<title>30DaysOfScript:Inline Script</title>
</head>
<body>
<button onclick="alert('Welcome to 30DaysOfJavaScript!')">Click Me</button>
</body>
</html>
```

## INTERNAL SCRIPT
This is an example of internal script
```
<!DOCTYPE html>
<html lang="en">
<head>
<title>30DaysOfScript:Internal Script</title>
<script>
    console.log('Welcome to 30DaysOfJavaScript')
</script>
</head>
<body></body>
</html>
```

## EXTERNAL SCRIPT
This is an example of external script

```
<!DOCTYPE html>
<html lang="en">
<head>
<title>30DaysOfJavaScript:External script</title>
<script src="introduction.js"></script>
</head>
<body></body>
</html>
```

# DATA TYPES 
JS have two types of data types. 
1. Primitive Data Types
2. Non-Primitive Data Types

## PRIMITIVE DATA TYPES
1. Numbers
2. Strings
3. Undefined
4. Boolean 
5. Null

### NUMBERS
- Integers - Negative, Zero and Positive 
```
-3, -2, -1, 0, 1, 2, 3
```
- Floating Point NUmbers - Decimal
```
1.1, -1.1, 0.1
```

### STRINGS
Collection of one or more characters. Any data type under single quote, double quote or backtick is a string.
```
'p'
'param'
'paramjeet singh'
```

### UNDEFINED
If we don't assign a value to a variable then the value of that variable is undefined. 

```
var a;
console.log(a); // output - undefined
```

### BOOLEAN 
True or False 

```
true
false
```


### NULL
Empty value 


# CHECKING DATA TYPES
To check the data type of a certain value, we use typeof operator.

```
console.log(typeof 'Param');    // string
console.log(typeof 22);         // number
console.log(typeof true);       // boolean
console.log(typeof a);          // undefined
```


# VARIABLES 
Variables are used to store data. When a variable is declared, a memory location is reserved and when we assing some value to that variable the memory space is filled with that value. 

We can use var, let and const to declare variables. 

Var - Not preferred to use. There are many flaws in this. 
Let - when the value keeps changing. 
Const - when the value didn't change. 

Valid js variable 
- should not start with number
- no keyword should be used as variable
- no special symbol except $ and _
- no space in between 


Valid JS variables examples
```
firstName
lastName
country
city
capitalCity
age
isMarried

first_name
last_name
is_married
capital_city

num1
num_1
_num_1
$num1
year2020
year_2020
```

Commonly we used camelCase in programming. We will use (camelWithOneHump) for variables and (CamelCaseWithTwoHump) for classes.

Invalid variables names
```
  first-name
  1_num
  num_#_1
```

Let us declare variables. We will use let and const only. 

```
//syntax 
let nameOfVariable = value;
```

```
let firstName = "Paramjeet";
let lastName = "Singh";
let age = 22;
let gender = "Male";
let isMarried = false;

console.log(firstName, lastName, age, gender, isMarried);
```


Variables can be declared in a single line also. But to increase readability, it is recommeneded to declare them in different lines. 

```
let firstName = "Paramjeet", lastName = "Singh", age = 22, gender = "Male", isMarried = false;
console.log(firstName, lastName, age, gender, isMarried);
```