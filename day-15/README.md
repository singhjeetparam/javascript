# CLASSES
Javascript is an OOP Langugage. Everything in JS is an object, with its properties and methods. 

A class is like a an object constructor, or a blueprint for creating objects. We instantiate a class to create an object. The class defines the
attributes and teh behaviour of the object. While the object represents the class. 

Once  we create a class we can create object from it whenever we want.  Creating an object from a class is called class instantiation

## DEFINING A CLASS
```
class ClassName{

}
```

example 
```
class Person{

}
```

## CLASS INSTANTIATION
It means creating an object from a class. 

```
class Person{

}

const person = new Person();
console.log(person);
```

Till now our class has no properties yet the object is empty. 

## CLASS CONSTRUCTOR
This is a built-in function which allows us to create blueprint for our object. It starts with a keyword "constructor" followed by paranthesis. Inside the paranthesis we pass the properties of the object as a parameter. We use "this" keyword to attach the constructor parameter with the class. 

```
class Persons{
    constructor(firstName, lastName){
        console.log(this);
        this.firstName = firstName;
        this.lastName = lastName;
    }
}

const person = new Person();
console.log(person)
```
Till now all the objects are undefined. Whenenver we instantiate we should pass the value of the properties. 

```
class Person{
    constructor(firstName, lastName){
        console.log(this);
        this.firstName = firstName;
        this.lastName = lastName; 
    }
}

const person = new Person("Paramjeet", "Singh");

console.log(person);
```

We have stated in the beginning that  we create a class at once and we can create as many objects from it. 
```
class Person {
  constructor(firstName, lastName) {
    console.log(this) // Check the output from here
    this.firstName = firstName
    this.lastName = lastName
  }
}

const person1 = new Person('Asabeneh', 'Yetayeh')
const person2 = new Person('Lidiya', 'Tekle')
const person3 = new Person('Abraham', 'Yetayeh')

console.log(person1)
console.log(person2)
console.log(person3)
```

## DEFAULT VALUES WITH CONSTRUCTOR
We can add default values to constructor also. 

```
class Person{
    constructor(
        firstName = "Paramjeet",
        lastName = "Singh"
    ){
        this.firstName = firstName;
        this.lastName = lastName;
    }
}

const person = new Person();    // this will give us default values of constructor
const anotherPerson = new Person("Dummy First Name", "Dummy Last Name");     // this will give us the values that we have passed in it
```


## CLASS METHODS
They are JS functions inside a class

```
class Person{
    constructor(firstName, lastName){
        this.firstName =firstName;
        this.lastName = lastName;
    }
    getFullName(){
        const fullName = this.firstName + " " + this.lastName;
        return fullName;
    }
}

const person = new Person("paramjeet" , "singh");

console.log(person.getFullName());
```

## PROPERTIES WITH INITIAL VALUES
We can have some properties with initial values that may change later. Like score or skills. 

```
class Person{
    constructor(firstName, lastName, score, skill){
        this.firstName = firstName;
        this.lastName = lastName;
        this.score = 0; 
        this.skill = [];
    }
}

const person = new Person("paramjeet", "singh");

console.log(person.skill);
console.log(person.score);
```

## GETTER METHOD
It is used to access values from the objects. 
```
class Person{
    constructor(firstName, lastName, score, skill){
        this.firstName = firstName;
        this.lastName = lastName; 
        this.score = score; 
        this.skill = skill;
    }

    get getScore(){
        return this.score;
    }

    get getSkill(){
        return this.skill;
    }
}

const person = new Person("paramjeet", "singh", 10, ["html", "css", "js"]);

console.log(person.getScore); // there is no need to use paranthesis in get method

console.log(person.getSkill());     // there is no need to use paranthesis in get method
```

## SETTER METHOD
This method allows us to modify values of certain properties. We use set keyword to do so. 

```
class Person{
    constructor(firstName, lastName, score){
        this.firstName = firstName;
        this.lastName = lastName; 
        this.score = score; 
    }

    set setScore(score){
        this.score += score;
    }
}

const person = new Person("Paramjeet", "Singh", 20);

person.setScore = 1;

console.log(person.score)
```