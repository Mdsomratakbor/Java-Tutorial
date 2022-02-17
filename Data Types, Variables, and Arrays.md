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

**Instance Variables:**
`A variable which is declared inside a class, but is declared outside any methods and blocks is known as instance variable.`
**Scope:** `Throughout the class except in the static methods.`
**Lifetime:** `Until the object of the class stays in the memory.`

***Class Variables:***
`A variable which is declared inside a class, outside all the blocks and is declared as static is known as class variable.`
**Scope:** `Throughout the class.`
**Lifetime:** `Until the end of the program.`

***Local Variables:***
`All variables which are not instance or class variables are known as local variables.`
**Scope:** `Within the block it is declared.`
**Lifetime:** `Until control leaves the block in which it is declared.
Now, let us look at an example code to paint a clear picture and understand the concept of scope and lifetime of variables better.`

**Example:**
<pre>public class scope_and_lifetime {
    int num1, num2;   //Instance Variables
    static int result;  //Class Variable
    int add(int a, int b){  //Local Variables
        num1 = a;
        num2 = b;
        return a+b;
    }
    public static void main(String args[]){
        scope_and_lifetime ob = new scope_and_lifetime();
        result = ob.add(10, 20);
        System.out.println("Sum = " + result);
    }
}</pre>

### 5. What is Type conversion in Java?
`The process of converting a value from one data type to another is known as type conversion in Java.`

`Widening conversion takes place when two data types are automatically converted. This happens when:`</br>
-**The two data types are compatible.**</br>
-**When we assign a value of a smaller data type to a bigger data type.**</br>

**Example:**
<pre>
class ConvertionVariable {
    // Main driver method
    public static void main(String[] args)
    {
        int i = 100; 
        // Automatic type conversion
        // Integer to long type
        long l = i;
        // Automatic type conversion
        // long to float type
        float f = l;
        // Print and display commands
        System.out.println("Int value " + i);
        System.out.println("Long value " + l);
        System.out.println("Float value " + f);
    }
}
</pre>

### 6. What is Type Casting in Java?
`In typing casting, a data type is converted into another data type by the programmer using the casting operator during the program design. In typing casting, the destination data type may be smaller than the source data type when converting the data type to another data type, that’s why it is also called narrowing conversion.`

**Example :**
<pre>
float x;
byte y;
y=(byte)x; 
</pre>


### 7. Types of Casting in Java?

`There are two types of type casting:`

- **Widening Type Casting/implicit conversion or casting down.**
- **Narrowing Type Casting/explicit conversion or casting up.**

**Widening Type Casting:**`Converting a lower data type into a higher one is called widening type casting. It is also known as implicit conversion or casting down. It is done automatically. It is safe because there is no chance to lose data. It takes place when:`

- `Both data types must be compatible with each other.`
- `The target type must be larger than the source type.`

**Example :**
<pre>
public class WideningTypeCastingExample  
{  
public static void main(String[] args)  
{  
int x = 7;  
//automatically converts the integer type into long type  
long y = x;  
//automatically converts the long type into float type  
float z = y;  
System.out.println("Before conversion, int value "+x);  
System.out.println("After conversion, long value "+y);  
System.out.println("After conversion, float value "+z);  
}  
} 
</pre>
![image](https://user-images.githubusercontent.com/53125546/154499123-9e8d3d98-89d6-4aba-bcf5-2ced3daae86f.png)

**Narrowing Type Casting :**`Converting a higher data type into a lower one is called narrowing type casting. It is also known as explicit conversion or casting up. It is done manually by the programmer. If we do not perform casting then the compiler reports a compile-time error.`

**Example:**
<pre>
public class NarrowingTypeCastingExample  
{  
public static void main(String args[])  
{  
double d = 166.66;  
//converting double data type into long data type  
long l = (long)d;  
//converting long data type into int data type  
int i = (int)l;  
System.out.println("Before conversion: "+d);  
//fractional part lost  
System.out.println("After conversion into long type: "+l);  
//fractional part lost  
System.out.println("After conversion into int type: "+i);  
}  
} 
</pre>
![image](https://user-images.githubusercontent.com/53125546/154499290-9fe7496e-e8a6-49a1-8b84-7429012ef6c1.png)
