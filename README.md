# JS_Tutorials_Notes

### Variable Scope
https://dev.to/sandy8111112004/javascript-introduction-to-scope-function-scope-block-scope-d11

### Difference between var, let, const
https://dev.to/sandy8111112004/javascript-var-let-const-41he

### Prevent Object Mutation: 
The problem is object decalred as a const can be changed using correspondng index. for example: 
```
const s = [2, 10 ,5];
s[1] = 10;// alowed, how to prevent it?
s = [1, 2, 3]; //error
Object.freeze(s);// will prevent any kind of data mutation.

```

### Set default parameter
It's fairly easy to add a default parameter.
An interesting thing is, if you want to use the default value of first parameter you have to do the following.
```
// Only change code below this line
const increment = (number = 1, value) => number + value;
// Only change code above this line
console.log(increment(undefined,2))

```
### Rest operator
```
const a = (...args) => return args.lenth();
a(null, "aass", [1,2,3,4]) //

```

### Spread operator for unpacking an array
```
const arr = [6, 89, 3, 45];
const maximus = Math.max(...arr);//max expects comma/spaced seperated agruments, spread operator does make spaced seperated values
```

### Destructuring Assignment : Used to Extract Values from Objects
```
const user = { name: 'John Doe', age: 34 };
const { name, age } = user;//destructures the values in the variable name and age
```
#### Here's how you can give new variable names in the assignment
```
const user = { name: 'John Doe', age: 34 };
const { name: userName, age: userAge } = user;
```
