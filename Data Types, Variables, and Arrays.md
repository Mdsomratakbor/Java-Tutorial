### 1. Why is Java a platform independent language?
`Java language was developed in such a way that it does not depend on any hardware or software due to the fact that the compiler compiles the code and then converts it to platform-independent byte code which can be run on multiple systems.`

 - The only condition to run that byte code is for the machine to have a runtime environment (JRE) installed in it.
### 2. How many data types in Java?
**There are two types of data type in java**

- **1. Primitive data types:** `The primitive data types include boolean, char, byte, short, int, long, float and double`.
- **2. Non-primitive data types:** `The non-primitive data types include Classes, Interfaces, and Arrays.`

   ![java-data-types](https://user-images.githubusercontent.com/53125546/154004892-b68cc95f-40e7-4126-b487-4fb83ce1d9c4.png)
### 3. What is Scope and Lifetime of Variables in Java?

- Java allows variables to be declared within any block.
- A block is begun with an opening curly bracket and ended by a closing curly bracket. A block defines a scope.
- A scope determines what objects are visible to other parts of your program. 
- It also determines the lifetime of those objects.
- Scopes can be nested.
- Variables are created when their scope is entered, and destroyed when their scope is left.
- The lifetime of a variable is confined to its scope.
### 4. Types of Variables and its Scope in Java?
`There are three types of variables.`

- **1. Instance Variables**
- **2. Class Variables**
- **3. Local Variables**

**Instance Variables**
`A variable which is declared inside a class, but is declared outside any methods and blocks is known as instance variable.`
**Scope:** `Throughout the class except in the static methods.`
**Lifetime:** `Until the object of the class stays in the memory.`

***Class Variables***
`A variable which is declared inside a class, outside all the blocks and is declared as static is known as class variable.`
**Scope:** `Throughout the class.`
**Lifetime:** `Until the end of the program.`

***Local Variables***
`All variables which are not instance or class variables are known as local variables.`
**Scope:** `Within the block it is declared.`
**Lifetime:** `Until control leaves the block in which it is declared.
Now, let us look at an example code to paint a clear picture and understand the concept of scope and lifetime of variables better.`
