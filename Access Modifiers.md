### What is Access Modifiers in Java?
`Access modifiers are object-oriented programming that is used to set the accessibility of classes, constructors, methods, and other members of Java.`
`Using the access modifiers we can set the scope or accessibility of these classes, methods, constructors, and other members.`

### How many Access Modifier have Java?

`Four Types of Access Modifiers:`
- **Private**
- **Default**
- **Protected**
- **Public**

**Private:** `We can access the private modifier only within the same class and not from outside the class.`

**Default:** `We can access the default modifier only within the same package and not from outside the package. And also, if we do not specify any access modifier it will automatically consider it as default.`

**Protected:** `We can access the protected modifier within the same package and also from outside the package with the help of the child class. If we do not make the child class, we cannot access it from outside the package. So inheritance is a must for accessing it from outside the package.`

**Public:** `We can access the public modifier from anywhere. We can access public modifiers from within the class as well as from outside the class and also within the package and outside the package.`

<table id="tablepress-1590" class="tablepress tablepress-id-1590 tablepress-responsive">
<thead>
<tr class="row-1 odd">
<th class="column-1">Access Specifier</th><th class="column-2">Inside Class</th><th class="column-3">Inside Package</th><th class="column-4">Outside package subclass</th><th class="column-5">Outside package</th>
</tr>
</thead>
<tbody class="row-hover">
<tr class="row-2 even">
<td class="column-1">Private</td><td class="column-2">Yes</td><td class="column-3">No</td><td class="column-4">No</td><td class="column-5">No</td>
</tr>
<tr class="row-3 odd">
<td class="column-1">Default</td><td class="column-2">Yes</td><td class="column-3">Yes</td><td class="column-4">No</td><td class="column-5">No</td>
</tr>
<tr class="row-4 even">
<td class="column-1">Protected</td><td class="column-2">Yes</td><td class="column-3">Yes</td><td class="column-4">Yes</td><td class="column-5">No</td>
</tr>
<tr class="row-5 odd">
<td class="column-1">Public</td><td class="column-2">Yes</td><td class="column-3">Yes</td><td class="column-4">Yes</td><td class="column-5">Yes</td>
</tr>
</tbody>
</table>


**Default Access Specifiers**
`A default access modifier in Java has no specific keyword. Whenever the access modifier is not specified, then it is assumed to be the default. The entities like classes, methods, and variables can have a default access.`

`A default class is accessible inside the package but it is not accessible from outside the package i.e. all the classes inside the package in which the default class is defined can access this class.`

`Similarly a default method or variable is also accessible inside the package in which they are defined and not outside the package.`

<pre>
class BaseClass 
{ 
    void display()      //no access modifier indicates default modifier
       { 
           System.out.println("BaseClass::Display with 'dafault' scope"); 
       } 
} 
 
class Main
{ 
    public static void main(String args[]) 
       {   
          //access class with default scope
          BaseClass obj = new BaseClass(); 
   
          obj.display();    //access class method with default scope
       } 
}
</pre>

**Output:Default Access Modifiers In Java**

`In the above program, we have a class and a method inside it without any access modifier. Hence both the class and method display has default access. Then we see that in the method, we can directly create an object of the class and call the method.`


**Public Access Modifier **
`A class or a method or a data field specified as ‘public’ is accessible from any class or package in the Java program. The public entity is accessible within the package as well as outside the package. In general, public access modifier is a modifier that does not restrict the entity at all.`

<pre>
class A 
{ 
   public void display() 
      { 
          System.out.println("SoftwareTestingHelp!!"); 
      } 
} 
class Main 
{ 
    public static void main(String args[]) 
      { 
          A obj = new A (); 
          obj.display(); 
      } 
}
</pre>

**Protected Access Specifier**
`The protected access specifier allows access to entities through subclasses of the class in which the entity is declared. It doesn’t matter whether the class is in the same package or different package, but as long as the class that is trying to access a protected entity is a subclass of this class, the entity is accessible.`

`Note that a class and an interface cannot be protected i.e. we cannot apply protected modifiers to classes and interfaces.`

`The protected access modifier is usually used in parent-child relationships.`


<pre>
class A 
{ 
   protected void display() 
    { 
        System.out.println("SoftwareTestingHelp"); 
    } 
} 
 
class B extends A {}  
class C extends B {}
 
class Main{
     public static void main(String args[]) 
   {   
       B obj = new B();     //create object of class B   
       obj.display();       //access class A protected method using obj
       C cObj = new C();    //create object of class C
       cObj.display ();     //access class A protected method using cObj
   }   
}
</pre>

**Private Access Modifier** 
`The ‘private’ access modifier is the one that has the lowest accessibility level. The methods and fields that are declared as private are not accessible outside the class. They are accessible only within the class which has these private entities as its members.`

`Note that the private entities are not even visible to the subclasses of the class. A private access modifier ensures encapsulation in Java.`

Some points to be noted regarding the Private Access Modifier.

`Private access modifier cannot be used for classes and interfaces`.
- `The scope of private entities (methods and variables) is limited to the class in which they are declared.`
- `A class with a private constructor cannot create an object of the class from any other place like the main method. (More details on private constructors has been explained in our earlier tutorial).`

<pre>
class DataClass {
    private String strname;    
 
// getter method
    public String getName() {
        return this.strname;
    }
    // setter method
    public void setName(String name) {
        this.strname= name;
    }
}
public class Main {
    public static void main(String[] main){
        DataClass d = new DataClass();       
 
 // access the private variable using the getter and setter
        d.setName("Java Programming");
        System.out.println(d.getName());
    }
}
</pre>







