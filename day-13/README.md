# CONSOLE METHOD
It is used to get output on the browser console. 

## CONSOLE.LOG
```
console.log("Hello");
```

we can also add css to it

```
console.log('%c30 Days Of JavaScript', 'color:green') // log output is green
console.log(
  '%c30 Days%c %cOf%c %cJavaScript%c',
  'color:green',
  '',
  'color:red',
  '',
  'color:yellow'
) // log output green red and yellow text
```

## CONSOLE.WARN 
It shows warning on browser. 
```
console.warn('This is a warning')
console.warn(
  'You are using React. Do not touch the DOM. Virtual DOM will take care of handling the DOM!'
)
console.warn('Warning is different from error')
```


## CONSOLE.ERROR
It shows an error message.
```
console.error('This is an error message')
console.error('We all make mistakes')
```

## CONSOLE.TABLE
It display data in table format. 

```
const user = {
  name: 'Asabeneh',
  title: 'Programmer',
  country: 'Finland',
  city: 'Helsinki',
  age: 250
}
console.table(user)
```

## CONSOLE.TIME
It starts a timer so that we can track how long an operation takes.

```
const countries = [
  ['Finland', 'Helsinki'],
  ['Sweden', 'Stockholm'],
  ['Norway', 'Oslo']
]

console.time('Regular for loop')
for (let i = 0; i < countries.length; i++) {
  console.log(countries[i][0], countries[i][1])
}
console.timeEnd('Regular for loop')

console.time('for of loop')
for (const [name, city] of countries) {
  console.log(name, city)
}
console.timeEnd('for of loop')

console.time('forEach loop')
countries.forEach(([name, city]) => {
  console.log(name, city)
})
console.timeEnd('forEach loop')
```

## CONSOLE.INFO
It displays information message on browser. 
```
console.info("This is an information");
```

## CONSOLE.CLEAR
It clears the console.
```
console.clear()
```