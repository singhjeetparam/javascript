# WEB STORAGES 
Before HTML 5, we store data using cookies. But in HTML 5 we have to option to store data in web storages. We can store large amount of data than the
cookies. at least 5mb of data can be stored in web storages. 


We have two types of web storage objects.
1. Local Storage
2. Session Storage 


## LOCAL STORAGE
In this data is stored with no expiration date. It is stored in key-value pairs. The data remains even after the browser closes and it remains for future sessions too. It is stored for a specific domain, port so it can be only accessed by these specific domains or ports only. 

```
// Storing data in localStorage
localStorage.setItem('name', 'John Doe');
localStorage.setItem('age', '30');

// Retrieving data from localStorage
const name = localStorage.getItem('name');
const age = localStorage.getItem('age');

console.log(name); // Output: "John Doe"
console.log(age); // Output: "30"

```

### SETTING DATA TO LOCAL STORAGE 
```
localStorage.setItem('key', 'value');
```

### GETTING DATA FROM LOCAL STORAGE
```
localStorage.getItem('key');
```

### CLEARING LOCAL STORAGE 
```
localStorage.clear();
```

## SESSION STORAGE 
It is similar to local storage. But the data remains for only a single session. It remains only till the browser remains open. 
```
// Storing data in sessionStorage
sessionStorage.setItem('token', 'abc123');
sessionStorage.setItem('isLoggedIn', 'true');

// Retrieving data from sessionStorage
const token = sessionStorage.getItem('token');
const isLoggedIn = sessionStorage.getItem('isLoggedIn');

console.log(token); // Output: "abc123"
console.log(isLoggedIn); // Output: "true"

```


## USE CASE OF WEB STORAGE 
- to store data temporarily 
- used in ecommerce to keep cart items
- used for authentication method 
