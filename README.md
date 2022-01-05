# JS_Tutorials_Notes

## Tasks to Accomplish

1. Javascript Fundamentals - [John Smillga Youtube JS Fundamentals](https://youtu.be/2Ji-clqUYnA)
2. Advanced Topics
   1. OOP - [OOP in JS by MOSH](https://youtu.be/PFmuCDHHpwk), [JS Classes FreeCodeCamp](https://youtu.be/2ZphE5HcQPQ)
   2. Asynchronous JavaScript Course (Async/Await, Promises, Callbacks)- [Joy Shaheb FreeCodeCamp](https://youtu.be/ZYb_ZU8LNxs)
3. Practice Problems
4. Projects
5. Frameworks

## Environment Setup

1. Install VSCode or Any other IDE
2. Install a Browser
3. Install Live Server/ VS Code Preview Server and Prettier Extension
4. Use the settings.json files codes in your vscode settings.json file.

## Backend Things need to learn

As a backend Developer you should learn these things

1. how to connect backend app with database
2. developing rest apis
3. storing and retrieving data from database
4. authentication and authorization admin role
5. user tracking with cookies and sessions
6. error handling
7. secure communication
8. file uploads
9. cross origin resource sharing
10. data caching
11. socket programming

### Variable Scope

https://dev.to/sandy8111112004/javascript-introduction-to-scope-function-scope-block-scope-d11

### JavaScript Hoisting

All declarations (var, let, const, function, function\*, class) are "hoisted" in JavaScript. This means that if a name is declared in a scope, in that scope the identifier will always reference that particular variable. However incase of let, const the situation become little different if they are not initialized(with default value or user value) before the use. "var" is initialized with undefined by default, however let/const are not.

Example 1

```
var a;
console.log(a); //undefined

console.log(b); //undefined
var b;

let x;
console.log(x); //undefined

console.log(y); // Uncaught ReferenceError: y is not defined
let y;
```

The variable 'y' gives a referenceError, that doesn't mean it's not hoisted. The variable is created when the containing environment is instantiated. But it may not be accessed because of it being in an inaccessible "temporal dead zone".

Example 2

```
let mylet = 'my value';

(function() {
  //let mylet;//uncomment it to test
  console.log(mylet); // "my value"
  mylet = 'local value';
})();
```

In Example 2, Uncomment the first line of the function, the freshly declared "mylet" variable inside the function does not have an Initializer before the log statement, hence the value "undefined".

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

### Server and Client

DNS Server: Reside to data center of the ISP or collects from third party, from where ISP sends the corresponding IP of the domain name the user tryng to access. Once the browser gets the IP it starts is's conversion with the Web Server hosting the website.
![image](https://user-images.githubusercontent.com/24862973/119589673-190f4380-bdf5-11eb-91cb-0369db01c6eb.png)

![image](https://user-images.githubusercontent.com/24862973/119736896-3fd68400-bea0-11eb-96c0-58eadd7674e9.png)

https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server
![image](https://user-images.githubusercontent.com/24862973/119736567-b757e380-be9f-11eb-824d-56cd90c9db5f.png)
