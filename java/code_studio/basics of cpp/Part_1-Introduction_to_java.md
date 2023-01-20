# Introduction to Java  
## Introduction

Java is an **object-oriented, class-based, secured, platform-independent, and general-purpose programming language.**

Java was originally developed by James Gosling at Sun Microsystems and released in 1995 as a core component of Sun Microsystem’s Java platform.

Java programming language is based on the **write once, run anywhere (WORA)** principle, meaning that compiled Java code can run on all platforms that support Java without the need for recompilation.

Java applications are typically **compiled to bytecode** that can run on any Java Virtual Machine (**JVM**) regardless of the underlying operating system.

### Different Editions of Java

There are four editions of the Java programming language.

* **Java Platform, Standard Edition (Java SE)**
    
* **Java Platform, Enterprise Edition (Java EE)**
    
* **Java Platform, Micro Edition (Java ME)**
    
* **JavaFX**
    

**Java SE:**

Java SE, also known as **Core Java**, is the most **basic and standard version** of java.

It consists of a wide variety of general-purpose **APIs (like java. lang, java. util)** as well as many special-purpose APIs.

Java SE is used to **create Desktop applications**.

It defines everything from the basic types and objects of java programming language to high-level classes that are used for **networking, security, database access**, graphical user interface development **(GUI), and XML parsing.**

**Java EE:**

The Java EE platform is built on top of the Java SE platform.

The Enterprise Edition version of java has a **much larger usage** of Java, like the development of web services, networking, server-side scripting, and other various **web-based applications**.

Java EE uses **HTML, CSS, JavaScript,** etc., to create web pages and web services.

It is also one of the most widely used web development standards.

**Java ME:**

The Java ME platform is widely used for developing **embedded systems, mobiles, and small devices**.

Java ME uses many libraries and APIs of Java SE, as well as many of its own.

The basic aim of this edition is to work on **mobiles, wireless devices, set-top boxes**, etc.

Most of the apps developed for the phones were built on Java ME only.

**JavaFX:**

JavaFX is another edition of java technology, which is now merged with **Java SE 8**.

It is mainly used to **create rich GUI** (Graphical User Interface) in java apps.

It is supported by both **desktop** environments as well as **web browsers**.

### Features of Java

The features of the Java programming language are given below.

1. Simple: Java programming language is easy to learn and its syntax is simple and easy to understand. According to Sun Microsystem, the java programming language is simple because the java syntax is similar to C++. So, it is easier for the programmer to learn java after C++. Java has removed many rarely-used features like explicit pointers, operator overloading, etc. In Java, there is no need to remove unused objects because there is an automatic garbage collection in java.
    
2. Object-Oriented: Java is an object-oriented programming language. Everything in java is an object. We can use the functionality of our program by using objects. Object-oriented programming language simplifies software development and maintenance by providing some rules. The basic concepts of 0OPs are classes and objects, packages, polymorphism, inheritance, abstraction, encapsulation, etc.
    
3. Platform-independent: Java is a platform-independent programming language. We can write java code once and run it anywhere. Java code can be run on multiple platforms, for example, Windows, Linux, Mac, etc. Java code is compiled by the compiler and converted into byte code. This byte code is platform-independent code because it can be run on multiple platforms.
    
4. Robust: Java programming language is robust because it uses strong memory management. There is an automatic garbage collection in java to destroy unused objects. Exception handling is another feature that makes java programming robust.
    

1. Portable: Java programming language is portable because it enables you to carry byte code to any platform.
    
2. Multithreaded: Java also supports multithreaded programming. We can create multiple threads in java. The main advantage of multithreading is that it doesn't occupy the memory for each thread. It shares a common memory area. Threads are important for web applications, multimedia applications, etc.
    
3. Distributed: Java programming language is distributed because it facilitates the user to create distributed applications. We can create distributed applications in java by using RMI and EJB.
    
4. Secure: When a java program is compiled, it generates a byte code that is in the non-readable form. The java byte code cannot be read by humans. That makes the java language secure.
    

### Uses of Java

Java is the most popular, widely used object-oriented programming language. By using java, we can develop a variety of applications such as web applications, mobile applications, desktop applications, network applications, and many more. Java is used for developing different applications. Some of them are listed below:

1. **Banking**: In banking, the Java programming language is used to **develop transaction management.**
    
2. **Mobile App Development**: Java can be used to develop mobile applications. Most **android applications** are built using java. So, if you are familiar with java, it will become much easier to develop mobile applications.
    
3. **Desktop Applications**: We can also create GUI applications in java. Java provides **AWT, Swings, and JavaFX** to develop desktop applications.
    
4. **Big Data**: In Big Data, the **Hadoop MapReduce framework** is written using java.
    
5. **Web applications**: We can also create web applications using java. The most popular frameworks like **Spring, Spring Boot, and Hibernate** used for developing web applications are based on java.
    

## JDK, JRE and JVM

JDK, JRE, and JVM are the most important parts of the Java programming language. Without these, you can not develop and run java programs on your machine.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673869249659/7e5e1388-d150-4d4b-b215-f226f4083553.png align="center")

1. **JDK**: JDK stands for **Java Development Kit**. JDK provides an environment to **develop and execute** the java program. JDK is a kit that includes two things - **Development Tools** to provide an environment to develop your java programs and JRE to execute your Java programs.
    
