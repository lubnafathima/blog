# Introduction to C++

This blog contains notes took by me while learning Basics of C++ at Coding Ninjas.

## Introduction, Features and Uses of C++

### Introduction

* C++ is a general-purpose programming language and is widely used nowadays for **competitive programming**.
    
* It has **imperative, object-oriented, and generic programming** features.
    
* C++ runs on lots of platforms like **Windows, Linux, Unix, Mac, etc.**
    
* It can be used to develop **operating systems, browsers, games**, and so on.
    
* This makes C++ powerful as well as flexible.
    
* You can run programs and practice them on your local desktop, Using one of these compilers: **Code blocks, VS Code, Dev C++, Atom**, and many more.
    

### Features of C++

* Simple
    
* Portability
    
* Powerful and Fast
    
* Rich Library
    
* Platform Dependent
    
* Mid-level programming language
    
* Structured programming language
    
* Object-Oriented
    
* Case Sensitive
    
* Compiler Based
    
* Syntax based language
    
* Pointers
    
* Dynamic Memory Management
    

**Simple**:

* C++ is a simple language because it provides a **structured approach** (to break the problem into parts), a **rich set of library functions, data types,** etc.
    
* It allows us to follow both **procedural** as well as **functional approaches** to design our flow of control.
    

**Portability:**

* It is the concept of **carrying the instruction** from one system to another system.
    
* In C++ language **.cpp file** contains **source code**, and we can also edit this code.
    
* **.exe file** contains the **application**, which is the only file that can be executed. W
    
* When we write and compile any C++ program on the Windows operating system, it **efficiently runs** on other window-based systems.
    

**Powerful:**

* C++ is a very powerful programming language, and it has a **wide variety** of data types, functions, control statements, decision-making statements, etc.
    
* C++ is a **fast language** as compilation and execution time is less.
    
* Also, it has a wide variety of **data types, functions & operators**.
    

**Rich Library**:

* C++ library is full of **in-built functions** that save a tremendous amount of time in the software development process.
    
* As it contains almost **all kinds of functionality**, a programmer can need it in the development process.
    
* Hence, saving **time** and increasing development **speed**.
    

**Platform Dependent:**

* Platform-dependent language means the language in which programs can be **executed only on the operating system where it is developed & compiled**.
    
* It **cannot run or execute** on any other operating system. E.g., compiled programs on Linux won’t run on Windows.
    

**Mid-level programming language:**

* C++ can do both **low-level & high-level** programming.
    
* That is the reason why C++ is known as a mid-level programming language.
    

**Structured programming language**:

* C++ is a structured programming language as it allows to **break off** of the program into parts **using functions**.
    
* So, it is **easy to understand and modify**.
    

**Object-oriented**:

* C++ is an **object-oriented programming** language.
    
* OOPs make **development and maintenance easier**.
    
* whereas, in Procedure-oriented programming language, it is **not easy** to manage if code grows as project size grows.
    
* It follows the concept of oops like **polymorphism, inheritance, encapsulation, abstraction.**
    

**Case sensitive**:

* C++ is a **case-sensitive** programming language.
    
* In C++ programming, '**break and BREAK'** both are different.
    

**Compiler-Based:**

* C++ is a **compiler-based** language, unlike Python.
    
* C++ programs used to be compiled, and their **executable file is used to run** it due to which C++ is a relatively faster language than Java and Python.
    

**Syntax-based language**:

* C++ is a **strongly typed syntax-based** programming language.
    
* If any language **follows the rules and regulations strictly**, it is known as a strongly syntax-based language.
    
* Other examples of syntax-based languages are C, C++, Java, .net etc.
    

**Pointer**:

* C++ supports pointers that allow the user to **deal directly with the memory** and **control** the programmer.
    
* This makes it very suitable for **low-level tasks** and **very complicated projects.**
    
* It is known to **increase the speed of execution** by decreasing the memory access overhead.
    

**Dynamic Memory Management**:

* It **supports** the feature of dynamic memory allocation.
    
* In C++ language, we can **free the allocated memory** by calling the **free()** function.
    
* These features are missing in languages like C.
    

### Uses of C++

There are several benefits of using C++ because of its **features and security**.

below are some uses of C++ Programming Language

**Operating Systems**:

* One of the key requirements of an Operating System is that it should be **very fast** as it is responsible for **scheduling and running** the user programs.
    
* The **strongly typed and fast nature** of C++ makes it an ideal candidate for writing operating systems.
    
* Also, C++ has a **vast collection of system-level functions** that also help in writing low-level programs.
    
* Microsoft Windows or Mac OS X, or Linux all operating systems have some parts programmed in C++.
    

**Games**:

* Again since most, games need to be **faster to support smooth gameplay**, C++ is extensively used in game design.
    
* C++ can easily **manipulate hardware resources**, and it can also provide procedural programming for CPU-intensive functions.
    

**Browsers**:

* With the **fast performance** of C++, most browsers have their **rendering** software written in C++.
    
* Browsers are mostly used in C++ for **rendering purposes**. Rendering engines need to be faster in execution as most people do not like to wait for the web page to be loaded.
    

