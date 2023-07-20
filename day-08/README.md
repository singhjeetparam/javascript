# OBJECTS 
Anything can be an object and objects do have properties and proerties have values. SO object is a kely value pair. 

## CREATING AN EMPTY OBJECT
```
const person = {}
```

## CREATING AN OBJECT WITH VALUES 

```
const person = {
firstName: "Paramjeet",
lastName: "Singh",
age: 22,
isMarried: false
};

console.log(person)
```

## GETTING VALUES FROM AN OBJECT
We can access values of object in two ways. 

1. using period. followed by keyname 
2. using square bracket and a quote


### Using period
```
const person = {
firstName: "Paramjeet",
lastName: "Singh",
age: 22,
isMarried: false
};

console.log(person.firstName);
```

### Using square bracket 
```
const person = {
firstName: "Paramjeet",
lastName: "Singh",
age: 22,
isMarried: false
};

console.log(person['firstName'])
```

## CREATING OBJECT METHODS
Functions associated with objects are called object methods. 

```
const person = {
firstName: 'Asabeneh',
lastName: 'Yetayeh',
age: 250,
country: 'Finland',
city: 'Helsinki',
skills: [
'HTML',
'CSS',
'JavaScript',
'React',
'Node',
'MongoDB',
'Python',
'D3.js'
],
getFullName: function() {
return `${this.firstName} ${this.lastName}`
}
}

console.log(person.getFullName())
// Asabeneh Yetayeh
```

Now here getFullName is a method. And this keyword inside it refers to the current object in which the method is. 


## SETTING NEW KEYS FOR AN OBJECT 
An object is mutable data structure. We can change the data of it even after its creation. 

```
const person = {
firstName: 'Paramjeet',
lastName: 'Singh',
age: 20
}

person.nationality = 'Indian'

console.log(person);
```


## OBJECT METHODS 
They are used to manipulate an object. 

1. object.assin - to copy an object without modifying the original object. 

```
const person = {
firstName: 'Paramjeet',
lastName: 'Singh',
age: 20
}

person.nationality = 'Indian'


const anotherPerson = Object.assign({}, person);

console.log(anotherPerson);

```

2. object.keys - to get the keys or properties of an object as an array 
```
const person = {
firstName: 'Paramjeet',
lastName: 'Singh',
age: 20
}

person.nationality = 'Indian'


const keys = Object.keys(person)

console.log(keys)

```

3. object.values - to get the values of an object in an array 
```
const person = {
firstName: 'Paramjeet',
lastName: 'Singh',
age: 20
}

person.nationality = 'Indian'


const keys = Object.values(person)

console.log(keys)

```

4. object.entries - to get both keys and values in an array 
```
const person = {
firstName: 'Paramjeet',
lastName: 'Singh',
age: 20
}

person.nationality = 'Indian'


const keys = Object.entries(person)

console.log(keys)

```
5. hasOwnProperty() -  It is used to check whether an object has a property with a specific name and returns a boolean value indicating the result. 

```
const myObject = {
  property1: 'value1',
  property2: 'value2'
};

console.log(myObject.hasOwnProperty('property1')); // Output: true
console.log(myObject.hasOwnProperty('property2')); // Output: true
console.log(myObject.hasOwnProperty('property3')); // Output: false

```