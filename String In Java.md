### What is String in Java?
`In Java, a string is a sequence of characters. For example, "hello" is a string containing a sequence of characters 'h', 'e', 'l', 'l', and 'o'.`
`We use double quotes to represent a string in Java.`

**Example:**

<pre>
class Main {
  public static void main(String[] args) {
    // create strings
    String first = "C#";
    String second = "Python";
    String third = "MSSQL";
    // print strings
    System.out.println(first);   // print C
    System.out.println(second);  // print Python
    System.out.println(third);   // print MSSQL
  }
}
</pre>

`Java String class provides a lot of methods to perform operations on strings such as compare(), concat(), equals(), split(), length(), replace(), compareTo(), intern(), substring() etc.`


**[Note:] The java.lang.String class implements Serializable, Comparable and CharSequence interfaces.**
![image](https://user-images.githubusercontent.com/53125546/155873785-02b42914-cc63-410e-bcb8-512cc66d89f6.png)

**CharSequence Interface**

`The CharSequence interface is used to represent the sequence of characters.` **String**, **StringBuffer** and **StringBuilder** `classes implement it. It means, we can create strings in Java by using these three classes.`
![image](https://user-images.githubusercontent.com/53125546/155873785-02b42914-cc63-410e-bcb8-512cc66d89f6.png)

`The Java String is immutable which means it cannot be changed. Whenever we change any string, a new instance is created. For mutable strings, you can use StringBuffer and StringBuilder classes.`

`We will discuss immutable string later. Let's first understand what String in Java is and how to create the String object.`
