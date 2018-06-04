---
layout: post
title:  "How to generate Java Getters and Setters with Lombok (Part 2)"
permalink: /:title
date:   2018-05-17 00:00:00
author: André Maré
images:
  - assets/images/blog-header/java-3-2.jpg
excerpt:
  This post will focus on how to make use of the @Getter and @Setter annotations on top off the member attributes of a class to generate the mutator and accessor methods for those fields. This post will also describe how to define Access Levels for the mutator and accessor methods.

categories: [Java, Lombok]
tags: [java, lombok, mutator, setter, accessor, getter]
---

##### Quick Summary
The Lombok Project is a java library that helps a developer generate boilerplate code like "getter" and "setter" methods for Plain Old Java Objects (POJOs). By simply adding the Lombok library to your IDE and build path, the Lombok library will autogenerate the Java bytecode, as per the annotations, into the .class files.

This post will focus on how to make use of the @Getter and @Setter annotations on top off the member attributes of a class to generate the mutator and accessor methods for those fields. This post will also describe how to define Access Levels for the mutator and accessor methods.

##### Requirements
The following list defines the technologies and libraries I used to implement the sample code:

* Lombok Library V 1.16.20. [Download][1]
* JDK 1.8 [Download][2]
* Spring Tool Suite [Download][3]


##### Multiple Posts
This will form part of a multi-part series on how to use the Lombok java library to auto generate the getter and setter methods for Java classes.

* [How to generate Java Getters and Setter with Lombok (Part 1)][4]
* [How to generate Java Getters and Setter with Lombok (Part 2)][5]


##### Introduction
You can annotate any field with @Getter and/or @Setter and the Lombok library will generate the access & mutator method for that specific member attribute. This allow you to be more specific for which fields you require accessor or mutator methods and even have the ability to specify the Java Access Modifiers for the particular methods.

Java Access Modifiers specifies the scope (accessibility) of member attributes, methods, constructors and classes. There are 4 types of access modifiers in Java namely, private, default, protected and public.

* The **public** access modifier specifies that the member and/or method can be accessed from anywhere.
* The **protected** access modifier specifies that the member and/or method  can only be accessed within its own package (as with package-private) and, in addition, by a subclass of its class in another package.
* The **default** access modifier (package-private or no modifier specified) specifies that the member and/or method  is only visible within its own package.
* The **private** access modifier specifies that the member and/or method can only be accessed in its own class.</li>


##### Example: Getter & Setter on Fields with AccessLevels

It is possible to specify the access level for the @Getter and/or @Setter annotations to auto generate the accessor and mutator methods with the appropriate Java Access Modifiers. This allows you to control the accessibility of the methods via the Lombok library.

The generated accessor/mutator method will be public unless you explicitly specify an AccessLevel as part of the annotation. The example below illustrates the use AccessLevels to specify the Java Access Modifier for each method.

You can always manually disable getter/setter generation for any field by using the special AccessLevel.NONE access level.

<script src="https://gist.github.com/Code2Bits/168f68529130623292d4510f0849fabc.js"></script>

The following table illustrates how the Lombok AccessLevel will be mapped to the Java Access Modifier to be used for the access and mutator methods.


<table>
<tr><th align="left">Lombok AccessLevel</th><th align="left">Java Access Modifier</th></tr>
<tr><td>AccessLevel.PRIVATE</td><td>private</td></tr>
<tr><td>AccessLevel.PROTECTED </td><td>protected</td></tr>
<tr><td>AccessLevel.PUBLIC </td><td>public</td></tr>
<tr><td>AccessLevel.PACKAGE </td><td>default</td></tr>
<tr><td>AccessLevel.MODULE</td><td>default</td></tr>
<tr><td>AccessLevel.NONE</td><td>Method Not Generated !!!</td></tr>
<tr><td>Not Specified</td><td>public</td></tr>
</table>

You should compile the Student class by making use of the "javac" command within a terminal. To run the command successfully, you should ensure that the Lombok Jar file and the Student.java file are within the same directory from where you execute the command. After the Student class has been compiled, you should disassemble the Student Java class file by making use of the "javap" command.

```bash
$ javac -cp lombok.jar Student.java
$ javap Student.class
```

The javap command prints out the package, protected, and public fields and methods of the class passed to it. The javap command displays its output to stdout. Therefor the private member attributes of the Student class is not printed out, but one can now see how a getter and setter method has been created for each of the non-static private members of the class, depending on the AccessLevel that was set as part of the annotation.

<script src="https://gist.github.com/Code2Bits/496e07f7f5dbfddbcc5edad577879322.js"></script>

So based on the example, the following are the reasons why lombok generated the methods with different java access modifiers:

* **Member Attribute: id** - The accessor method is public because the AccessLevel was not specified. The mutator method is private because the AccessLevel was set to PRIVATE.

* **Member Attribute: firstName** - The accessor method is public because the AccessLevel was not specified. The mutator method is protected because the AccessLevel was set to PROTECTED. (See line 5)

* **Member Attribute: lastName** - The accessor method is public because the AccessLevel was not specified. The mutator method is public because the AccessLevel was set to PUBLIC. (See line 7)

* **Member Attribute: gender** - The accessor method is public because the AccessLevel was not specified. The mutator method is "default" because the AccessLevel was set to PACKAGE. (See line 9)

* **Member Attribute: birthDate** - The accessor method is public because the AccessLevel was not specified. The mutator method is "default" because the AccessLevel was set to MODULE. (See line 11)

* **Member Attribute: contactEmail** - The accessor method is public because the AccessLevel was not specified. The mutator method is not generated because the AccessLevel was set to NONE.

* **Member Attribute: isFirstYear** - The accessor method is public because the AccessLevel was not specified. The accessor method is public because the AccessLevel was not specified.

##### Summary
This post has shown another example of how to make use of the Lombok library together with the @Getter and @Setter annotations to generate the methods. It has further shown how to specify the expected java access modifier for each of generated methods. The next post in the series will illustrate how to make use of lombok config to change how the methods are generated.



[1]: https://projectlombok.org/download
[2]: http://www.oracle.com/technetwork/java/javase/downloads/index.html
[3]: https://spring.io/tools/sts/all
[4]: {{site.url}}/how-to-generate-java-getters-and-setters-with-lombok-part-1
[5]: {{site.url}}/how-to-generate-java-getters-and-setters-with-lombok-part-2
