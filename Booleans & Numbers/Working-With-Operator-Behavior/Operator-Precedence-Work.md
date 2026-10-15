# Operator Precedence Work 
 Operator precedence determines the order in which operations are evaluated in an expression. 

 Think about if you were to write an expression with several operators in JS, how do you think JS will decide which operator to do first? This is where Operator precedence comes into play. 

 Operators with higher precedence are evaluated before those with lower precedence! 
- Think of it like math
    - division and multiplation happen before addition and subtraction 
    - JS has its own rules for which operators come first, second, etc etc 
    - follow this rule so you dont get the wrong answers 

## Precednece In Arithmetic Expressions

```javascript 
// Multiplication Precedence
const result = 2 + 3 * 4;
console.log(result); // 14 

// multiplication held a higher precedence, JS started with that operator.
```


```javascript
// Division Precedence 
const result = 2 + 6 / 3;
console.log(result); // 4
// division is the highest precedence here. 
```


```javascript
// Parentheses to Override Precendence
const result = (2 + 3) * 4;
console.log(result); // 20
// Note: to override precedence, using the parentheses will run first, regarless of precedence rules. Anything inside the parentheses will be evaluated first, no matter what. 
```


## Understanding Associativity
Associativity is what tells JavaScript whether to evaluate operators from left > right or right > left

For most operators, like addition and multiplication, associativity goes from left to right 
```javascript
const result = 10 - 2 +3;
console.log(result); // 11
// this goes from the leftmost side of the expression
```


For (=) operators, they're right > left asociative, which means the right side gets evaluated first
```javascript
// = Operator
let a, b;
a = b = 5;

console.log(a); // 5
console.log(b); // 5
console.log(a + b); // 10
// going from right to left, right side get evualted first
```


Exponent Operator 
This operator is also right to left associative 
```javascript
const result = 2 ** 3 ** 2;
console.log(result); // 512
// going from right to left with this operator, 2 would be the exponent, then 3^2 = 9, then 2^9 = 512
```