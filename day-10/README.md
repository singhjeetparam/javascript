# SETS AND MAPS

## SET
Set is an collection of elements. Set can only contains unique elements. It automatically removes duplicate elements. 

### CREATING AN EMPTY SET 
```
const companies = new Set();
console.log(companies);
```

### CREATING SETS FROM AN ARRAY 

```
const languages = [
  'English',
  'Finnish',
  'English',
  'French',
  'Spanish',
  'English',
  'French',
]

const setOfLanguages = new Set(languages)
console.log(setOfLanguages)
```

### ITERATING IN SET 
```
const languages = [
  'English',
  'Finnish',
  'English',
  'French',
  'Spanish',
  'English',
  'French',
]

const setOfLanguages = new Set(languages)

for (const language of setOfLanguages) {
  console.log(language)
}
```

### ADDING AN ELEMENT TO A SET 
```
const companies = new Set() // creating an empty set
console.log(companies.size) // 0

companies.add('Google') // add element to the set
companies.add('Facebook')
companies.add('Amazon')
companies.add('Oracle')
companies.add('Microsoft')
console.log(companies.size) // 5 elements in the set
console.log(companies)
```

### DELETING AN ELEMENT TO A SET 
```
const mySet = new Set(['apple', 'banana', 'orange']);

console.log(mySet);     // Set(3) { 'apple', 'banana', 'orange' }

mySet.delete('apple');

console.log(mySet);     // Set(2) { 'banana', 'orange' }
```

### CHECKING AN ELEMENT IN A SET 
```
const mySet = new Set(['apple', 'banana', 'orange']);
console.log(mySet.has('apple'));    //true
console.log(mySet.has('Apple'));    //false

```


### CLEARING THE SET 
It removes all elements from a set.

```
const mySet = new Set(['apple', 'banana', 'orange']);
console.log(mySet);     // Set(3) { 'apple', 'banana', 'orange' }
mySet.clear();
console.log(mySet);     // Set(0) {}
```


### UNION OF SET 
To find the union of two sets. It can be acheived using the spread operator. 

```
let a = new Set([1,2,3,4,5]);
let b = new Set([4,5,6,7,8,9]);
let c = new Set([...a, ...b]);
console.log(c);
```

### INTERSECTION OF SET
It can be done using filters. 
```
let a = [1,2,3,4,5];
let b = [4,5,6,7,8,9];

let A = new Set(a);
let B = new Set(b);

let c = a.filter((num) => B.has(num));

let mySet = new Set(c);

console.log(mySet);

```

### DIFFERENCES OF SET
It will be same as the intesection, but we will change the has with !has. Ultimately the opposite of intersection will be difference. 

```
let a = [1,2,3,4,5];
let b = [4,5,6,7,8,9];

let A = new Set(a);
let B = new Set(b);

let c = a.filter((num) => !B.has(num));

let mySet = new Set(c);

console.log(mySet);
```

## MAPS
Map allows us to store ket-value pairs, where each key is unique. 

### CREATING A MAP 
```
const map = new Map();
console.log(map)
```

### CREATING A MAP FROM AN ARRAY 
```
const num = [[1,2],[3,4],[5,6],[7,8]];
const map = new Map(num);
console.log(map);
```
OR we can directly create an array with Map method

```
const map = new Map([[1,2],[3,4],[5,6],[7,8]]);
console.log(map);
```

### ADDING VALUES TO MAP 
```
const map = new Map();
console.log(map); // Map(0) {size: 0}
map.set(1,2);
map.set(3,4);
console.log(map); // Map(2) {1 => 2, 3 => 4}
```
### GETTING VALUE FROM MAP 
```
const map = new Map();
console.log(map);
map.set(1,2);
map.set(3,4);
console.log(map);
console.log(map.get(1)); // 2
```

### CHECKING KEY IN A MAP
```
const map = new Map([[1,2],[3,4],[5,6],[7,8]]);
console.log(map.has(1));
```

### GETTING ALL VALUES FROM MAP USING LOOP 
```
const map = new Map([[1,2],[3,4],[5,6],[7,8]]);
for(const [key,value] of map){
    console.log(key, value)
}
```