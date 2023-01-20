# Variables and Data Types in C++

## Introduction to Variables

* A variable is a storage place that has some memory allocated to it. It is used to store some form of data.
    
* Different types of variables require different amounts of memory.
    

### **Variable Declaration**

In C++, we can declare variables as follows:

* data\_type: Type of the data that can be stored in this variable. It can be int, float, double, etc.
    
* variable\_name: Name given to the variable.
    

```cpp
data_type variable_name; 

Example: int x;
```

In this way, we can only create a variable in the memory location. Currently, it doesn’t have any value. We can assign the value in this variable by using two ways:

* By using variable initialization.
    
* By taking input
    

Here, we can discuss only the first way, i.e., variable initialization. We will discuss the second way later.

```cpp
data_type variable_name=value; 

Example: int x = 20;
```

Rules for defining variables in C++

* You can’t begin with a number. Ex- 9a can't be a variable, but a9 can be a variable.
    
* Spaces and special characters except for underscore(\_) are not allowed.
    
* C++ keywords (reserved words) must not be used as a variable name.
    
* C++ is case-sensitive, meaning a variable with the name ‘A’ is different from a variable with the name ‘a. (Difference in the upper-case and lower-case holds true).
    

### **C++ Keywords**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673759283293/9f19b65a-f06d-4376-900c-e92938bf5f92.png align="left")

## Introduction to Data Types

All variables use data type during declaration to restrict the type of data to be stored.

Therefore, we can say that data types tell the variables the type of data they can store.

Pre-defined data types available in C++ are:

* int: Integer value
    
* unsigned int: Can store only positive integers
    
* float, double: Decimal number
    
* char: Character values (including special characters)
    
* unsigned char: Character values
    
* bool: Boolean values (true or false)
    
* long: Contains integer values but with the larger size
    
* unsigned long: Contains large positive integers or 0
    
* short: Contains integer values but with smaller size
    

### Table for datatype and its size in C++:

(This can vary from compiler to compiler and system to system depending on the version you are using)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673759737356/f0e58669-ddc0-48ae-8ebd-cdcdd39e7463.png align="center")

Examples:

```cpp
int price = 5000;// Integer (whole number)

float interestRate = 5.99f; // Floating point number

char myLetter = 'D'; // Character

bool isPossible = true; // Boolean 

string myText = "Coding Ninjas"; // String
```

### auto keyword in c++

* The auto keyword specifies that the type of the declared variable will automatically be deduced from its initializer.
    
* It would set the variable type to initialize that variable’s value type or set the function return type as the value to be returned.
    

Example:

```cpp
auto a = 11 // will set the variable as int type

auto b = 7.65 //will set the variable b as a float 

auto c = "abcdefg" // will set the variable c as string
```

## Scope of Variables

* The scope of a variable refers to the region of visibility or availability of a variable i.e the parts of your program in which the variable can be used or accessed.
    
* There are mainly two types of variable scopes: **Local Scope and Global Scope**
    

### **Local Scope**

* Variables declared within the body of a function or block are said to have local scope and are referred to as local variables.
    
* They can be used only by the statements inside the body of the function or the block they are declared within. Example:
    
    ```cpp
    void person () { 
    string gender = "Male"; 
    //This variable gender is Local to the function person () 
    //and cannot be used outside this function.
    }
    ```
    

### **Global Scope**

* The variables whose scope is not limited to any block or function are said to have global scope and are referred to as 'global variables.
    
* Global variables are declared outside of all the functions, generally on the top of the program, and can be accessed from any part of your program.
    
* These variables hold their values throughout the lifetime of the program. Example:
    

```cpp
#include <iostream> 
using namespace std; 
// Global variable declaration: and can be used anywhere in code 
int g;
int main() {
    g=10; // Using global variable 
    cout << g;
    return 0;
}
```

## Types of Variables, Overflow and Underflow

There are three types of variables based on the scope of the variable in C++ -

* Local Variables
    
* Instance Variables
    
* Static Variables
    

### Local Variables

* The variables declared within the body of a function or block are known as local variables and are created(occupy memory) when the program enters the block or makes a function call.
    
* The local variables get destroyed(memory is released) after exiting from the block or returning from the function call.
    
