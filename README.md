# JS_Tutorials_Notes

## Variable Scope : https://dev.to/sandy8111112004/javascript-introduction-to-scope-function-scope-block-scope-d11

## Difference between var, let, const: https://dev.to/sandy8111112004/javascript-var-let-const-41he

## Prevent Object Mutation: The problem is object decalred as a const can be changed using correspondng index. for example: 
```
const s = [2, 10 ,5];<br /> 
s[1] = 10;// alowed, how to prevent it? <br /> 
s = [1, 2, 3]; //error <br /> 

Object.freeze(s);// will prevent any kind of data mutation.
```

