# ERROR HANDLING

Sometimes we can get error when we try to access an undefined variables or call undefined function etc.

```
try{
//code that may throw error
}
catch(err){
code to be executed if an error occurs
}
finally{
//code to be executed regardless of an error occurs or not
}
```

## TRY

code that may throw error

## CATCH

code to be executed if an error occurs

## FINALLY

code to be executed regardless of an error occurs or not

```
try{
    let lastName = "Singh";
    let fullName = firstName + lastName;
}
catch(err){
    console.log(err);
}
finally{
    console.log("In any case I will be executed");
}
```

## THROW
It allows is to create a custom error. 

```
const throwErrorExample = () =>{
    let message; 
    let x = prompt('Enter a Number');
    try{
        if(x=='') throw 'empty';
        if(isNaN(x)) throw 'not a number';
        x = Number(x);
        if(x<5) throw 'Number too low';
        if(x>10) throw 'Number too high';
    }
    catch(err){
        console.log(err);
    }
}
throwErrorExample();
```


## TYPES OF ERRORS IN JAVASCRIPT
### 1. Reference Error
When we use a variable that is not declared. 
```
let name = "param";
console.log(lastName);
```

### 2. Syntax Error
When we use wrong syntax

```
let square = 2 X 2;
console.log(square);
```

### 3. Type Error
when a typo error occurs.
```
let num = 10; 
console.log(num.toLowerCase());
```
