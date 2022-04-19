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
