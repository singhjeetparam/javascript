# REGULAR EXRPRESSION
It helps to find patterns in data. It is used to check if some pattern is presentin the data or not.

## REGEXP PARAMETER
 A regular expression takes two parameter. One required search pattern and an optional fleg. 

## FLAGS
1. g - a global flag which means looking for a pattern in whole text. 
2. i - case insensitive flag. It looks for both lowercase and uppercase. 
3. m - multiline 

## CREATING A PATTERN WITH REGEXP CONSTRUCTOR
```
let pattern  = 'love'
let regEx = new RegExp(patter)
```
## CREATING A PATTERN WITH PATTERN AND FLAG
```
let patter = 'love';
let flag = 'g';
let regEx = new RegExp(pattern, flag);
```

## WRITING THE PATTERN AND FLAG INSIDE THE REGEXP CONSTRUCTOR
```
let regEx = new RegExp('love', 'g');
```

## CREATING A REGEXP WITHOUT REGEXP CONSTRUCTOR
```
let regEx = /love/gi
```

BAAKI SEARCH FOR IT EVERYTIME ON INTERNET
