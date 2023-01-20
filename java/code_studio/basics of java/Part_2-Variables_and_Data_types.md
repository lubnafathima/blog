## Introduction

### Introduction and Declaration of Variables

**Introduction to Variables**

A Variable is a name given to a **memory location.**

It is used to store a value that may vary.

Java is a statically typed language, and hence, all the variables are declared before use.

**Variable Declaration**

In Java, we can declare variables as follows:

* type: Type of the data that can be stored in this variable. It can be int, float, double, etc.
    
* name: Name given to the variable.
    

```java
// Syntax:
data_type variable_name;
// Example:
int x;
```

In this way, we can only create a variable in the memory location. Currently, it doesn’t have any value. We can assign the value in this variable by using two ways:

* By using variable initialization.
    
* By taking input
    

Here, we have discussed only the first way, i.e. variable initialization. We will discuss the second way later.

```java
// Syntax
data_type variable_name = value; 
// Example: 
int x = 10;
```

### Variables naming Convention in Java

* A variable name should be short and meaningful.
    
* It should begin with a lowercase letter.
    
* It can begin with special characters such as (underscore) and a $ (dollar) sign.
    
* If the variable name contains multiple words, then use the camel case, ie. the variable name should start with a lowercase letter followed by an uppercase letter. For eg: helloWorld, camelCase.
    
* Always try to avoid single-character variable names such as i,j, and k except for the temporary variables.
    
* A variable name can not contain whitespaces. We can't use keywords(pre-defined literals) as the variable names.
    

## Keywords in Java

### Java Keywords:

Keywords in Java are also known as reserved words.

These are predefined words, therefore they can’t be used as a variable name.

If we will use keywords as a variable name, the result will be a compile-time error.

The list of all the Java Keywords is given below.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673874755003/cb53e250-0444-4cfb-a28a-3c7efc6c6a34.png align="center")

```java
// Examples: 
// Correct 
int x = 10; 
int _x = 10; 
int $x = 10; 
Int x1 = 10;
// Incorrect 
int 1x = 10; 
int number = 10;
```

## Data Types in Java

The data type defines the type of value that can be stored in a variable.

For example, if a variable has an int data type, it can only store an integer value.

In Java, there are two categories of data types.

### Primitive Data Type:

A primitive data type is predefined by the language and is named by a **keyword** or reserved keyword.

There are **eight** types of primitive data types in java such as **boolean, char, int, short, byte, long, float, and double.**

* **boolean**: boolean data type specifies only one bit of information and it is used to store only two possible values either true or false.
    
* **byte**: byte data type is 8-bit signed two’s complement integer. Its value lies between -128 to 127. It has a minimum value of -128 and a maximum value of 127 (inclusive). The byte data type is most commonly used to save memory in large arrays.
    
* **short**: short data type is a 16-bit signed two’s complement integer. It can hold any number between -32768 to 32767 (inclusive). Like byte data type, it is commonly used to save memory in large arrays.
    
* **int**: int data type is a 32-bit signed two’s complement integer. It can hold the number between -2,147,483,648 to 2,147,483,648. The default value of the int data type is 0.
    
* **long**: long data type is 64-bit two’s complement integer. It can hold the number between -2^63 to 2^63-1. The default value of the long data type is 0.
    
* **float**: float data type is used to store floating-point numbers. The float data type is a single-precision 32-bit IEEE 754 floating-point. It can hold 6 to 7 decimal digits. It is recommended to use float instead of double if you need to save memory in large arrays of floating-point numbers. The default value of float is 0.0f.
    
* **double**: double data type is generally used to store decimal values. The double data type is a double-precision 64-bit IEEE 754 floating-point. For decimal values, this data type is generally the default choice. The default value of double is 0.0d.
    
* **char**: The char data type is used to store characters. The char data type is a single 16-bit Unicode character.
    

### Non-Primitive Data Type:

Non-Primitive data type refers to the objects.

ArrayList and String are some examples of Non-Primitive data types.

We will discuss the Non-Primitive data type later.

Example:

```java
// Primitive Data Types 
int price = 5000;  // Integer Value
float rateOfInterest = 5.99f;  // Floating point number
char ch = 'a';  // Character
// Non-Primitive Data Types 
String str = "Coding Ninjas"; // String
```

## Scope of Variables in Java

The variable scope is the part of the program where the variable is accessible.

The scope of the variable can be determined at compile time. There are mainly two types of variable scope.

### **Local Variables Scope:**

A variable that is defined inside a block, method body, or constructor is called a local variable.

These variables can't be accessed outside the method.

```java
// Example: 
public class Variablescope { 
    void method () { 
        // Local variable (Method Level Scope) 
        // This method can't be accessed outside 
        // method body. 
        int x;
    }
}
```

### **Member/Class Level Variable Scope:**

A variable that is declared inside the class but outside the method body, block, or constructor is known as a member/class-level variable.

These variables can be directly accessed anywhere in the class.

```java
// Example: 
class VariableScope {
    //variable defined inside the class 
    int x; 
}
public class VariablescopeDemo{ 
    public static void main (String args[]) { 
        //Creating VariableScope class object 
        Variablescope obj = new VariableScope(); 
        //Assigning values in the variable 
        obj.x = 10; 
        // Printing the value 
        system.out.printIn(obj.x);
    }
}
// Output: 
1O
```

## Types of Variables in Java

A variable is a name given to memory location. There are three types of variables in java.

* Local Variable
    
* Instance Variable
    
* Static variable
    

### **Local Variables:**

A variable that is defined inside a block, method body, or constructor is called a local variable.

These variables are created when the methods are called and they get destroyed when the methods are executed and returned to the caller.

The initialization of the local variable is mandatory.

