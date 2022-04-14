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

### How to create a string object?
`There are two way to :`
**1. By string literal**
**2. By new keyword**

**Frist:** `String Literal`

`Java String literal is created by using double quotes.`

**syntax**
<pre>
String name="Md Somrat Akbor"
</pre>

**Second:** `new keyword`
`In such case, JVM will create a new string object in normal (non-pool) heap memory, and the literal "Welcome" will be placed in the string constant pool. The variable s will refer to the object in a heap (non-pool).`


**syntax**
<pre>
String name= new String("Md Somrat Akbor")
</pre>


### Methods of Java String Class
<table class="alt">
<tbody><tr><th>No.</th><th>Method</th><th>Description</th></tr>
<tr><td>1</td><td><a href="#">char charAt(int index)</a></td><td>It returns char value for the particular index</td></tr>
<tr><td>2</td><td><a href="#">int length()</a></td><td>It returns string length</td></tr>
<tr><td>3</td><td><a href="#">static String format(String format, Object... args)</a></td><td>It returns a formatted string.</td></tr>
<tr><td>4</td><td><a href="#">static String format(Locale l, String format, Object... args)</a></td><td>It returns formatted string with given locale.</td></tr>
<tr><td>5</td><td><a href="#">String substring(int beginIndex)</a></td><td>It returns substring for given begin index.</td></tr>
<tr><td>6</td><td><a href="#">String substring(int beginIndex, int endIndex)</a></td><td>It returns substring for given begin index and end index.</td></tr>
<tr><td>7</td><td><a href="#">boolean contains(CharSequence s)</a></td><td>It returns true or false after matching the sequence of char value.</td></tr>
<tr><td>8</td><td><a href="#">static String join(CharSequence delimiter, CharSequence... elements)</a></td><td>It returns a joined string.</td></tr>
<tr><td>9</td><td><a href="#">static String join(CharSequence delimiter, Iterable&lt;? extends CharSequence&gt; elements)</a></td><td>It returns a joined string.</td></tr>
<tr><td>10</td><td><a href="#">boolean equals(Object another)</a></td><td>It checks the equality of string with the given object.</td></tr>
<tr><td>11</td><td><a href="#">boolean isEmpty()</a></td><td>It checks if string is empty.</td></tr>
<tr><td>12</td><td><a href="#">String concat(String str)</a></td><td>It concatenates the specified string.</td></tr>
<tr><td>13</td><td><a href="#">String replace(char old, char new)</a></td><td>It replaces all occurrences of the specified char value.</td></tr>
<tr><td>14</td><td><a href="#">String replace(CharSequence old, CharSequence new)</a></td><td>It replaces all occurrences of the specified CharSequence.</td>
</tr>
<tr><td>15</td><td><a href="#">static String equalsIgnoreCase(String another)</a></td><td>It compares another string. It doesn't check case.</td></tr>
<tr><td>16</td><td><a href="#">String[] split(String regex)</a></td><td>It returns a split string matching regex.</td>
</tr><tr><td>17</td><td><a href="#">String[] split(String regex, int limit)</a></td><td>It returns a split string matching regex and limit.</td>
</tr><tr><td>18</td><td><a href="#">String intern()</a></td><td>It returns an interned string.</td>
</tr><tr><td>19</td><td><a href="#">int indexOf(int ch)</a></td><td>It returns the specified char value index.</td></tr>
<tr><td>20</td><td><a href="#">int indexOf(int ch, int fromIndex)</a></td><td>It returns the specified char value index starting with given index.</td></tr>
<tr><td>21</td><td><a href="#">int indexOf(String substring)</a></td><td>It returns the specified substring index.</td></tr>
<tr><td>22</td><td><a href="#">int indexOf(String substring, int fromIndex)</a></td><td>It returns the specified substring index starting with given index.</td></tr>
<tr><td>23</td><td><a href="#">String toLowerCase()</a></td><td>It returns a string in lowercase.</td></tr>
<tr><td>24</td><td><a href="#">String toLowerCase(Locale l)</a></td><td>It returns a string in lowercase using specified locale.</td></tr>
<tr><td>25</td><td><a href="#">String toUpperCase()</a></td><td>It returns a string in uppercase.</td></tr>
<tr><td>26</td><td><a href="#">String toUpperCase(Locale l)</a></td><td>It returns a string in uppercase using specified locale.</td></tr>
<tr><td>27</td><td><a href="#">String trim()</a></td><td>It removes beginning and ending spaces of this string.</td></tr>
<tr><td>28</td><td><a href="#">static String valueOf(int value)</a></td><td>It converts given type into string. It is an overloaded method.</td></tr>
</tbody></table>



