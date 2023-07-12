# ARRAYS
It is used to store multiple values. Each value in an array has an index, each index has a reference in a memory address
Each value can be accessed using these indexes. 

An array can be empty and mutuable(we can change it's data after creation). We can also store duplicate data to it. 

## HOW TO CREATE AN ARRAY 
1. Using array Constructor 
```
const arr = Array();
```

2. Using square bracket[] 
```
const arr = []
```

## HOW TO CREATE AN ARRAY WITH VALUES 
```
const arr = [1,2,3,4,5];
```

An array can have different types of data types in it 

Example - 
```
const arr = [1, "one", true, {name: "param"}]
```

## CREATING AN ARRAY USING SPLIT
We can use split method in a string to make array out of it. 

```
let name = "paramjeet sing";
let arr = name.split("");
```

## ACCESSING ELEMENT USING INDEX 
We can access elements of an array using index values. 

```
let arr = [1,2,3];
console.log(arr[0], arr[1], arr[2]);
```

## LENGTH OF AN ARRAY 
we can find the length of an array using length method. 

```
let arr = [1,2,3];
console.log(arr.length)
```


## MODIFYING AN ARRAY 

we can modify the elements of an array too even after the creation of it. 

```
let arr = [1,2,3];
arr[1] = 4;

console.log(arr)
```


## METHODS TO MANIPULATE AN ARRAY 

1. Array constructor  - we can use this to create an array even with predefined sizes. 

```
let arr = Array(8);
console.log(arr.length);
```

2. Creating static values with fill - using this we can fill an array with static values 

```
let arr = Array(8).fill("x");
console.log(arr)
```


3. Concatenating an array - we can use concat() to concatenate two arrays 

```
let first = [1,2,3];
let second = [4,5,6];
let third = first.concat(second);
console.log(third);
```

4. Checking index of an element  in array 

```
let arr = [1,2,3];
console.log(arr.indexOf(1))
```

5. Getting last index of an element

```
let arr = [1,2,3,1];
console.log(arr.lastIndexOf(1));
```

6. Checking whether an element exist in an array or not. 
```
let arr = [1,2,3];
console.log(arr.includes(1));
```

7. Converting Array to String 

```
let arr = [1,2,3];
let arrString= arr.toString();
console.log(arrString);
```

8. Joining array elements- we can join any particular argument that we pass in this method to all element of an array. It also converts the array into string.

```
let arr =  [1,2,3];
console.log(arr.join("#"))
```

9. Slicing of elements - to cut out mulitple items in a range. It takes two parameters starting position and ending position. It doesn't include the ending position. 

```
let arr = [1,2,3,4,5];
console.log(arr.slice(1,3));
```

10. Splicing of element - It takes three parameters, starting index, number of elements to be removed and number of elements to be added. 

```
let arr = [1,2,3,4,5,6];
arr.splice(2,2,10,11);
console.log(arr);
```

11. Adding an element to an array - this adds an element to the end of an array 
```
let arr = [1,2,3];
arr.push(4);
console.log(arr);
```

12. Removing an element to an array - this removes the last element of the array. It always remove the last element of the array.
```
let arr = [1,2,3];
arr.pop();
console.log(arr)
```

13. Removing an element from the beginning - shift()
```
let arr = [1,2,3,4];
arr.shift();
console.log(arr);
```

14. Adding an element to the beginning - unshift()
```
let arr = [1,2,3];
arr.unshift(10);
console.log(arr);
```

15. Reversing an array - reverse() is used to reverse an array 
```
let arr = [1,2,3];
arr.reverse();
console.log(arr);
```

16. sorting an element - sort() 
```
const webTechs = [
  'HTML',
  'CSS',
  'JavaScript',
  'React',
  'Redux',
  'Node',
  'MongoDB'
]

webTechs.sort()
console.log(webTechs) // ["CSS", "HTML", "JavaScript", "MongoDB", "Node", "React", "Redux"]
```

But it only works well for string array. In case of numerical array it can produce false results because it compares the very first character only. Check the following example 

```
let arr = [1,4,9,11,0];
arr.sort();
console.log(arr);
```

## ARRAY OF ARRAYS
We can have array of arrays 
```
let arr = [[1,2,3], [4,5,6], [7,8,9]];
console.log(arr);
```