* They can be used only by the statements inside the body of the function or the block they are declared within. Example:
    

```cpp
void function () { 
//Local variable marks 
int marks = 90; 
marks = marks + 2;
cout << "Student obtained "<<marks<< "marks. "
return; 
}
Output: Student obtained 92 marks. 
```

### Instance variables

* Instance variables are non-static variables that belong to an instance of a class and are declared in a class outside any method, constructor, or block.
    
* These variables are created when an object of the class is created and destroyed when the object is destroyed and are accessible to all the constructors, methods, or blocks in the class.
    
* Each object of the class within which the instance variable is declared will have its separate copy or instance of this variable.
    
* Unlike local variables, we may use access specifiers for instance variables. Example:
    

```cpp
class A { 
    int a; // by default private instance variables 
    int b; 
    public:
        int c; // public instance variable 
    Void function () { 
        a 10; 
        cout << a;
    }
};
```

### Static Variables

* Static variables are declared using the keyword 'static, within a class outside any method, constructor, or block.
    
* Space is allocated only once for static variables i.e we have a single copy of the static variable corresponding to a class, unlike instance variables.
    
* The static variables are created at the start of the program and get destroyed at the end of the program ie the lifetime of a static variable is the lifetime of the program.
    
* Static variables are initialized only once and they hold their value throughout the lifetime of the program. Example:
    

```cpp
class A { 
    static int var; //static variable 
    Void func() { 
        ++var;
    }
};
```

### Overflow and Underflow

* Overflow occurs when we assign a value to more than its range, and Underflow is the opposite of overflow.
    
* In the case of overflow and underflow, the C++ compiler doesn't throw any errors.
    
* It simply changes the value.
    
* For example, in the case of an int variable, the maximum value of the int data type is 2,147,483,647 (NT MAX) and after incrementing 1 on this value, it will return -2,147,483,648 (INTMIN). This is known as overflow.
    
* The minimum value of the int data type is -2,147,483,648 (INT MIN) and after decrementing 1 on this value, it will return 2,147,483,647 (INT MAX). This is known as underflow. Example:
    

```cpp
#include <iostream> 
using namespace std; 
int main() { 
    int x = INT_MAX; //2147483647 
    int y = INT_MIN; //-2147483648 
    x = X + 1; 
    y =y- 1; 
    cout < x << endl; 
    cout < y;
}
Output: 
-2147483648 
2147483647
```

## Typecasting

Converting an expression of a given data type into another data type is known as type-casting or type-conversion.

There are two types of type conversions:  
\- Implicit Type Conversion  
\- Explicit Type Conversion

### Implicit Type Conversion

* It is automatically performed by the compiler itself to ensure that the calculations between the same data types take place and avoid any loss of data.
    
* Such types of conversions take place when more than one data type is present in an expression.
    
* The rule associated with implicit type conversions involves upgrading the data type of all the variables to the data type of the variable with the "largest data type".
    
* The order of automatic type conversion or the sequence for smallest to largest data type(left to right) for this type conversion is given as:  
    **bool-&gt; char -&gt; short int -&gt; int -&gt; unsigned int -&gt; long -&gt; unsigned-&gt; long long -&gt; float-&gt; double -&gt; long double**
    
* Example:
    
    ```cpp
    #include <iostream> 
    using namespace std; 
    int main() { 
        int number = 200;  
        char letter = 'c'; 
        float dec = 0.7;
        int res1 = number + letter; // here Letter is implicitly converted to int and its va // ASCII value of c i.e. 99 
        cout << res1 << " "; 
        float res2 = res1 + dec; // here resi is implicitly converted to float. 
        cout < res2; 
    }
    Output: 299 299.7 
    ```
    

### Explicit Type Conversion:

* This process is also called typecasting, and it is user-defined.
    
* Here the user can typecast the result to make it of a particular data type which may lead to data loss and is also known as forceful casting.
    
* Syntax:
    
    ```cpp
    (type) expression 
    Example: 
    int main() { 
        double dbl = 5.6; 
        int res = (int)dbl + 10; // Here dbl is explicity con verted to int i.e value of dbl becomes 5. 
        cout <<"Result = " << res;
    }
    ```
