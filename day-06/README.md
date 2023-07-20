# LOOPS

They are used to perform iterative operations

## FOR LOOP

```
// For loop structure
for(initialization, condition, increment/decrement){
// code goes here
}

for(let i = 0; i <= 5; i++){
console.log(i)
}

// 0 1 2 3 4 5


```

## WHILE LOOP

```
let i = 0
while (i <= 5) {
console.log(i)
i++
}

// 0 1 2 3 4 5
```


## DO WHILE LOOP 
```
let i = 0
do {
  console.log(i)
  i++
} while (i <= 5)

// 0 1 2 3 4 5
```

## FOR OF LOOP 
This is the very handy way to iterate over only an array, if the index if not our concern. 

```
for (const element of arr) {
  // code goes here
}
```

## BREAK 
It is used to interrrupt a loop. Like if we want to end the loop on a particular condition

```
for(let i = 0; i<10; i++){
    if(i==3){
        break;
    }
    console.log(i);
}

// 0 1 2 
```

## CONTINUE
When we want to skip a particular iteration 
```
for(let i = 0; i<10; i++){
    if(i==3){
        continue;
    }
    console.log(i);
}

//0 1 2 4 5 6 7 8 9 10
```