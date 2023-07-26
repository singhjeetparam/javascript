# JSON - JAVASCRIPT OBJECT NOTATION 
JSON is mostly used when data is sent from a server to a client. 

```
{
    "Alex": {
        "email": "alex@alex.com",
        "skills": [
            "HTML",
            "CSS",
            "JavaScript"
        ],
        "age": 20,
        "isLoggedIn": false,
        "points": 30
    },
    "Asab": {
        "email": "asab@asab.com",
        "skills": [
            "HTML",
            "CSS",
            "JavaScript",
            "Redux",
            "MongoDB",
            "Express",
            "React",
            "Node"
        ],
        "age": 25,
        "isLoggedIn": false,
        "points": 50
    },
    "Brook": {
        "email": "daniel@daniel.com",
        "skills": [
            "HTML",
            "CSS",
            "JavaScript",
            "React",
            "Redux"
        ],
        "age": 30,
        "isLoggedIn": true,
        "points": 50
    },
    "Daniel": {
        "email": "daniel@alex.com",
        "skills": [
            "HTML",
            "CSS",
            "JavaScript",
            "Python"
        ],
        "age": 20,
        "isLoggedIn": false,
        "points": 40
    },
    "John": {
        "email": "john@john.com",
        "skills": [
            "HTML",
            "CSS",
            "JavaScript",
            "React",
            "Redux",
            "Node.js"
        ],
        "age": 20,
        "isLoggedIn": true,
        "points": 50
    },
    "Thomas": {
        "email": "thomas@thomas.com",
        "skills": [
            "HTML",
            "CSS",
            "JavaScript",
            "React"
        ],
        "age": 20,
        "isLoggedIn": false,
        "points": 40
    },
    "Paul": {
        "email": "paul@paul.com",
        "skills": [
            "HTML",
            "CSS",
            "JavaScript",
            "MongoDB",
            "Express",
            "React",
            "Node"
        ],
        "age": 20,
        "isLoggedIn": false,
        "points": 40
    }
}
```

## CONVERTING JSON TO JAVACRIPT OBJECT 
We can fetch JSON data from HTTP response or from a file. It is stored as a JSON String we can't use this string directly. So we have to covert this into json object. We have a json parse function for this. 

```
const jsonString = '{"name": "John Doe", "age": 30, "email": "john@example.com"}';
const jsonObject = JSON.parse(jsonString);
```

use case of conversion of json to js objects - data retrival. when we receive data from an api. it is often in the form of json string. to work with it we need to convert it to json object.  

## CONVERTING OBJECT TO JSON 
We have a stringify method to do so. 
```
const person = {
  name: "John Doe",
  age: 30,
  email: "john@example.com"
};

const jsonString = JSON.stringify(person);
console.log(jsonString);
```

Use case of conversion of object to json - local storage. we can't save data in the format of object in local storage we need to convert this object into strings to do so. 


