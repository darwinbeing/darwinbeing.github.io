---
layout: post
title:  "How to generate Java Getters and Setters with Lombok (Part 1)"
permalink: /:title
date:   2018-05-16 00:00:00
author: André Maré
images:
  - assets/images/blog-header/java-3-2.jpg
excerpt:
  The Lombok Project is a java library that helps a developer generate boilerplate code like "getter" and "setter" methods for Plain Old Java Objects (POJOs). This post will focus on how to make use of the @Getter and @Setter annotations on the top off a class to generate the mutator and accessor methods of a class.

categories: [Java, Lombok]
tags: [java, lombok, mutator, setter, accessor, getter]
---

##### Quick Summary
The Lombok Project is a java library that helps a developer generate boilerplate code like "getter" and "setter" methods for Plain Old Java Objects (POJOs). By simply adding the Lombok library to your IDE and build path, the Lombok library will autogenerate the Java bytecode, as per the annotations, into the .class files.

This post will focus on how to make use of the @Getter and @Setter annotations on the top off a class to generate the mutator and accessor methods of a class.

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
In Java, a mutator method is a method used to control changes to a variable within a Java class. They are also widely known as setter methods. Often a setter is accompanied by a getter (also known as an accessor), which returns the value of the private member variable.

There are many opinions about the use of Getter and Setter methods, and when to use them correctly, but this will not be discussed in this post. Let's assume that you have correctly applied OO principles to the design of your Java class and require the getter and setter methods.

If a Java class contains a large number of members attributes, it will contain a large number of boilerplate code like the getter and setter methods, and hence the use of the Lombok library makes it much easier to generate the code. This means less errors can occur when writing the code yourself, and the class is easier to read and understand.

##### Example 1: Getter & Setter on Class
The @Getter and/or @Setter annotation can be placed on the class declaration. This is similar as if you annotate all the non-static fields in that class with the annotations.

The following example illustrates how to add the @Getter and/or @Setter annotation to the top of the class.

<script src="https://gist.github.com/Code2Bits/bceef0f30d626a490e36f6d252b29829.js"></script>

To truly appreciate the magic of the Lombok library, you should compile the Student class by making use of the "javac" command within a terminal. To run the command successfully, you should ensure that the Lombok Jar file and the Student.java file are within the same directory from where you execute the command. After the Student class has been compiled, you should disassemble the Student Java class file by making use of the "javap" command.

```bash
$ javac -cp lombok.jar Student.java
$ javap Student.class
```

The javap command prints out the package, protected, and public fields and methods of the class passed to it. The javap command displays its output to stdout. Therefor the private member attributes of the Student class is not printed out, but one can now see how a getter and setter method has been created for each of the non-static private members of the class.

<script src="https://gist.github.com/Code2Bits/425597962d0bd42fd90c78a9ec02de74.js"></script>

The 7 getter (accessor) methods are listed from line 3 - 9, and the 7 setter (mutator) methods are listed from line 10 - 16. The generated getter/setter methods will be public, unless you explicitly specify an AccessLevel. Access levels for getter and setter annotations will be discussed in the next post.

##### Summary
Congratulations !!! You have successfully generated Getter and Setter methods for a Java class by making use of the Lombok java library. Please lookout for more examples on how to make use of Project Lombok to simplify your Java coding experience.

[1]: https://projectlombok.org/download
[2]: http://www.oracle.com/technetwork/java/javase/downloads/index.html
[3]: https://spring.io/tools/sts/all
[4]: {{site.url}}/how-to-generate-java-getters-and-setters-with-lombok-part-1
[5]: {{site.url}}/how-to-generate-java-getters-and-setters-with-lombok-part-2
