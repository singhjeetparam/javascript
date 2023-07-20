# FUNCTIONS
Reusable piece of code that perform a specific task. A function can be declared in different ways. 
1. Declaration Function 
2. Expression Function 
3. Anonymous Function
4. Arrow Function 


## FUNCTION DECLARATION 
```
//declaring a function without parameters
function functionName(){

}

functionName();
```

## FUNCTION WITHOUT A PARAMETER AND RETURN 
```
function square(){
    let num = 2; 
    console.log(num*num);
}

square(); //4
```

## FUNCTION RETURNING A VALUE 
```
function square(){
    let num = 2; 
    return num*num;
}

console.log(square());
```

## FUNCTION WITH PARAMETER 
```
function square(num){
    return num*num;
}

console.log(square(2));
```

## FUNCTION WITH MANY PARAMETERS
We have two ways to make functions with vary parameters 
1. Using rest parameters
2. Using the argument object 

### REST PARAMETER
```
function sumNumbers(...numbers) {
  var sum = 0;
  for (var i = 0; i < numbers.length; i++) {
    sum += numbers[i];
  }
  return sum;
}

var result = sumNumbers(5, 10, 15);
console.log(result); // Output: 30

```

### ARGUMENT OBJECT 
```
function sum(){
  let sum = 0; 
  for(let i = 0; i<arguments.length; i++){
    sum+=arguments[i];
  }
  
  console.log(sum);
}

sum(1,2,3,4,5);
```

## ARROW FUNCTION WITH MANY PARAMETERS
Arrow function didn't have any argument object, so we only have to use rest operator. 

```
const sum = (...num) =>{
    console.log(num);
}

sum(1,2,3,4,5);
```
## ANONYMOUS FUNCTION
Function without any name. 
```
const anonymouseFunc = function(){
    console.log("This is a anonymous function)
}
```

## SELF INVOKING FUNCTION 
They are anonymous function that aren't need to be called to return a value. 
```
(function(n){
    console.log(n)
})(2)
```

## ARROW FUNNCTION 
It's just an alternative to define a function 
```
//normal function 
function square(n){
    return n*n;
}
console.log(square(2));

```

## SCOPE
It refers to the context in which a variable, functions and objects are defined and can be accessed.

There are two types of scope. 
1. Global Scope
2. Local Scope 


### GLOBAL SCOPE
A globally declared variables, functions and objects can be accessed everywhere in the same file. 

```
//scope.js
let a = 'JavaScript' // is a global scope it will be found anywhere in this file
let b = 10 // is a global scope it will be found anywhere in this file
function letsLearnScope() {
  console.log(a, b) // JavaScript 10, accessible
  if (true) {
    let a = 'Python'
    let b = 100
    console.log(a, b) // Python 100
  }
  console.log(a, b)
}
letsLearnScope()
console.log(a, b) // JavaScript 10, accessible
```

### LOCAL SCOPE
A variable declared as a local can be accessed only in  a certain block code. 

```
//scope.js
let a = 'JavaScript' // is a global scope it will be found anywhere in this file
let b = 10 // is a global scope it will be found anywhere in this file
// Function scope
function letsLearnScope() {
  console.log(a, b) // JavaScript 10, accessible
  let value = false
// block scope
  if (true) {
    // we can access from the function and outside the function but 
    // variables declared inside the if will not be accessed outside the if block
    let a = 'Python'
    let b = 20
    let c = 30
    let d = 40
    value = !value
    console.log(a, b, c, value) // Python 20 30 true
  }
  // we can not access c because c's scope is only the if block
  console.log(a, b, value) // JavaScript 10 true
}
letsLearnScope()
console.log(a, b) // JavaScript 10, accessible
```

