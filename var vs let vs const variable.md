# Difference between var, let and const variable?

<table><tbody><tr><td><strong>var</strong></td><td><strong>let</strong></td><td><strong>const</strong></td></tr><tr><td>The scope of a <i>var </i>variable is functional scope.</td><td>The scope of a<i> let</i> variable is block scope.</td><td>The scope of a <i>const</i> variable is block scope.</td></tr><tr><td>It can be updated and re-declared into the scope.</td><td>It can be updated but cannot be re-declared into the scope.</td><td>It cannot be updated or re-declared into the scope.</td></tr><tr><td>It can be declared without initialization.</td><td>It can be declared without initialization.</td><td>It cannot be declared without initialization.</td></tr><tr><td>It can be accessed without initialization as its default value is “undefined”.</td><td>It cannot be accessed without initialization otherwise it will give ‘referenceError’.</td><td>It cannot be accessed without initialization, as it cannot be declared without initialization.</td></tr><tr><td>hoisting done , with initializing as ‘default’ value</td><td>Hoisting is done , but not initialized (this is the reason for error when we access the let variable before declaration/initialization</td><td>Hoisting is done, but not initialized (this is the reason for error when we access the const variable before declaration/initialization</td></tr></tbody></table>

### Example: 1. var, let and const variable Example:**
<pre>
if(true)
{
    var varVariable = 'The var variable is true';
}
console.log(varVariable);
if(true)
{
    let letVariable = 'The let variable is ture';
}
console.log(letVariable);
</pre>
<pre>
if(true)
{
    var varVariable = 'The var variable is true';
}
console.log(varVariable);

if(true){
    const constVariable = 'The const variable is true';
}
console.log(constVariable);

</pre>

**browser console var and let variable**
![image](https://user-images.githubusercontent.com/53125546/189515482-efaa760f-62c1-4882-867a-4fb7e8de001a.png)

**browser console var and const variable**
![image](https://user-images.githubusercontent.com/53125546/189515569-23c0b0aa-4ea2-4514-9d7c-d8152ee81dd4.png)


### Example 2
<pre>
   console.log(varVariableValue);
    var varVariableValue = 'md somrat akbor with var variable';
    console.log(letVariableValue);
    let letVariableValue='md somrat akbor with let variable';
</pre>