**Libraries**:

* Many **high-level libraries** use C++ as the core programming language.
    
* For example, **TensorFlow** uses C++ as the back-end programming language.
    
* Such libraries required **high-performance computations** because they involve multiplications of huge matrices to train Machine Learning models.
    
* As a result, performance becomes critical.
    
* C++ comes to the rescue in such libraries.
    

**Graphics**:

* C++ is widely used in almost all **graphics applications** that require **fast rendering, image processing, real-time physics, and mobile sensors**.
    

**Cloud/Distributed Systems:**

* Cloud storage systems use **scalable file systems** that work close to the hardware.
    
* Also, the multi-threading libraries in C++ provide h**igh concurrency and load tolerance.**
    

**Embedded Systems:**

* C++ is **closer to the hardware leve**l, and so it is quite useful in **embedded systems** as the software and hardware in these are closely coupled.
    
* Many embedded systems use C++, Such as **smartwatches, MP3 players, GPS systems**, etc.
    

**Compilers**:

* Compilers of various programming languages use **C++ as the back-end** programming language.
    

## **How to implement a code in C++**

### Headers in C++

* C++ code begins with the inclusion of header files.
    
* There are many header files available in the C++ programming language.
    
* So, what are these header files? The names of program elements such as variables, functions, classes, and so on must be declared before they can be used.
    
* For example, you can’t just write x = 42 without first declaring variable x as:
    
    ```cpp
    int x = 42;
    ```
    
    The declaration tells the compiler whether the element is **an int, a double, a float, a function, or a class**.
    
    Similarly, header files allow us to put **declarations** in one location and then import them wherever we need them.
    
    This saves a lot of typing in multi-file programs.
    
    To declare a header file, we use the **#include** directive in every **.cpp file**.
    
    This #include is used to ensure that they are not inserted multiple times into a single .cpp file.
    
    Now, moving forward to the code:
    

```cpp
#include <iostream>
using namespace std;
```

* **iostream** stands for **Input/Output stream**, meaning this header file is necessary to take input through the user or print output to the screen. This header file contains the definitions for the functions:
    
    * **cin**: used to take input
        
    * **cout**: used to print output
        
* **namespace** defines which input/output form is to be used. You will understand these better as you progress in the course.
    
* **Note**: **semicolon (;) is used for terminating a C++ statement.** i.e., different statements in a C++ program are separated by a semicolon.
    

### main() function

```cpp
int main() { 
    Statement 1; 
    Statement 2; 
    ... 
}
```

int main()

* **int**: This is the **return type** of the function. You will get this thing clear once you learn about Functions.
    
* **main()**: This is the portion of any C++ code inside which all the **commands** are written and executed.
    
    * This is the line at which the program will **begin executing**. This statement is similar to the **start block** of flowcharts.
        
* **{}**: All the code written inside the curly braces is said to be in **one block**, also known as a particular function scope. Again, things will be clear once you learn about Functions
    

### Compiler and Run

For compiling and running a CPP program in Linux following are the command lines:

```cpp
Compile: g++ Filename.cpp 
Run or execute: ./a.out
```

For compiling and running a CPP program in Windows following are the command lines:

```cpp
Compile: gcc Filename.cpp 
Run or execute: filename
```

## **Macros and Comments in C++**

### **Macros in C++**

* Macros are a piece of code in a program that is given some name.
    
* Whenever the compiler encounters this name, the compiler replaces the name with the actual piece of code.
    
* The '#define' directive is used to define a macro.
    
* Note: There is no semicolon(:) at the end of the macro definition.
    

```cpp
#include <iostream>
using names pace std;
//macro definition
#define LIMIT 5

int main() {
    for (int i 0; i < LIMIT; i++) {
        cout << i <<" ";
    }
    return 0;
}
/*    Output:
      e1 2 3 4     */
```

**Macros with arguments:**

* We can also pass arguments to macros.
    
* Macros defined with arguments work similarly as functions. Example:
    

```cpp
#include 
using namespace Std;
// macrO wth parameter 
#define Area(l, b)(* b) 
int main() {
    int l = 10, b =5, a;
    a = Area(1, b); 
    cout << "The Area of the rectangle is: " << a; 
    return 0;
}
/*    Output:
      The area of the rectangle is: 50    */
```

### **Comments in C++**

* C++ comments are hints that a programmer can add to make their code easier to read and understand.
    
* They are completely ignored by C++ compilers.
    

There are two ways to add comments to code:

* // - Single Line Comment
    
* /\* \*/ - Multi-line Comments
    

Example: Single-line comment

```cpp
 #include <iostream>
using namespace std;
int main() {
    // This is a comment 
    cout << "Hello World! "; 
    return 0;
}

/*    Output:
      Hello World    */
```

Example: Multi-line comment

```cpp
 #include <iostream>
using namespace std;
int main() {
    /* This is a comment will print
    Hello World*/
    cout << "Hello World! "; 
    return 0;
}

/*    Output:
      Hello World    */
```

If you have read this far... Do not forget to stay tuned for Part 2 of this series.  
Thank you for reading 👋
