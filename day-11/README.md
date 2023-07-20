# DESTRUCTURING AND SPREAD 

## DESTRUCTURING 
It is a way to unpack arrays, and objects and assigning to a distinct variable. 

### DESTRUCTURING ARRAYS 
```
const num = [1,2,3];
let [numOne, numTwo, numThree] = num;
console.log(numOne, numTwo, numThree);
```
```
const fullStack = [
  ['HTML', 'CSS', 'JS', 'React'],
  ['Node', 'Express', 'MongoDB']
]
const [frontEnd, backEnd] = fullStack

console.log(frontEnd)
console.log(backEnd)
```

If we want to skip on the values in the array we can use additional commas. It'll help to omit the value at that specific index. 

```
const num = [1,2,3];
const [numOne, , numThree] = num;
console.log(numOne, numThree);
```

We can also use default values in case the value of array for that index is undefined.

```
const num = [undefined, 2, 3];
const [
    numOne = 1, 
    numTwo,
    numThree
] = num; 
console.log(numOne, numTwo, numThree);
```

We cannot assign variable to all the elements of an array. That will be hectic work. So we can use spread operator to do so. The rest operator will provide us an array of the remaining elements
```
const num = [1,2,3,4,5,6,7,8,9,0];
let [numOne, numTwo, numThree, ...rest] = num;
console.log(numOne, numTwo, numThree, rest);
```

### DESTRUCTURING DURING ITERATION
```
const countries = [['Finland', 'Helsinki'], ['Sweden', 'Stockholm'], ['Norway', 'Oslo']]

for (const [country, city] of countries) {
console.log(country, city)
}
```

### DESTRUCTURING OBJECTS
When we destructure an object. The variable name should be same as the key name of the object. 
```
const rectangle = {
  width: 20,
  height: 10,
  area: 200
}
let { width, height, area, perimeter } = rectangle

console.log(width, height, area, perimeter)
```

### RENAMING DURING DESTRUCTURING 
we can also change the variables name at the time of destructuring. 
```
onst rectangle = {
  width: 20,
  height: 10,
  area: 200
}
let { width: w, height: h, area: a, perimeter: p } = rectangle

console.log(w, h, a, p)
```


### OBJECT PARAMETER WITHOUT DESTRUCTURING
```
// Without destructuring
const rect = {
  width: 20,
  height: 10
}
const calculatePerimeter = rectangle => {
  return 2 * (rectangle.width + rectangle.height)
}

console.log(calculatePerimeter(rect)) // 60
//with destructuring
```


### OBJECT PARAMETER WITH DESTRUCTING
```
const calculatePerimeter = ({ width, height }) => {
  return 2 * (width + height)
}

console.log(calculatePerimeter(rect)) // 60

```
## SPREAD OR REST OPERATOR
When we destructure an array we use the spread operator to get the rest of the elements as array. 

### SPREAD OPERATOR TO GET THE REST OF ARRAY ELEMENT. 

```
const num = [1,2,3,4,5,6,7,8,9,0];
let [num1, ...rest] = num;
console.log(num1);
console.log(rest);
```

### SPREAD OPERATOR TO COPY ARRAY 
```
const evens = [0,2,4,6,8,10];
const even = [...evens];
console.log(even);
```

### SPREAD OPERATOR TO COPY AN OBJECT

```
const user = {
  name:'Asabeneh',
  title:'Programmer',
  country:'Finland',
  city:'Helsinki'
}

const copiedUser = {...user}
console.log(copiedUser)
```

### MODIFYING OR CHANING THE OBJECT WHILE COPYING 
```const user = {
  name:'Asabeneh',
  title:'Programmer',
  country:'Finland',
  city:'Helsinki'
}

const copiedUser = {...user, title:'instructor'}
console.log(copiedUser)
```

### SPREAD OPERATOR WITH ARROW FUNCTIONS
Whenever we have to pass unlimited number or arguments we can use spread operator

```
const sumOfAll = (...args) =>{
    let sum = 0; 
    for(const n of args){
        sum += n;
    }
    
    console.log(sum)
}

sumOfAll(1,2,3,4,5,6);
```