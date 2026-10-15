# Increment and Decrement Operators at Work
If you need to increase or decrease a value by one, the increment and decrement operators makes the process much easier (in a simple way). 
- These operators are presented by ++ and --
- Allowing you to adjust by 1


## To Add and Subtract
- Add = x++
- To subtract = x--


## Pre and Postfix
But there is a twist on this, the pre and postfix, coming in 2 forms 
- The difference being when the value gets updated
    - prefix = ++x
    - postfix = x++

Prefix (++x) - increases the value of the variable first, then returns the new value 
For example
```javascript
let x = 5
console.log(++x); // 6
console.log(x); // 6
// the prefix increases by 1 then gives you the value
```

Postfix (x++) - returns the current value of the variable first, then increases it 
```javascript 
let y = 5; 
console.log(y++); // 5
console.log(y); // 6
//In this example, y++ means "use y first, then increment it". When you log y++, you get 5, but y becomes 6 after that line of code


