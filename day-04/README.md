# CONDITIONALS
They are used to make decisions based on conditions. 

1. If
2. If Else 
3. If Else If Else
4. Switch 
5. Ternary Operatory

## IF 
It is used to check whether a condition is true and to execute block code. 
```
if(condition){
    //block code
}
```

Example 
```
let isRaining = true
if (isRaining) {
  console.log('Remember to take your rain coat.')
}
```


## IF ELSE 
If first condition is true the it'll be executed and if not then the second one will be executed. 

```
if(condition){
    // if this condition is true this block will run 
}
else{
    //this block will run 
}
```

Example
```
let num = 3
if (num > 0) {
  console.log(`${num} is a positive number`)
} else {
  console.log(`${num} is a negative number`)
}
//  3 is a positive number

num = -3
if (num > 0) {
  console.log(`${num} is a positive number`)
} else {
  console.log(`${num} is a negative number`)
}
//  -3 is a negative number
```

## IF ELSE IF ELSE
when we have multiple conditions. 
```
if(condition){
    //code
}
else if(condition){
    //code
}
else{
    //code
}
```

Example
```
let a = 0
if (a > 0) {
  console.log(`${a} is a positive number`)
} else if (a < 0) {
  console.log(`${a} is a negative number`)
} else if (a == 0) {
  console.log(`${a} is zero`)
} else {
  console.log(`${a} is not a number`)
}
```

## SWITCH 
It is an alternative of if else if else. 

```
switch(caseValue){
  case 1:
    // code
    break
  case 2:
   // code
   break
  case 3:
   // code
   break
  default:
   // code
}
```

Example -
```
let weather = 'cloudy'
switch (weather) {
  case 'rainy':
    console.log('You need a rain coat.')
    break
  case 'cloudy':
    console.log('It might be cold, you need a jacket.')
    break
  case 'sunny':
    console.log('Go out freely.')
    break
  default:
    console.log(' No need for rain coat.')
}
```