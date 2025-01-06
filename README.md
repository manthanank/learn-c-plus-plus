# Learn C++

### **C++ Introduction**

C++ is a general-purpose programming language developed by Bjarne Stroustrup. It is an extension of the C language with object-oriented features, making it suitable for system-level programming, game development, and applications requiring high performance.

**Key Features**

- Object-Oriented Programming (OOP)
- Standard Template Library (STL)
- Memory Management (pointers, dynamic allocation)
- Multi-paradigm (procedural, functional, object-oriented)

### **IDE (Integrated Development Environment)**

An IDE is a software application that provides comprehensive facilities for software development. Popular IDEs for C++ include:
- Visual Studio Code
- Code::Blocks
- Eclipse
- JetBrains CLion

**Features**

- Code Editor
- Debugger
- Compiler Integration
- IntelliSense (code suggestions)

### **Compiler**

A compiler translates human-readable C++ code into machine code. Popular C++ compilers:
- GCC (GNU Compiler Collection)
- Clang
- Microsoft Visual C++ Compiler

### **Downloading Visual Studio Code**

Visual Studio Code is a lightweight, powerful code editor with extensive extensions for C++ programming.

**Steps to Download**

1. Visit the [official website](https://code.visualstudio.com/).
2. Download the version appropriate for your operating system.
3. Install the downloaded file.

### **Downloading, Installing & Configuring Compiler**

**Steps**

1. Download GCC using **MinGW** or a similar tool.
   - For Windows, use [MinGW-w64](http://mingw-w64.org/doku.php).
2. Install MinGW and add its `bin` directory to the system `PATH`.
3. Test installation by typing `g++ --version` in the terminal.

### **Installing VS Code**

1. Open the VS Code installer and follow the on-screen instructions.
2. Install the **C/C++ extension** from the Extensions Marketplace.
3. Configure the `tasks.json` and `launch.json` files for building and debugging.

### **Basics of VS Code**

- **Explorer**: View and manage project files.
- **Editor**: Write and edit code.
- **Terminal**: Execute commands.
- **Extensions**: Add new features like IntelliSense and debugging tools.

### **Writing First C++ Program**

**Code**

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
```

**Steps**

1. Open a new file in VS Code.
2. Save it with a `.cpp` extension.
3. Compile using `g++ filename.cpp -o filename`.
4. Run the executable using `./filename`.

### **Understanding First Program**

- **`#include <iostream>`**: Includes the library for input/output.
- **`using namespace std;`**: Avoids prefixing standard library functions with `std::`.
- **`int main()`**: Entry point of the program.
- **`cout`**: Outputs text to the console.
- **`return 0;`**: Indicates successful program termination.

### **Comments**

- **Single-line comment**: `// This is a comment`
- **Multi-line comment**:

```cpp
/* This is
   a multi-line
   comment */
```

### **Data Types in C++**

**Primitive Types**

- `int`, `float`, `double`, `char`, `bool`

**Derived Types**:

- Arrays, Functions, Pointers
**User-defined Types**:
- Structures, Classes, Enums

### **Variables**

A variable is a container for storing data.

**Syntax**

```cpp
int number = 10;
float pi = 3.14;
char grade = 'A';
```

### **Taking User Input**

**Code**

```cpp
#include <iostream>
using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;
    cout << "Your age is " << age << endl;
    return 0;
}
```

### **Operators**
1. **Arithmetic**: `+`, `-`, `*`, `/`, `%`
2. **Relational**: `==`, `!=`, `>`, `<`, `>=`, `<=`
3. **Logical**: `&&`, `||`, `!`

### **If-Else Statements**

**Code**

```cpp
if (condition) {
    // code block
} else {
    // code block
}
```

### **Switch Statement**

**Code**

```cpp
switch (variable) {
    case value1:
        // code block
        break;
    case value2:
        // code block
        break;
    default:
        // code block
}
```

### **Loops**

1. **For Loop**

```cpp
for (int i = 0; i < 5; i++) {
    cout << i << endl;
}
```

2. **While Loop**

```cpp
while (condition) {
    // code block
}
```

3. **Do-While Loop**

```cpp
do {
    // code block
} while (condition);
```

### **Functions**

**Syntax**

```cpp
returnType functionName(parameters) {
    // code block
    return value;
}
```

### **Arrays**

An array stores multiple values of the same type.

```cpp
int arr[5] = {1, 2, 3, 4, 5};
```

### **Typecasting**

Converting one data type to another.

```cpp
float num = 10.5;
int integer = (int)num;
```

### **Strings**

Strings are objects in C++.

```cpp
#include <string>
string str = "Hello";
```

### **Pointers**

A pointer stores the address of a variable.

```cpp
int var = 10;
int* ptr = &var;
```

### **Objects & Classes**

C++ is object-oriented, using **classes** and **objects**.

**Class**

```cpp
class Car {
public:
    string brand;
    void display() {
        cout << brand;
    }
};
```

**Object**

```cpp
Car car1;
car1.brand = "Toyota";
car1.display();
```

### **Constructor**

Special method called when an object is created.

```cpp
class Car {
public:
    string brand;
    Car(string b) {
        brand = b;
    }
};
```

### **Inheritance**

A way to derive one class from another.

```cpp
class Parent {
public:
    void display() {
        cout << "Parent Class";
    }
};

class Child : public Parent {
};
```