2. **JRE**: JRE stands for **Java Runtime Environment**. JRE provides an environment to **only run (not develop)** the java programs onto your machine. JRE is only used by the **end-users** of the system. JRE consists of **libraries** and other files that JVM uses at runtime.
    
3. **JVM**: JVM stands for **Java Virtual Machine**, which is a very important part of both JDK and JRE because it is **inbuilt** into both. Whatever java program you run using JDK and JRE goes into the JVM and JVM is responsible for executing the java program line by line.
    

## How to run a Java Code?

### main() Method

Before explaining the java main() method, let’s first create a simple program to print Hello World.

After that, we will explain why the main() method in java is a public static void main(String args\[\]).

```java
public class HelloWorld { 
    public static void main(String args[]) { 
        System.out.println("Hello World"); 
    } 
}
```

* **public**: the public is an **access modifier** that can be used to specify who can access this main() method. It simply defines the **visibility of the method**. The **JVM** calls the main() method **outside the class**. Therefore it is necessary to make the java main() method as public.
    
* **static**: static is a **keyword** in java. We can make static variables and static methods in java with the help of the static keyword. The main advantage of a static method is that we can call this method **without creating an instance** of the class. JVM calls the main() method without creating an instance of the class, therefore it is necessary to make the java main() method static.
    
* **void**: void is a **return type of method**. The java main() method **doesn’t return** any value. Therefore, it is necessary to have a void return type.
    
* **main**: main is the **name of the method**. It is a method where program execution starts.
    
* **String args\[\]:** String in java is a class that is used to **work on Strings** and args is a **reference variable** that refers to an array of type Strings. If you want to pass the argument through the command line then it is necessary to make the argument of the main() method as String args\[\].
    

### Compile and Run

Below are the steps to compile and run your first java program

1. Open a text editor like notepad or notepad++.
    
2. Write a java program in your text editor and save it with (java extension), remember that the file name and the class name may be the same. For example, if you are creating a class HelloWorld, then you need to save it with [HelloWorld.java](http://HelloWorld.java).
    
3. Open your command prompt. Set the directory where your java program is saved.
    
4. Once you enter the directory where your java program is saved, now it's time to compile your java program, to compile the java program use the command javac HelloWorldjava (In this case my java file is [HelloWorld.java](http://HelloWorld.java)).
    
5. Once your Java program compiles fine, now it's time to run your java program. You can run your java program by using the java HelloWorld (java file Name) command.
    

### Creating Comments

Comments are statements that are **not executed** by the compiler.

Comments make the program more **human-readable** by including the details of the code involved.

The proper use of comments makes **maintenance and debugging** of the code **easier**.

**Types of Comments**

There are three types of comments in java

* Single line comments
    
* Multi-line comments
    
* Documentation comments
    

**Single-line comment:**

The single-line comment is used to comment only one line. A beginner-level programmer uses mostly single-line comments for describing the code functionality.

**Syntax**:

```java
//write your comment here
```

**Example**:

```java
// Java program to show single line comment 
public class HelloWorld { 
    public static void main (String args[]) { 
        // Print "Hello World" on console 
        system.out.println ("Hello world");
    }
}
```

**Multi-line comments:**

The multi-line comments are used to comment on multiple lines of code.

**Syntax**:

```java
Syntax: 
/*
This is 
multiline Comment
*/
```

**Example:**

```java
public class HelloWorld { 
    public static void main (String args[]) { 
        /*
        Here, we nave declared a variable and 
        we are printing its value 
        */ 
        int a = 10; 
        system.out.println(a);
    }
}
```

**Documentation Comments:**

This type of comment is used generally when we write the code for projects. It helps to generate a documentation page for reference, which can be used for getting information about the methods present, their parameters, etc.

**Syntax:**

```java
/**Comment start
*
*tags are used in order to specify a parameter 
*or method or heading. 
*HTML tags can also be used 
*such as <h1>
*
*comment ends*/ 
```

**Example:**

```java
// Java program to illustrate documentation comments
/** 
*Find product of four numbers! 
*The FindPro program implements an application 
*that simply calculates product of four integers 
*and Prints the output on the Screen. 
*
*@author abc 
*@version 1.0 
*@since xyx
*/
 public class FindPro { 
    /**
    *
    *This method is used to find the product of four integers. 
    *
    *@param numl This is the first parame ter to FindPro method 
    *@param num2 This is the second parameter to FindPro method
    *@param num3 This is the third parameter to FindPro method 
    *@param num4 This is the fourth parameter to FindPro method    
    *@return int This returns average 0f numA, numB and numC.
    */ 
    public int FindPro(int num1, int num2, int num3, int num4) { 
        return (numi  num2 num3num4) 
    }
    /** 
    *
    *This is the main method which makes use of the FindPro method. 
    *
    *@param args Unused. 
    *@return Nothing. 
    */
    public static void main (string args []) { 
        FindPro obj = new FindPro(); 
        int pro obj.FindPro(10, 20, 20, 40); 
        System.out.println("Product of 10, 20, 30 and 40 is: " + pro) ; 
    }
}
```

**Output:**

```java
Product of 10, 20, 30 and 40 is: 240000
```