If you don't initialize the variable before use, the compiler will give a compile-time error.

```java
// Example: 
public class Addition { 
    // Function to add two numbers 
    public void add() { 
        // Local variables 
        int a = 10; 
        int b = 20; 
        int c = a + b;
        // Printing the sum 
        System.out.println(c); 
    }
    //Driver Code 
    public static void main(Sstring args[]) { 
        //Creating an object of Addition class 
        Addition obj = new Addition(); 
        // Function Call 
        obj.add(); 
    }
}
// Output:
30
```

### **Instance Variables:**

A variable that is declared inside the class but outside the method body, block, or constructor is known as an instance variable.

It is a non-static variable.

These variables are created when an instance (object) of the class is created and are destroyed when the object is destroyed.

Initialization of the instance variable is not mandatory.

Even If you don't initialize the instance variable, it has a default value in it. Instance variables can be accessed only by creating the object of the class.

```java
// Example: 
class student { 
    //These are instance variables 
    // these are declared inside the 
    // class but outside the method body 
    String name;
    int rollno; 
}
public class student Records{ 
    public static void main(string args[]) {
        //Creating Student class object 
        Student obj = new Student (); 
        // Assigning values in the variables 
        obj.name = "Ram"; 
        obj.rollno = 10; 
        // Printing name and rollno 
        system.out.println(obj.name); 
        system.out.println(obj.rollno);
    }
}
// Output
Ram
10
```

### **Static Variables:**

A variable that is declared static is known as a static variable. It is also known as a class variable.

These variables are created at the beginning of the program execution and destroyed automatically when the program execution ends.

We can create only a single copy of a static variable.

To access the static variables, we don't need to create the object of the class.

We can simply access the static variable as

```java
// Stntax
class_Name. variable_Name; 
// Example: 
class student { 
    // static variables 
    public static int rollno; 
    public static String name = "Ram"; 
}
public class studentDemo { 
    public static void main (String args[]) {
        // accessing static variable without creating object 
        student.rollno = 10;
        system.out.println(student.name +" 's rollno is :" + Student.rollno);
    }
}
//Output: 
Ram's rollno is :10
```

## TypeCasting in Java

TypeCasting in Java is the process of converting one primitive data type into another. TypeCasting can be done automatically and explicitly.

When we assign the value of one data type to another data type, then there is a chance that two data types might not be compatible with each other.

The Java compiler will automatically perform the conversion if the data types are consistent.

This type of conversion is known as Automatic Type Conversion.

If the java compiler cannot perform the conversion automatically, they need to be cast explicitly.

There are two types of TypeCasting in Java.

* Widening or Automatic Type Conversion
    
* Narrowing or Explicit Type Conversion
    

### Widening or Automatic Type Conversion:

When we assign a value of a smaller data type to a large data type, this process is known as Widening Type Casting.

It is also known as Automatic Type Conversion because the Java compiler will perform the conversion automatically.

This can happen only when the two data types are compatible.

```java
byte -> short -> int -> long -> float > double (Widening or Automatic Type Conversion) 
```

For example, In Java, int data types are compatible, but it isn't compatible with char and boolean data types. Also, char and boolean data types are not compatible with each other.

```java
// Example: 
public class WideningConversation {
    public static void main(string argsl]) { 
        // Automatic Type Converson. 
        int i = 2147483647 ; // Int max value in java. 
        long l = 1; // AutomaticaLly converted to long, now we can extend l's value. 
        l = l + 1; 
        double d = 1; // Automatically converted to double. 
        system.out.println ("Int value: " + i); 
        system.out.printIn("Long value " + 1); 
        System.out.println("Double value: " + d); 
    }
}
// Output 
Int value: 2147483647 
Long value: 2147483648 
Double value: 2.147483648E9 
```

### Narrowing or Explicit Type Conversion:

When we assign a value of a large data type to a small data type, the process is known as Narrowing Type Casting.

This can't be done automatically. We need to convert the type explicitly.

If we don't perform coasting, the java compiler will give a compile-time error.

```java
double-> float > long-> int -> short -> byte ( Narrowing or Explicit Type Conversion)
// Example: 
public class Explicitconversation { 
    public static void main (String args[]) { 
        //Explicit Type Conversion 
        double d = 25.123; 
        int i = (int) d; 
        byte b= (byte) i; 
        System.out.println("Double value: " + d); 
        System.out.println ("Int value: "+ i); 
        System.out.println ("Byte value: "+ b); 
    }
}
// Output 
Double value: 25.123 
Int value: 25 
Byte value: 25
```

## Overflow and Underflow in Java

Overflow in java happens when we assign a value to a variable that is more than its range and Underflow is the opposite to overflow.

In case of overflow and underflow, the Java compiler doesn't throw any error.

It simply changes the value.

For example, in the case of an int variable, its size is 4 bytes or 32 bits.

The maximum value of the int data type is 2,147,483,647 (Integer.MAX\_VALUE) and after incrementing 1 on this value, it will return -2,147,483,648 (Integer.MIN\_VALUE). This is known as overflow.

The minimum value of the int data type is -2,147,483,648 (integer.MIN\_VALUE) and after decrementing 1 on this value, it will return 2,147,483,647 (Integer.MAX VALUE). This is known as underflow in Java.

```java
// Example: 
public class OverflowExample { 
    public static void main (String args[]) { 
        // Overflow 
        int overFlow = 2147483647; 
        system.out.println ("Overflow "+(overFlow + 1)); 
        // Underflow 
        int underFlow = -2147483648; 
        System.out.println("Underflow "+ (underFlow + 1));
    }
}
// Output 
Overflow -2147483648 
Underflow 2147483647
```
