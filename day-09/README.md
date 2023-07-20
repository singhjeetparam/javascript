# HIGHER ORDER FUNCTIONS
HOFs are functions which take other function as a parameter or return a funtion as a value. This function that is passed as a parameter is called a callback. 

## CALLBACK 
A function which can be passed as a parameter to other function. 

```
const callback = (n) =>{
    return n*2;
}

function cube(callback, n){
    return callback(n)*n;
}

console.log(cube(callback, 3))
```

## RETURNING FUNCTION
HOF return function as a value. 
```
const higherOrder = n =>{
    const doSomething = m =>{
        const doWhatEver = o = > {
            return n*m*o;
        }
        return doWhatEver;
    }
    return doSomething;
}

console.log(higherOrder(2)(3)(4));
```

Where can we use callback function. ForEach is the perfect example of this. 
```
const num = [1,2,3,4,5];
const sumNum = arr =>{
    let sum = 0;
    arr.forEach(function(e){
        sum+=e;
    })
    return sum;
}

console.log(sumNum(num))
```


#SETTING TIME
In JS, We can execute some activities in a certain interval of time or we can schedule it too. 

1. setInterval - It performs a function after a certain period of time, until it is stopped. 

```
funtion sayHello(){
    console.log("Hello);
}

setInterval(sayHello, 1000);
```

This will print hello after every 1 second with stopping.  To stop this we need to use clearInterval()

```
funtion sayHello(){
    console.log("Hello);
}

setInterval(sayHello, 1000);
```

2. setTimeout - It is used to perfrom a some action after sometime in future. This method takes a callback function and a duration as parameter.
```
function sayHello() {
  console.log('Hello')
}
setTimeout(sayHello, 2000)
```
this will print hello after 2 seconds. 


# FUNCITONAL PROGRAMMING
Instead of writing regular loops we have built-in methods which can help us to solve complicated problems.

1. forEach() - iterate an array element. 

```
arr.forEach(function(element, index, arr){
    console.log(element, index, arr);
})
//above code can be written as 
arr.forEach((element, index, arr) => {
    console.log(element, index, arr);
})
//the above code can be written as
arr.forEach((element, index, arr) => console.log(element, index, arr));
```

eg- 
```
let arr = [1,2,3,4,5]
let sum = 0; 
arr.forEach((e) => {
    sum+=e;
});
console.log(sum);
```

2. map() - it iterates an array and modify it's element. It returns a new array 

```
const arr = [1,2,3,4,5];
const arrSquare = arr.map((n) => n*n);
console.log(arrSquare);
```

3. filter() - it filter out items which fulfill filtering conditions and return a new array. 

```
const countries = ['ALBANIA', 'BOLIVIA', 'CANADA', 'DENMARK', 'ETHIOPIA', 'FINLAND', 'GERMANY', 'HUNGARY', 'IRELAND', 'JAPAN', 'KENYA']

const countriesContainingLand = countries.filter((country) => country.includes("LAND"));

console.log(countriesContainingLand)
```

4. every() - it checks if all the elements are similar in one aspect. It returns a boolean.

```
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook']
const areAllStr = names.every((name) => typeof name === 'string') // Are all strings?

console.log(areAllStr)
```

5. find() - return the first element which satisfies the condition

```
const ages = [24,22,25,32,33,45];
const age = ages.find((age) => age > 20);
console.log(age)
```

6. findIndex() - return the index of first element which satisfies the condition

```
const ages = [24, 25, 26, 27, 28, 29, 30];
const age = ages.findIndex((age) => age > 25);
console.log(age);
```

7. some() - it check if some of the elements are similar in one aspect. It returns boolean. 

```
const bools = [false, true];

const areSomeTrue = bools.some((b) =>  b === true);

console.log(areSomeTrue);
```

8. reduce() - it takes an array, applies a callback function to each element of the array and accumulates the result to form a single value. Or it reduces the array based on the callback function to a single value. 

```
const numbers = [2, 4, 6, 8];
const sum = numbers.reduce((accumulator, currentNumber) => accumulator + currentNumber, 0);

console.log(sum); // Output: 20 (2 + 4 + 6 + 8)

```

9. sort() - it arranges the array in either ascending or descending order. It works best for string array only. Not for numbers array. 
```
const products = ['Milk', 'Coffee', 'Sugar', 'Honey', 'Apple', 'Carrot']
console.log(products.sort())
```

But in case of numbers
```
const num = [40, 100, 50, 99]
console.log(num.sort()) // Output:[ 100, 40, 50, 99 ]
```