## **Core Java**

- [Features of Java?](#q1-features-of-java)
- [What is a Compiler?](#q2-what-is-a-compiler)
- [Classes and Objects in Java?](#q3-classes-and-objects-in-java)
- [wrapper classes classes Java?](#q4-wrapper-classes-classes-java)

## Short Tips Vault

```
Local variables are destroyed after the method ends.
Instance variables exist as long as the object exists.
Static variables exist throughout the program's lifecycle and are shared among all instances.
```

```
Widening (Implicit) Casting: Happens automatically when there’s no risk of data loss.
Narrowing (Explicit) Casting: Requires manual casting, might lead to data loss.
```

```
final: Indicates that the variable's value cannot be changed once initialized. It behaves like a constant.

static: Indicates the variable belongs to the class, not to any specific object. It can be accessed directly using the class name.
```

---

## Q1: Features of Java

1. **Object-Oriented**  
   Java is an object-oriented programming language that supports encapsulation, inheritance, and polymorphism.

2. **Platform-Independent**  
   Java code can run on any platform with a Java Virtual Machine (JVM) installed, embodying the principle of “write once, run anywhere.”

3. **Simple and Easy to Learn**  
   Java’s syntax is similar to C and C++, making it easier for developers to learn and use.

4. **Robust Security**  
   Java includes built-in security features such as bytecode verification, secure class loading, and a robust security manager, making it ideal for building secure applications.

5. **Multithreading**  
   Java supports multithreading, enabling the execution of multiple threads simultaneously to improve performance and responsiveness.

6. **Automatic Memory Management**  
   Java provides automatic garbage collection, freeing developers from manual memory management and reducing the risk of memory leaks.

7. **Dynamic Loading of Classes**  
   Java allows for the dynamic loading of classes, making applications more flexible and modular.

8. **Extensive Libraries and APIs**  
   Java offers a wide range of libraries and APIs, including the Java Standard Edition (SE) and Enterprise Edition (EE) APIs, suitable for diverse applications.

9. **High-Performance**  
   Java achieves high performance through Just-In-Time (JIT) compilation and runtime optimizations.

10. **Garbage Collection**  
    Java’s garbage collector periodically frees unused memory, reducing the need for manual memory management and minimizing memory-related errors.

11. **Encapsulation**  
    Java enables developers to hide implementation details and expose only the necessary information, promoting code reuse and modularity.

12. **Inheritance**  
    Java’s inheritance feature allows the creation of a hierarchy of classes, encouraging code reuse and better organization.

---

---

## Q2: reserved keywords in Java ?

Java has a total of **53 reserved keywords** as of Java SE 17. These are predefined words in the language that have special meanings and cannot be used as identifiers (e.g., variable names, method names). Aside from `void`, these keywords are categorized as follows:

### 1. **Control Flow Keywords** (12)

These keywords control the flow of execution in a program:

- `if`, `else`
- `switch`, `case`, `default`
- `for`, `while`, `do`
- `break`, `continue`
- `return`

### 2. **Data Type Keywords** (8)

Used to define variable data types:

- Primitive types: `int`, `float`, `double`, `char`, `boolean`, `byte`, `short`, `long`

### 3. **Access Modifiers** (4)

Define access control for classes, methods, and variables:

- `private`, `protected`, `public`, `default` (implied when no modifier is used)

### 4. **Class, Object, and Inheritance Keywords** (6)

Used for defining and managing classes and objects:

- `class`, `interface`
- `extends`, `implements`
- `this`, `super`

### 5. **Exception Handling Keywords** (6)

For managing exceptions and errors:

- `try`, `catch`, `finally`
- `throw`, `throws`
- `assert`

### 6. **Modifiers** (11)

Used to define properties of classes, methods, and variables:

- `static`, `final`, `abstract`, `synchronized`
- `volatile`, `transient`, `native`, `strictfp`
- `sealed`, `non-sealed`, `permits` (introduced in Java 17 for sealed classes)

### 7. **Package-Related Keywords** (2)

For organizing classes:

- `package`, `import`

### 8. **Boolean Literals** (2)

Used to define logical values:

- `true`, `false`

### 9. **Null Literal** (1)

Represents a null reference:

- `null`

### 10. **Instance-Related Keywords** (2)

Used to check or create objects:

- `new`, `instanceof`

### 11. **Miscellaneous Keywords** (2)

Used for more advanced functionality:

- `enum`, `record`

### 12. **Unutilized Reserved Keywords** (2)

Reserved for future use (not currently functional in Java):

- `goto`, `const`

### Total:

Excluding `void`, there are **52 other keywords** in Java. These keywords form the foundation of Java's syntax and features.

---

---

## Q3: Difference between a **compiler** and an **interpreter**

The real difference between a **compiler** and an **interpreter** lies in how they translate and execute source code. Here's a breakdown:

### **Compiler**

1. **Translation**: A compiler translates the entire source code of a program into machine code (binary) before the program is executed.
2. **Output**: Produces an executable file (e.g., `.exe`) that can be run independently of the source code or compiler.
3. **Execution**: The program is executed directly by the machine, using the compiled binary code.
4. **Performance**: Compiled programs usually run faster since the translation happens only once, and the machine directly executes the binary code.
5. **Error Handling**: Reports errors all at once after the compilation process, which means you must fix errors before running the program.
6. **Examples**: C, C++, Rust, Go.

### **Interpreter**

1. **Translation**: An interpreter translates source code into machine code line-by-line or statement-by-statement during execution.
2. **Output**: Does not produce an independent executable file . The source code must be interpreted every time it runs.
3. **Execution**: Executes code immediately, making it ideal for scripting and testing.
4. **Performance**: Interpreted programs tend to run slower because the translation happens dynamically during execution.
5. **Error Handling**: Stops execution as soon as it encounters an error, making it easier to debug specific issues in the code.
6. **Examples**: Python, JavaScript, Ruby.

### Key Differences in Detail

| Aspect                 | **Compiler**                  | **Interpreter**                |
| ---------------------- | ----------------------------- | ------------------------------ |
| **Translation Timing** | Before execution              | During execution               |
| **Execution Speed**    | Faster (precompiled)          | Slower (real-time translation) |
| **Output**             | Produces executable binary    | Does not produce a binary file |
| **Error Reporting**    | All errors at once            | Errors reported one-by-one     |
| **Use Case**           | High-performance applications | Rapid prototyping, scripting   |

### Hybrid Approach

Some languages, like Java, use both a compiler and an interpreter:

- Java source code is **compiled** into bytecode (intermediate form).
- The bytecode is then **interpreted** by the Java Virtual Machine (JVM) during execution.

### Conclusion

- **Compilers** are better suited for performance-critical applications where speed and efficiency matter.
- **Interpreters** excel in environments requiring flexibility, quick iterations, or simplicity.

---

---

## Q4: Stack and Heap Memory management in Java

### **Stack and Heap in Java**

In Java, memory is managed in two primary areas:

1. **Stack**: Used for storing local variables, method calls, and references to objects.
2. **Heap**: Used for storing objects and arrays created dynamically at runtime.

---

### **1. Stack Memory**

- **Purpose**: The stack is used to store method calls and local variables. Each thread in a Java application has its own stack.
- **Memory Structure**:

  - It is organized as a Last In, First Out (LIFO) structure.
  - Every time a method is invoked, a new stack frame is created. This frame stores the local variables, parameters, and the reference to the method's return address.
  - Once the method finishes executing, the stack frame is popped off the stack.

- **Characteristics**:

  - **Fast Access**: Since stack memory operates in a LIFO manner, it allows for fast access and memory allocation.
  - **Limited Size**: Stack memory is limited in size, and excessive recursion or deep method calls can result in a **stack overflow**.
  - **Automatic Memory Management**: Local variables are automatically removed when the method scope ends.
  - **Primitive Data Types**: Local primitive variables like `int`, `char`, and `boolean` are stored in the stack.
  - **References to Objects**: References to objects (but not the objects themselves) are stored in the stack.

- **Example**:

  ```java
  public class StackExample {
      public static void main(String[] args) {
          int a = 10;  // Stored in stack
          String str = "Hello";  // Reference to the string object in the heap
          printSum(a);
      }

      static void printSum(int number) {  // Local variable 'number' stored in stack
          System.out.println(number + 10);
      }
  }
  ```

  In the above code, `a` and `str` are stored in the stack, while the actual string `"Hello"` is stored in the heap.

---

### **2. Heap Memory**

- **Purpose**: The heap is used to store objects and arrays dynamically created during the execution of a program.
- **Memory Structure**:

  - The heap is where objects created using the `new` keyword (e.g., objects, arrays) are allocated memory.
  - The **Garbage Collector** (GC) automatically frees up memory in the heap by removing objects that are no longer in use (i.e., unreachable objects).

- **Characteristics**:

  - **Dynamic Memory Allocation**: Objects and arrays are created dynamically, and memory is allocated at runtime.
  - **Larger Memory Size**: Heap memory is much larger than stack memory and can grow as needed (depending on JVM settings).
  - **Slower Access**: Since objects in the heap are accessed through references, accessing them is slower compared to accessing stack variables.
  - **Garbage Collection**: Objects in the heap are cleaned up automatically by Java’s garbage collector when they are no longer referenced.

- **Example**:

  ```java
  public class HeapExample {
      public static void main(String[] args) {
          // Object creation in heap
          Person person = new Person("John", 25);
          System.out.println(person.name);
      }
  }

  class Person {
      String name;
      int age;

      // Constructor
      public Person(String name, int age) {
          this.name = name;
          this.age = age;
      }
  }
  ```

  Here, the `Person` object is stored in the heap, while the reference `person` is stored in the stack.

---

### **Comparison of Stack and Heap**

| Feature               | **Stack**                                                  | **Heap**                              |
| --------------------- | ---------------------------------------------------------- | ------------------------------------- |
| **Purpose**           | Stores method calls and local variables                    | Stores objects and arrays             |
| **Memory Allocation** | Static and automatic                                       | Dynamic and managed by GC             |
| **Size**              | Small and limited                                          | Larger and can grow                   |
| **Access Speed**      | Fast (LIFO)                                                | Slower (indirect reference access)    |
| **Lifetime**          | Until the method call is finished                          | Until the object is garbage collected |
| **Memory Management** | Managed by the compiler (automatic)                        | Managed by the garbage collector      |
| **Objects**           | No objects, only primitive types and references to objects | Objects and arrays are stored here    |
| **Example**           | Local variables, method arguments                          | Objects created with `new` keyword    |

---

### **Key Differences Between Stack and Heap**

1. **Storage**:
   - **Stack** stores **primitive data types** and **method calls**, while **Heap** stores **objects** and **arrays**.
2. **Size**:
   - **Stack** memory is smaller and has a fixed size, while **Heap** memory is larger and grows dynamically.
3. **Access Speed**:

   - **Stack** memory is faster to access because it operates in a **LIFO** manner, whereas **Heap** memory is slower due to indirect referencing.

4. **Garbage Collection**:

   - **Stack** memory does not need garbage collection because the data is automatically removed when a method finishes executing.
   - **Heap** memory requires **Garbage Collection** (GC) to clean up objects that are no longer referenced.

5. **Lifetime**:
   - **Stack** data exists only during the method call's lifetime.
   - **Heap** data exists until it is no longer referenced and is garbage collected.

---

### **Example of Stack and Heap in Action**

```java
public class MemoryExample {
    public static void main(String[] args) {
        int x = 10;  // Stack
        int y = 20;  // Stack

        // Object creation in heap
        Person p1 = new Person("Alice", 30);  // Heap
        p1 = new Person("Bob", 25);  // New object created in Heap

        // Array creation in heap
        int[] numbers = new int[5];  // Heap
        numbers[0] = 1;  // Stack stores reference to the array in Heap
    }
}

class Person {
    String name;  // Stored in heap
    int age;      // Stored in heap

    public Person(String name, int age) {
        this.name = name;  // Reference to string object stored in heap
        this.age = age;
    }
}
```

In this example:

- **`x` and `y`** are stored in the **stack**.
- **`p1`** is a reference variable stored in the **stack**, but the actual `Person` object is in the **heap**.
- The **array `numbers`** is created in the **heap**, but the reference to the array is stored in the **stack**.

---

### **Conclusion**

- **Stack** is used for storing temporary data (local variables, method calls) and is limited in size.
- **Heap** is used for dynamically created objects and arrays and has a larger and more flexible memory space.
- Understanding how stack and heap memory work is essential for optimizing memory usage and preventing issues like **stack overflow** or **memory leaks**.

---

---

## Q5: Mutable vs Immutable String in Java

### **Mutable vs Immutable String in Java**

In Java, strings can be classified as **immutable** and **mutable**. The key difference lies in how the string objects behave after creation.

#### **1. Immutable String**

- **Definition**: An **immutable string** is an object whose value cannot be changed once it is created. In Java, the `String` class is **immutable**.
- **Characteristics**:

  - When you modify a string, a new string object is created, and the old string remains unchanged.
  - Any operation on a string like concatenation, replacement, or substring creates a new `String` object.
  - This ensures **thread-safety** and **security** as the string’s state cannot be modified once created.

- **Example**:

  ```java
  public class ImmutableStringExample {
      public static void main(String[] args) {
          String str = "Hello";
          System.out.println("Original String: " + str);

          // Modifying the string (This creates a new string object)
          str = str.concat(" World");
          System.out.println("Modified String: " + str);
      }
  }
  ```

  **Output**:

  ```
  Original String: Hello
  Modified String: Hello World
  ```

  - **Explanation**: In the example, `str.concat(" World")` does not modify the original string. Instead, it creates a new string `"Hello World"`. The original string `"Hello"` remains unchanged.

- **Why is String Immutable?**
  - **Security**: Strings are widely used in applications like URL, file paths, database connections, etc. If they were mutable, their values could change unexpectedly, leading to security issues.
  - **Hashing**: Since strings are used as keys in hash-based collections (like `HashMap`), immutability guarantees that the hash code of the string does not change over time.

---

#### **2. Mutable String**

- **Definition**: A **mutable string** is an object whose value can be modified after it is created. In Java, `StringBuilder` and `StringBuffer` classes are **mutable**.
- **Characteristics**:

  - These classes allow you to modify the string's content (such as appending or deleting characters) without creating new objects every time.
  - **StringBuilder** is not thread-safe but faster for single-threaded use, while **StringBuffer** is thread-safe but slower due to synchronization.
  - Mutable strings are more efficient when performing many string manipulations in loops, as they do not require creating new objects for each modification.

- **Example using `StringBuilder`**:

  ```java
  public class MutableStringExample {
      public static void main(String[] args) {
          StringBuilder sb = new StringBuilder("Hello");
          System.out.println("Original StringBuilder: " + sb);

          // Modifying the string
          sb.append(" World");
          System.out.println("Modified StringBuilder: " + sb);
      }
  }
  ```

  **Output**:

  ```
  Original StringBuilder: Hello
  Modified StringBuilder: Hello World
  ```

  - **Explanation**: In the example, `sb.append(" World")` modifies the existing `StringBuilder` object without creating a new one. The string is mutable, and its value changes in-place.

- **Advantages of Mutable Strings (`StringBuilder`/`StringBuffer`)**:
  - **Efficiency**: Since `StringBuilder` and `StringBuffer` don’t create new objects, they are more memory-efficient and faster when performing frequent modifications.
  - **Performance**: Useful in loops or when concatenating strings in many operations.

---

### **Key Differences Between Mutable and Immutable Strings**

| Feature           | **Immutable String** (`String`)                 | **Mutable String** (`StringBuilder`/`StringBuffer`)                   |
| ----------------- | ----------------------------------------------- | --------------------------------------------------------------------- |
| **Mutability**    | Cannot be changed after creation                | Can be modified after creation                                        |
| **Classes**       | `String`                                        | `StringBuilder`, `StringBuffer`                                       |
| **Memory**        | New object created for each modification        | Same object is modified in place                                      |
| **Thread Safety** | Thread-safe (since it's immutable)              | `StringBuffer` is thread-safe, `StringBuilder` is not                 |
| **Performance**   | Slower for frequent modifications               | Faster for frequent modifications                                     |
| **Use Case**      | When the string is not modified often           | When the string is modified frequently (e.g., in loops)               |
| **Example**       | `"Hello".concat(" World")` creates a new string | `StringBuilder sb = new StringBuilder("Hello"); sb.append(" World");` |

---

### **When to Use Immutable vs Mutable Strings**

1. **Use Immutable Strings** (`String`):

   - When string content does not need to be changed frequently.
   - When working with **hash-based collections** (`HashMap`, `HashSet`), since the immutability guarantees that the hash code does not change.
   - In multi-threaded applications where thread safety is critical.

2. **Use Mutable Strings** (`StringBuilder` or `StringBuffer`):
   - When performing many modifications or concatenations on strings (e.g., inside loops or when building large strings).
   - In performance-critical sections where the overhead of creating new string objects every time is inefficient.

---

### **Conclusion**

- **Immutable strings** (`String`) are safe, thread-friendly, and commonly used in scenarios where string values don’t change often.
- **Mutable strings** (`StringBuilder`/`StringBuffer`) are more performance-efficient when strings undergo frequent modifications.
- Understanding when to use **String** and when to use **StringBuilder** or **StringBuffer** can significantly improve performance in Java applications.

---

---

## Q3: Instance Variables in Java?

### **Instance Variables (Non-Static Fields) in Java**

Instance variables are **non-static fields** that are defined within a class but outside of any method, constructor, or block. These variables are called **instance variables** because their values are unique to each instance (or object) of the class.

### **Key Characteristics of Instance Variables**

1. **Declared at the Class Level**:

   - Instance variables are declared directly within a class but outside any methods, constructors, or blocks.

2. **Belong to an Instance**:

   - Each object (instance) of the class has its own copy of the instance variables. Changes to these variables in one object do not affect others.

3. **Default Values**:

   - If not explicitly initialized, instance variables are assigned default values:
     - `int` → `0`
     - `double` → `0.0`
     - `boolean` → `false`
     - `char` → `\u0000` (null character)
     - Object references → `null`

4. **Access Modifiers**:

   - Instance variables can be declared with access modifiers (`private`, `protected`, `public`, or default) to control their visibility.

5. **Accessed via Objects**:
   - You need an object of the class to access or modify instance variables.

### **Example of Instance Variables**

```java
class Person {
    // Instance variables
    String name; // Default value is null
    int age;     // Default value is 0

    // Constructor
    Person(String name, int age) {
        this.name = name; // Assign value to instance variable
        this.age = age;
    }

    // Method to display person details
    void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

public class Main {
    public static void main(String[] args) {
        // Creating objects of the Person class
        Person person1 = new Person("Alice", 25);
        Person person2 = new Person("Bob", 30);

        // Accessing instance variables via objects
        person1.displayInfo();
        person2.displayInfo();

        // Modifying instance variable for one object
        person1.age = 26;
        System.out.println(person1.name + "'s updated age: " + person1.age);
    }
}
```

### **Output**

```
Name: Alice
Age: 25
Name: Bob
Age: 30
Alice's updated age: 26
```

### **How Instance Variables Work**

1. **Separate Copies for Each Object**:

   - Each object gets its own copy of the instance variables (`name` and `age` in this case). Changing these values for one object does not affect the others.

2. **`this` Keyword**:
   - The `this` keyword is used to differentiate between instance variables and parameters with the same name in constructors or methods.

### **Memory Management**

- **Instance variables** are stored in the **heap memory** because each object resides in the heap. The lifecycle of instance variables is tied to the lifecycle of the object they belong to.

### **Common Use Case**

Instance variables are used when you want data to be associated with an object. For example, in a class `Car`, instance variables like `color`, `brand`, and `speed` can store details specific to each car object.

---

---

## Q4: Class Variables in Java?

### **Class Variables (Static Fields) in Java**

Class variables, also known as **static fields**, are variables declared using the `static` keyword inside a class, but outside any method, constructor, or block. These variables belong to the **class itself**, not to any specific object of the class.

### **Key Characteristics of Class Variables**

1. **Shared Across All Instances**:

   - Class variables are shared by all objects of the class. If one object modifies a class variable, the change is reflected for all other objects.

2. **Declared with `static`**:

   - The `static` keyword is used to define class variables.

3. **Stored in Class Memory**:

   - Class variables are stored in the **method area** of memory, rather than the heap where instance variables are stored.

4. **Default Values**:

   - If not explicitly initialized, class variables are assigned default values, just like instance variables:
     - `int` → `0`
     - `double` → `0.0`
     - `boolean` → `false`
     - `char` → `\u0000` (null character)
     - Object references → `null`

5. **Access Without Objects**:

   - Class variables can be accessed directly using the class name (`ClassName.variableName`) or via an object reference, though using the class name is recommended.

6. **Scope**:
   - Class variables are accessible to all methods, constructors, and blocks of the class, but their visibility can be controlled using access modifiers (`public`, `private`, `protected`).

### **Example of Class Variables**

```java
class Counter {
    // Class variable (static field)
    static int count = 0; // Shared by all objects

    // Instance variable
    String name;

    // Constructor
    Counter(String name) {
        this.name = name;
        count++; // Increment the static count variable
    }

    // Method to display information
    void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Total Objects: " + count); // Accessing static field
    }
}

public class Main {
    public static void main(String[] args) {
        // Creating objects of Counter class
        Counter obj1 = new Counter("Object 1");
        Counter obj2 = new Counter("Object 2");
        Counter obj3 = new Counter("Object 3");

        // Displaying information for each object
        obj1.displayInfo();
        obj2.displayInfo();
        obj3.displayInfo();

        // Accessing the static variable using the class name
        System.out.println("Final Count: " + Counter.count);
    }
}
```

### **Output**

```
Name: Object 1
Total Objects: 1
Name: Object 2
Total Objects: 2
Name: Object 3
Total Objects: 3
Final Count: 3
```

### **How Class Variables Work**

1. **Single Copy in Memory**:

   - Only one copy of a class variable exists, regardless of how many objects of the class are created.

2. **Shared State**:

   - Modifications to a class variable affect its value across all objects of the class.

3. **Access Using Class Name**:
   - It is a good practice to access class variables using the class name (`ClassName.variableName`), making it clear that the variable is shared.

### **Usage of Class Variables**

Class variables are typically used for:

- **Constants**:

  ```java
  public class MathConstants {
      public static final double PI = 3.14159; // Shared constant
  }
  ```

  Access: `MathConstants.PI`

- **Counters or Trackers**:
  To keep track of the number of objects created, as shown in the example above.

- **Global Information**:
  To store information that needs to be accessible to all objects (e.g., configuration data).

### **Difference Between Instance and Class Variables**

| **Feature**       | **Instance Variables**    | **Class Variables**       |
| ----------------- | ------------------------- | ------------------------- |
| **Keyword**       | No `static`               | Declared with `static`    |
| **Scope**         | Belongs to an object      | Belongs to the class      |
| **Memory**        | Stored in the heap memory | Stored in the method area |
| **Default Value** | Default initialized       | Default initialized       |
| **Access**        | Via object references     | Via class name or object  |
| **Shared**        | Unique to each object     | Shared by all objects     |

---

---

## Q2: What is a Compiler?

A **compiler** is a software tool that translates code written in a high-level programming language (such as Java) into machine code or an intermediate form that can be executed by a computer. In Java, the compiler converts source code (`.java` files) into an intermediate form called **bytecode** (`.class` files).

Key points about the Java Compiler:

1. The compiler ensures the source code is free from syntax errors before execution.
2. In Java, the compiler (e.g., `javac`) converts Java code into **bytecode**, which is platform-independent.

### **How JVM Works in Java**

The **Java Virtual Machine (JVM)** is the runtime environment that executes Java bytecode. It acts as an interpreter between the bytecode and the underlying hardware or operating system, enabling Java's platform independence.

Here is a step-by-step explanation of how JVM works:

#### **1. Compilation Phase**

- Source code (`.java`) → Compiled by `javac` → Bytecode (`.class`).
- Bytecode is a set of instructions that can be understood by the JVM.

#### **2. Class Loader Subsystem**

- **Class Loading:** The JVM's class loader loads the required `.class` files into memory.
- **Class Linking:** Verifies bytecode and resolves dependencies among classes.
- **Class Initialization:** Prepares static variables and runs static blocks.

#### **3. Execution Engine**

The Execution Engine is the core component of the JVM responsible for executing bytecode.

- **Interpreter:** Executes bytecode line by line, which can be slower due to repeated interpretation of frequently used code.
- **Just-In-Time (JIT) Compiler:** Converts frequently used bytecode into native machine code during runtime for faster execution.

#### **4. Memory Areas in JVM**

JVM uses several memory areas to execute applications:

- **Method Area:** Stores class metadata, static variables, and method code.
- **Heap Area:** Stores objects and their instance variables (shared among threads).
- **Stack Area:** Stores method-specific local variables and function call data (specific to each thread).
- **Program Counter Register (PC):** Keeps track of the current execution point in the bytecode.
- **Native Method Stack:** Handles native code execution.

#### **5. Garbage Collection**

- JVM manages memory automatically by identifying and freeing unused objects in the heap.

### **Execution Flow**

1. Java source code is compiled into bytecode using `javac`.
2. The JVM loads the bytecode via the **class loader**.
3. The bytecode is verified for security and correctness.
4. The **Execution Engine** interprets or compiles the bytecode to native machine code.
5. The program is executed with automatic memory management by the garbage collector.

### **Diagram of JVM Workflow**

```text
Source Code (.java)
        ↓
  Compiler (javac)
        ↓
   Bytecode (.class)
        ↓
    Class Loader
        ↓
Execution Engine → Native Machine Code → Output
 (Interpreter + JIT Compiler)
```

Would you like further details about any specific component or process?

---

---

## Q3: classes and objects in Java

### **Class in Java**

A class is a blueprint or template for creating objects (instances). It defines the properties (fields) and behaviors (methods) that the objects of that class will have. In other words, a class is a collection of attributes and methods that represent the common characteristics and behaviors of objects.

A class can contain:

- **Fields (Variables)**: These are the properties or attributes that define the state of the objects.
- **Methods**: These define the actions or behaviors that can be performed on the objects.
- **Constructors**: These are special methods used to initialize objects.
- **Access Modifiers**: These specify the visibility of fields, methods, and classes (e.g., `public`, `private`, `protected`).

#### Syntax for a Class:

```java
public class Car {
    // Fields (attributes)
    String color;
    String model;
    int year;

    // Constructor
    public Car(String color, String model, int year) {
        this.color = color;
        this.model = model;
        this.year = year;
    }

    // Method (behavior)
    public void displayDetails() {
        System.out.println("Car Model: " + model);
        System.out.println("Car Color: " + color);
        System.out.println("Car Year: " + year);
    }
}
```

### **Object in Java**

An object is an instance of a class. When you create an object from a class, the class serves as a blueprint, and the object contains the actual data for the properties defined in the class.

Each object has:

- **State**: The values of the attributes (fields).
- **Behavior**: The methods that can be called on the object.
- **Identity**: A unique reference to the object in memory.

#### Creating an Object:

You create an object by using the `new` keyword followed by the class constructor.

```java
public class Main {
    public static void main(String[] args) {
        // Creating an object of the Car class
        Car myCar = new Car("Red", "Tesla", 2024);

        // Accessing the object's methods
        myCar.displayDetails();
    }
}
```

---

### **Difference Between Class and Object**

| Feature         | **Class**                                                    | **Object**                                                     |
| --------------- | ------------------------------------------------------------ | -------------------------------------------------------------- |
| **Definition**  | A blueprint or template for objects.                         | An instance of a class.                                        |
| **Existence**   | Logical entity (does not consume memory directly).           | Physical entity (occupies memory).                             |
| **Purpose**     | Defines structure and behavior.                              | Represents a specific instance of that structure and behavior. |
| **Declaration** | Declared using the `class` keyword.                          | Created using the `new` keyword.                               |
| **Examples**    | `class Car { }`                                              | `Car myCar = new Car();`                                       |
| **Usage**       | Used to define properties and methods.                       | Used to call properties and methods defined in the class.      |
| **Number**      | One class can have many objects.                             | Each object is tied to a specific class.                       |
| **Access**      | Cannot access instance-level properties or methods directly. | Can access instance-level properties and methods.              |

---

### **Key Concepts:**

1. **Encapsulation**: This refers to the bundling of data (attributes) and methods (behaviors) that operate on the data into a single unit (the class). It also involves restricting access to some of the object's components using access modifiers like `private` or `protected` to hide implementation details.

   - Example: The `color`, `model`, and `year` attributes in the `Car` class can be encapsulated using private access modifiers, making them accessible only through getter and setter methods.

2. **Constructor**: A constructor is a special type of method used to initialize an object when it is created. It has the same name as the class and does not have a return type.

   - Example: `public Car(String color, String model, int year) { ... }` is a constructor in the `Car` class that initializes the object's state.

3. **Methods**: Methods define the behaviors of the objects. They can modify the object's state or perform actions.

   - Example: The `displayDetails()` method in the `Car` class displays the car's details.

4. **Inheritance**: A class can inherit fields and methods from another class, allowing for code reuse and extension of functionality. This is achieved using the `extends` keyword.

   - Example: If we create a `SportsCar` class that inherits from `Car`, it will automatically have the `color`, `model`, and `year` attributes, and the `displayDetails()` method.

5. **Polymorphism**: Polymorphism allows objects to be treated as instances of their parent class. The actual method that is called is determined at runtime (dynamic polymorphism) or compile time (static polymorphism).

   - Example: A `SportsCar` object can be treated as a `Car` object, and the appropriate methods for the actual object type will be called.

6. **Abstraction**: Abstract classes and interfaces are used to hide implementation details and expose only the essential features of the object. An abstract class cannot be instantiated directly.
   - Example: An abstract `Vehicle` class can define a general `move()` method, and subclasses like `Car` and `Bike` can implement it in their own way.

### **Example of Class and Object:**

```java
// Class Definition
public class Car {
    // Fields
    String color;
    String model;
    int year;

    // Constructor
    public Car(String color, String model, int year) {
        this.color = color;
        this.model = model;
        this.year = year;
    }

    // Method to display car details
    public void displayDetails() {
        System.out.println("Car Model: " + model);
        System.out.println("Car Color: " + color);
        System.out.println("Car Year: " + year);
    }
}

// Main class to create an object and use it
public class Main {
    public static void main(String[] args) {
        // Creating an object of Car class
        Car myCar = new Car("Blue", "Honda Civic", 2020);

        // Calling the method on the object
        myCar.displayDetails(); // Outputs car details
    }
}
```

### **Summary:**

- **Class**: A blueprint that defines properties and behaviors.
- **Object**: An instance of a class with specific values for properties.
- **Constructors**: Special methods used for object initialization.
- **Encapsulation, Inheritance, Polymorphism, and Abstraction**: Core OOP principles that help in building modular, reusable, and maintainable code.

---

---

## Q4: wrapper classes in Java?

In Java, **wrapper classes** are a set of classes in the `java.lang` package that provide a way to use primitive data types (like `int`, `double`, `char`, etc.) as objects. Each primitive type in Java has a corresponding wrapper class. For example:

| Primitive Type | Wrapper Class |
| -------------- | ------------- |
| `byte`         | `Byte`        |
| `short`        | `Short`       |
| `int`          | `Integer`     |
| `long`         | `Long`        |
| `float`        | `Float`       |
| `double`       | `Double`      |
| `char`         | `Character`   |
| `boolean`      | `Boolean`     |

### Why Use Wrapper Classes?

1. **Object-Oriented Context**: Some Java APIs require objects instead of primitive types. Wrapper classes help bridge this gap.
2. **Collections Framework**: Classes like `ArrayList`, `HashMap`, etc., can only store objects, not primitives.
3. **Utility Methods**: Wrapper classes provide utility methods for converting data, parsing strings, etc.

### Key Features of Wrapper Classes

1. **Autoboxing and Unboxing**:

   - **Autoboxing**: Automatic conversion of a primitive to its corresponding wrapper class object.
     ```java
     int num = 5;
     Integer obj = num;  // Autoboxing
     ```
   - **Unboxing**: Automatic conversion of a wrapper class object back to its corresponding primitive.
     ```java
     Integer obj = 10;
     int num = obj;  // Unboxing
     ```

2. **Immutability**: Wrapper class objects are immutable, meaning their values cannot be changed after they are created.

3. **Static Utility Methods**: They provide methods like `parseXxx()` to convert strings to corresponding primitives.

   ```java
   String str = "123";
   int num = Integer.parseInt(str);  // Convert string to int
   ```

4. **Constants**: Some wrapper classes have constants like `Integer.MAX_VALUE` and `Integer.MIN_VALUE`.

### Example of Using Wrapper Classes

```java
import java.util.ArrayList;

public class WrapperClassExample {
    public static void main(String[] args) {
        // Autoboxing
        ArrayList<Integer> numbers = new ArrayList<>();
        numbers.add(10);  // Autoboxing converts int to Integer

        // Unboxing
        int num = numbers.get(0);  // Unboxing converts Integer to int

        // Utility methods
        String str = "50";
        int parsedNumber = Integer.parseInt(str);  // Parsing string to int

        System.out.println("ArrayList element: " + num);
        System.out.println("Parsed number: " + parsedNumber);
    }
}
```

### When to Use Wrapper Classes?

- When working with generic classes in Java Collections.
- When primitive data needs to interact with classes or methods that require objects.
- When using features like `null` values for primitives (which is not possible without wrapper classes).

#### Wrapper classes play a crucial role in bridging the gap between Java's object-oriented features and its primitive types.

---

---

## Q5: Packages in Java ?

In Java, **packages** are used to organize classes and interfaces into namespaces, making it easier to manage and access them. They are a way to group related types (classes, interfaces, enums, and annotations) to avoid naming conflicts and improve code maintainability.

### Key Features of Packages

1. **Namespace Management**: Packages help prevent naming conflicts. For instance, two classes with the same name can exist in different packages.
2. **Access Protection**: They control access levels of classes and members. The `protected` and default (package-private) access modifiers are package-specific.
3. **Reusability**: Code in one package can be reused in another without redundancy.
4. **Categorization**: Logical grouping of classes and interfaces improves project organization and readability.
5. **Versioning**: Packages can be used to manage different versions of classes and interfaces, making
   it easier to maintain and update codebases.
6. **Dependency Management**: Packages help manage dependencies between classes and interfaces, making it easier to understand.
7. **Security**: Packages can be used to control access to classes and interfaces, improving security.
8. **Scalability**: Packages make it easier to scale large projects by organizing code into logical
   groups.
9. **Portability**: Packages make it easier to move code between projects and platforms.
10. **Readability**: Packages improve code readability by grouping related classes and interfaces together.

### Types of Packages

1. **Built-in Packages**:
   These are provided by Java, and you can use them directly.

   - Examples:
     - `java.lang` (automatically imported; contains core classes like `String`, `Math`, etc.)
     - `java.util` (utility classes like `ArrayList`, `HashMap`, etc.)
     - `java.io` (classes for input-output operations like `FileReader`, `BufferedWriter`, etc.)

2. **User-defined Packages**:
   These are created by developers to organize their project structure.

### Creating a Package

To create a package:

1. Declare it at the top of your Java file using the `package` keyword.
2. Save the file in a directory matching the package name.

#### Example:

```java
package com.example.myapp; // Declares the package

public class MyClass {
    public void displayMessage() {
        System.out.println("Hello from MyClass in com.example.myapp package!");
    }
}
```

### Using a Package

To use a class or interface from a package, you can:

1. **Fully Qualified Name**:
   ```java
   com.example.myapp.MyClass obj = new com.example.myapp.MyClass();
   ```
2. **Import Statement**:
   - Import specific classes:
     ```java
     import com.example.myapp.MyClass;
     MyClass obj = new MyClass();
     ```
   - Import all classes in a package:
     ```java
     import com.example.myapp.*;
     ```

### Package Access Modifiers

- **Public**: Accessible from any package.
- **Protected**: Accessible within the same package and by subclasses in other packages.
- **Default (no modifier)**: Accessible only within the same package.
- **Private**: Not accessible outside the class.

### Directory Structure

The directory structure should match the package name:

```
com/
  example/
    myapp/
      MyClass.java
```

When compiled, the `.class` files are placed in the same structure.

### Common Java Package Commands

1. **Compile with packages**:
   Use `-d` option to set the base directory for the package:

   ```bash
   javac -d . MyClass.java
   ```

   This places the compiled `.class` files in the appropriate directories.

2. **Run with packages**:
   Use the fully qualified class name:
   ```bash
   java com.example.myapp.MyClass
   ```

#### Packages are crucial for structuring large Java applications and managing dependencies effectively.

#### Commonly Used Built-in Packages

1. **`java.util`**: Classes like `ArrayList`, `HashMap`, `Date`, etc.
2. **`java.io`**: Classes like `File`, `BufferedReader`, `FileWriter`, etc.
3. **`java.net`**: Classes like `Socket`, `URL`, etc.
4. **`java.sql`**: Classes like `Connection`, `ResultSet`, etc.

---

---

## Q6: What is `static` in Java?

The `static` keyword in Java is used to define members (variables, methods, blocks, and nested classes) that belong to the class rather than any specific object. These members are shared across all instances of the class.

- **Static Variable**: A variable that is shared by all instances of the class.
- **Static Method**: A method that belongs to the class and can be called without creating an object of the class.
- **Static Block**: A block of code executed once when the class is loaded.
- **Static Class**: A nested class that is declared static.

### **2. Why Use `static`?**

1. **Memory Efficiency**: Shared members save memory by storing only one copy for all instances.
2. **Global Access**: Static members can be accessed without creating objects, making them convenient for utility or constant values.
3. **Class-Level Behavior**: They define behaviors or properties common to all objects of the class.
4. **Initialization Logic**: Static blocks can initialize static members or perform tasks when the class is loaded.

### **3. How to Use `static`?**

#### **Static Variables**

- Shared across all instances.
- Example:

  ```java
  class Counter {
      static int count = 0;  // Static variable

      Counter() {
          count++;
      }

      void displayCount() {
          System.out.println("Count: " + count);
      }
  }

  public class Main {
      public static void main(String[] args) {
          Counter c1 = new Counter();
          Counter c2 = new Counter();

          c1.displayCount();  // Output: Count: 2
          c2.displayCount();  // Output: Count: 2
      }
  }
  ```

#### **Static Methods**

- Called without creating an object of the class.
- Cannot access non-static members directly.
- Example:

  ```java
  class Utility {
      static int square(int num) {  // Static method
          return num * num;
      }
  }

  public class Main {
      public static void main(String[] args) {
          System.out.println("Square of 5: " + Utility.square(5));  // Output: Square of 5: 25
      }
  }
  ```

#### **Static Blocks**

- Executes once when the class is loaded.
- Used for initialization.
- Example:

  ```java
  class Demo {
      static int num;

      static {  // Static block
          num = 10;
          System.out.println("Static block executed!");
      }
  }

  public class Main {
      public static void main(String[] args) {
          System.out.println("Number: " + Demo.num);
      }
  }
  ```

#### **Static Classes**

- Only nested classes can be static.
- A static nested class can access only static members of the outer class.
- Example:

  ```java
  class OuterClass {
      static class NestedClass {  // Static nested class
          static void display() {
              System.out.println("Static nested class!");
          }
      }
  }

  public class Main {
      public static void main(String[] args) {
          OuterClass.NestedClass.display();  // Calling static nested class method
      }
  }
  ```

### **4. When to Use `static`?**

- **Static Variables**:
  - When a property should be shared across all instances (e.g., a counter, configuration values).
- **Static Methods**:
  - For utility or helper methods (e.g., `Math.max()`, `Math.sqrt()`).
  - For methods that don’t depend on object-specific data.
- **Static Blocks**:
  - When initialization logic for static members is needed (e.g., initializing a database connection).
- **Static Classes**:
  - When a nested class doesn’t require access to instance data of the outer class.

### **Key Points**

1. Static methods cannot access non-static variables or methods directly.
2. Static blocks are executed in the order they appear, only once when the class is loaded.
3. The `this` keyword cannot be used in static methods because they are class-level and don’t reference any specific object.

### Example to Combine `static` Members

```java
class Config {
    static String appName = "MyApp";  // Static variable
    static String version;

    static {  // Static block
        version = "1.0";
        System.out.println("Static block initialized!");
    }

    static void displayConfig() {  // Static method
        System.out.println("App Name: " + appName);
        System.out.println("Version: " + version);
    }
}

public class Main {
    public static void main(String[] args) {
        Config.displayConfig();  // Accessing static members
    }
}
```

Output:

```
Static block initialized!
App Name: MyApp
Version: 1.0
```

By using `static`, you ensure better memory usage and provide a clear separation of class-level and instance-level behavior in your programs.

---

---

## Q7: What is `main` in Java ?

The `main` method in Java is always declared as `static` because it serves as the entry point of the application. Let’s break this down systematically:

### **1. What is the `main` Method?**

The `main` method is the method where the Java Virtual Machine (JVM) starts executing a Java program. Its signature is:

```java
public static void main(String[] args)
```

- **`public`**: The method is accessible from anywhere.
- **`static`**: Indicates that the method belongs to the class, not an instance of the class.
- **`void`**: Specifies that the method does not return a value.
- **`String[] args`**: An array of `String` arguments passed from the command line.

### **2. Why is the `main` Method `static`?**

#### a) **JVM Can Invoke It Without Creating an Object**

- The `main` method is executed by the JVM without creating an instance of the class. Declaring it as `static` allows the JVM to call it directly using the class name.
- Example:
  ```java
  ClassName.main(args);  // JVM invokes this without an object
  ```

#### b) **No Need for Object Creation**

- If `main` were non-static, the JVM would need to create an instance of the class before calling the `main` method. However:
  - To create an instance, the JVM would need to call a constructor.
  - If the constructor has dependencies or requires initialization, it could complicate the startup process.

#### c) **Memory Efficiency**

- Declaring `main` as `static` ensures no unnecessary memory is allocated for an object that serves no purpose in the application's startup.

#### d) **Universality**

- The static `main` method provides a standard, predictable way for the JVM to start the program, ensuring consistency across all Java applications.

### **3. What Happens If `main` Is Not Static?**

If you attempt to declare the `main` method without the `static` keyword, the program will compile but throw a runtime error when executed.

**Example:**

```java
public class Test {
    public void main(String[] args) {  // Non-static main
        System.out.println("This won't work!");
    }
}
```

**Output:**

```
Error: Main method is not static in class Test, please define the main method as:
   public static void main(String[] args)
```

### **4. Why Not Make It Non-Static?**

1. **Circular Dependency Problem**:
   If `main` were non-static, the JVM would need to create an object of the class. However, there’s no predefined way for the JVM to know how to instantiate the class.
2. **Unnecessary Complexity**:
   Requiring object creation just to execute the program would complicate the startup process unnecessarily.
3. **Standardization**:
   Keeping `main` static ensures consistency across all Java programs.

### **5. Practical Example**

```java
public class MainExample {
    public static void main(String[] args) {
        System.out.println("Program started without creating an object!");
    }
}
```

This works because the `main` method is static and can be executed directly by the JVM without creating an instance of `MainExample`.

### **6. When Does It Make Sense to Use Non-Static Methods?**

- Non-static methods are used when the behavior depends on the state of an object (i.e., instance variables).
- In contrast, `main` is simply a starting point and does not depend on object-specific data.

### **Key Takeaways**

- The `main` method is static to allow the JVM to execute it without instantiating the class.
- This ensures a clean, efficient, and standardized entry point for Java applications.
- Making it non-static would complicate the program's execution process and result in runtime errors.

---

---

## Q8: why static methods cannot directly access non-static members (variables or methods) ?

**static methods cannot directly access non-static members (variables or methods)** because static members belong to the class, whereas non-static members belong to instances of the class. However, you can still use non-static members inside static methods by creating an instance of the class.

### **How to Use Non-Static Members in a Static Method?**

#### **1. Create an Instance of the Class**

To use non-static variables or methods inside a static method, you need to create an object of the class. Through this object, you can access the non-static members.

#### Example:

```java
class Example {
    int nonStaticVar = 10;  // Non-static variable

    void nonStaticMethod() {  // Non-static method
        System.out.println("This is a non-static method.");
    }

    static void staticMethod() {  // Static method
        Example obj = new Example();  // Create an instance
        System.out.println("Accessing non-static variable: " + obj.nonStaticVar);
        obj.nonStaticMethod();  // Accessing non-static method
    }
}

public class Main {
    public static void main(String[] args) {
        Example.staticMethod();  // Call the static method
    }
}
```

**Output:**

```
Accessing non-static variable: 10
This is a non-static method.
```

### **2. Why Can't Static Methods Directly Access Non-Static Members?**

Static methods and variables are tied to the class, not a specific object. Since non-static members depend on an instance of the class, they cannot be accessed directly without knowing which instance they belong to.

### **3. Access Non-Static Members Through Parameters**

If a static method receives an object of the class as a parameter, it can use that object to access non-static members.

#### Example:

```java
class Example {
    int nonStaticVar = 20;

    void nonStaticMethod() {
        System.out.println("Non-static method called.");
    }

    static void staticMethod(Example obj) {
        System.out.println("Accessing non-static variable: " + obj.nonStaticVar);
        obj.nonStaticMethod();
    }
}

public class Main {
    public static void main(String[] args) {
        Example example = new Example();
        Example.staticMethod(example);  // Pass the object to the static method
    }
}
```

**Output:**

```
Accessing non-static variable: 20
Non-static method called.
```

### **4. Use Non-Static Members Within Static Blocks**

Static blocks execute once when the class is loaded. To use non-static members, create an instance of the class within the block.

#### Example:

```java
class Example {
    int nonStaticVar = 30;

    Example() {
        System.out.println("Constructor called.");
    }

    static {
        Example obj = new Example();
        System.out.println("Accessing non-static variable in static block: " + obj.nonStaticVar);
    }
}

public class Main {
    public static void main(String[] args) {
        // No explicit action needed; the static block executes during class loading.
    }
}
```

**Output:**

```
Constructor called.
Accessing non-static variable in static block: 30
```

### **5. Combine Static and Non-Static Members**

Use both static and non-static members within a class, ensuring that non-static members are accessed through an instance.

#### Example:

```java
class Example {
    static int staticVar = 100;  // Static variable
    int nonStaticVar = 50;      // Non-static variable

    static void staticMethod() {
        Example obj = new Example();
        System.out.println("Static Variable: " + staticVar);
        System.out.println("Non-Static Variable: " + obj.nonStaticVar);
    }

    void nonStaticMethod() {
        System.out.println("Static Variable: " + staticVar);
        System.out.println("Non-Static Variable: " + nonStaticVar);
    }
}

public class Main {
    public static void main(String[] args) {
        Example.staticMethod();  // Access via class

        Example example = new Example();
        example.nonStaticMethod();  // Access via instance
    }
}
```

**Output:**

```
Static Variable: 100
Non-Static Variable: 50
Static Variable: 100
Non-Static Variable: 50
```

### **Key Points to Remember**

1. **Static members** are class-level and shared by all instances.
2. **Non-static members** are instance-level and belong to specific objects.
3. To access non-static members inside static methods:
   - Create an instance of the class.
   - Pass an instance of the class to the method.
4. Mixing static and non-static members should be done carefully to avoid confusion or unnecessary memory usage.

---

---

### **Key Differences Between Static and Non-Static**

| Feature               | **Static**                                | **Non-Static**                                |
| --------------------- | ----------------------------------------- | --------------------------------------------- |
| **Belongs To**        | Class (shared among all instances)        | Instance (specific to an object)              |
| **Access**            | Using the class name                      | Using an object reference                     |
| **Memory Allocation** | At class loading time                     | When an object is created                     |
| **Accessing Members** | Cannot directly access non-static members | Can access both static and non-static members |
| **Usage**             | Shared data, constants, utility methods   | Instance-specific behavior                    |
| **Context**           | Exists even without objects               | Requires an object to exist                   |

---

---

## Q9: Explain this concept `Parent person1 = new Child("Drawing", 12);` type `Parent person1` is different and object `Child("Drawing", 12)` is different ?

This concept in Java is known as **polymorphism** and specifically **upcasting**.

### 1. **The Setup**

You have:

- **Parent class**: It has some variables and overloaded constructors.
- **Child class**: It extends the Parent class and has its own variables and a constructor.
- In the main file:
  ```java
  Parent person1 = new Child("Drawing", 12);
  ```

Here, you are:

- Declaring `person1` as a **Parent type reference**.
- Creating an object of the **Child class**.

### 2. **What's Happening?**

#### **Polymorphism**

When you write:

```java
Parent person1 = new Child("Drawing", 12);
```

The **type of the reference** (`Parent`) decides what you can access at compile-time.  
The **actual object** (`Child`) determines what happens at runtime.

- **Compile-Time**:  
  The compiler only knows about the `Parent` class, so you can only call methods and access variables that are declared in `Parent`.
- **Run-Time**:  
  When a method is called, the overridden version of the method (in the `Child` class) will execute if it exists.

#### **Upcasting**

You are "upcasting" the `Child` object to the `Parent` type. This is allowed because a `Child` **is-a** `Parent`. It's like saying "a square is a rectangle."

#### **Constructors**

The constructor of the `Child` class will invoke the `Parent` constructor (via `super(...)`) as part of the instantiation process. This ensures the `Parent` part of the object is initialized before the `Child` part.

### 3. **What Happens in Memory?**

When you create `new Child("Drawing", 12)`:

- **Parent's part of the object** is initialized first using the appropriate constructor.
- **Child's part of the object** is initialized next using the Child class constructor.
- The `person1` reference points to the memory of this Child object but treats it as a Parent.

### 4. **Code Example**

Here’s a complete example:

```java
// Parent class
class Parent {
    String hobby;
    int age;

    // Overloaded constructor
    public Parent(String hobby, int age) {
        this.hobby = hobby;
        this.age = age;
    }

    // Method in Parent
    public void showDetails() {
        System.out.println("Hobby: " + hobby + ", Age: " + age);
    }
}

// Child class
class Child extends Parent {
    String favoriteToy;

    // Constructor in Child
    public Child(String hobby, int age) {
        super(hobby, age); // Call Parent's constructor
        this.favoriteToy = "Lego"; // Child-specific property
    }

    // Overriding method
    @Override
    public void showDetails() {
        super.showDetails();
        System.out.println("Favorite Toy: " + favoriteToy);
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Parent person1 = new Child("Drawing", 12);
        person1.showDetails(); // Calls Child's overridden method
        // person1.favoriteToy; // Compile error: Parent reference can't access Child-specific properties
    }
}
```

### 5. **Key Points**

- **Parent person1 = new Child(...)**:  
  You can only access methods and fields defined in `Parent` through `person1`. Child-specific properties or methods are hidden unless cast back to `Child`.
- **Overriding**:  
  If the `Child` overrides a method from the `Parent`, the `Child`'s version will be executed, thanks to runtime polymorphism.

- **Cannot Access Child's Properties Directly**:  
  To access `Child`-specific methods or variables, you need to cast the reference:
  ```java
  ((Child) person1).favoriteToy;
  ```

---

---

## Q9: Explain this concept `Child person1 = new Parent("Drawing", 12);` type `Child person1` is different subclass and object `Parent("Drawing", 12)` is different parent class ?

In Java, if you try to do the reverse, i.e.,:

```java
Child person1 = new Parent("Drawing", 12);
```

It **will not compile** and will result in a **compile-time error**. Here's why:

### 1. **Why It Doesn't Work**

The **Parent** class is a **superclass** of the **Child** class. Not every `Parent` is necessarily a `Child`. While the reverse (upcasting) is true because a `Child` **is-a** `Parent`, the same logic does not apply when trying to downcast a `Parent` to a `Child`.

#### **Explanation**

When you declare `Child person1`, Java expects an object that is actually of type `Child` or a subclass of `Child`. However, `new Parent("Drawing", 12)` creates an object of type `Parent`, which does not have the additional features (fields or methods) of the `Child` class.

### 2. **Why Upcasting Works But Not This**

- **Upcasting** (`Parent person1 = new Child(...)`) works because every `Child` has all the features of a `Parent` (inheritance ensures this).
- **Downcasting** (`Child person1 = new Parent(...)`) requires the object to be an actual `Child`. Java does not allow this assignment unless you explicitly cast, and even then, it will fail at runtime if the object is not a `Child`.

### 3. **Explicit Casting**

If you try to **force** it using an explicit cast, like this:

```java
Child person1 = (Child) new Parent("Drawing", 12);
```

It will compile, but you will encounter a **`ClassCastException`** at runtime. This is because the actual object in memory is of type `Parent`, and you cannot treat it as a `Child`.

### 4. **Example**

Here’s what happens in code:

```java
// Parent class
class Parent {
    String hobby;

    public Parent(String hobby) {
        this.hobby = hobby;
    }

    public void showDetails() {
        System.out.println("Hobby: " + hobby);
    }
}

// Child class
class Child extends Parent {
    String favoriteToy;

    public Child(String hobby) {
        super(hobby);
        this.favoriteToy = "Lego";
    }

    @Override
    public void showDetails() {
        super.showDetails();
        System.out.println("Favorite Toy: " + favoriteToy);
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        // This line will not compile
        // Child person1 = new Parent("Drawing");

        // Forceful casting
        try {
            Parent parent = new Parent("Drawing");
            Child person1 = (Child) parent; // Explicit cast
            person1.showDetails(); // Runtime error: ClassCastException
        } catch (ClassCastException e) {
            System.out.println("Error: " + e.getMessage());
        }
    }
}
```

### 5. **Key Points**

1. **You cannot assign a Parent object to a Child reference directly.**

   - Compile-time error: "Incompatible types: Parent cannot be converted to Child."

2. **Explicit casting will compile but fail at runtime unless the object is actually of the Child type.**

3. **Why?**
   - A `Parent` object lacks the additional properties or methods of a `Child`. Treating it as a `Child` violates the type system.

### 6. **When Does Downcasting Work?**

Downcasting is valid only when the object was originally created as a `Child`. For example:

```java
Parent parent = new Child("Drawing");
Child child = (Child) parent; // Works because the object is actually a Child
child.showDetails();
```

This works because the actual object in memory is of type `Child`, even though it was referenced as a `Parent`.

---

---

## Q10: Implicit and Explicit Type Casting

**implicit** and **explicit** type casting.

### Implicit Type Casting (Widening Conversion)

- Java automatically converts a smaller data type to a larger one.
- No data loss occurs.

#### Example:

```java
public class TypeCastingDemo {
    public static void main(String[] args) {
        // Implicit Casting: int to double
        int num = 100;
        double doubleNum = num; // Automatically converts int to double

        System.out.println("Original int value: " + num);
        System.out.println("Implicitly casted to double: " + doubleNum);
    }
}
```

### Explicit Type Casting (Narrowing Conversion)

- You manually convert a larger data type to a smaller one.
- May lead to data loss or truncation.

#### Example:

```java
public class TypeCastingDemo {
    public static void main(String[] args) {
        // Explicit Casting: double to int
        double doubleValue = 99.99;
        int intValue = (int) doubleValue; // Manually cast double to int

        System.out.println("Original double value: " + doubleValue);
        System.out.println("Explicitly casted to int: " + intValue); // Fractional part is truncated
    }
}
```

### Practice Tasks

1. **Implicit Casting**:

   - Declare variables of types `byte`, `short`, `int`, `long`, `float`, and `double`.
   - Assign values and observe how smaller types automatically cast to larger types.

   ```java
   byte byteVal = 10;
   int intVal = byteVal; // Implicit cast
   float floatVal = intVal; // Implicit cast

   System.out.println("Byte to Int: " + intVal);
   System.out.println("Int to Float: " + floatVal);
   ```

2. **Explicit Casting**:

   - Declare a variable of type `double` and cast it to `int` and `float`.
   - Observe the truncation of fractional parts.

   ```java
   double price = 123.45;
   int roundedPrice = (int) price;
   System.out.println("Double to Int: " + roundedPrice);
   ```

3. **Mixed Type Operations**:

   - Perform arithmetic operations involving different types and observe automatic type promotion.

   ```java
   int intNum = 10;
   double doubleNum = 3.5;
   double result = intNum + doubleNum; // int is promoted to double
   System.out.println("Result of int + double: " + result);
   ```

4. **Overflow in Explicit Casting**:

   - Assign a large `int` or `long` value to a smaller type like `byte` and observe the behavior.

   ```java
   int largeNum = 130; // Larger than byte range (-128 to 127)
   byte smallNum = (byte) largeNum; // Overflow occurs
   System.out.println("Overflowed byte value: " + smallNum);
   ```

### Key Concepts to Understand

- **Widening (Implicit) Casting**: Happens automatically when there’s no risk of data loss.
- **Narrowing (Explicit) Casting**: Requires manual casting, might lead to data loss.
- **Type Promotion in Expressions**: Smaller types are promoted to `int` or larger during operations.

### Challenges to Try

1. Write a program that accepts user input as a `String`, converts it to `int`, and then performs calculations by implicitly and explicitly casting it to other types.
2. Simulate a data truncation scenario where a large floating-point number is explicitly cast to an integer.
3. Implement a program that demonstrates type promotion in a multi-type arithmetic operation.

Experiment with these examples and try modifying them to observe the different behaviors of type casting in Java!

---

---

## Q11: Inner Class in Java

### **Inner Class in Java**

An **inner class** in Java is a class that is defined within another class. Inner classes are useful when you want to logically group classes that are used only in one place or need to interact closely with the outer class. Java provides several types of inner classes, each with different characteristics and use cases.

---

### **Types of Inner Classes in Java**

1. **Member Inner Class** (Non-static Inner Class)
2. **Static Nested Class**
3. **Local Inner Class**
4. **Anonymous Inner Class**

---

### **1. Member Inner Class (Non-static Inner Class)**

- A **non-static inner class** is associated with an instance of the outer class. It can access all the members (including private members) of the outer class.
- To create an instance of a non-static inner class, you need an instance of the outer class.

#### **Example**:

```java
class OuterClass {
    private String outerField = "Outer Field";

    // Non-static inner class
    class InnerClass {
        void display() {
            System.out.println("Accessing outer class field: " + outerField);
        }
    }

    void createInnerObject() {
        InnerClass inner = new InnerClass();  // Creating an inner class object
        inner.display();
    }
}

public class InnerClassExample {
    public static void main(String[] args) {
        OuterClass outer = new OuterClass();
        outer.createInnerObject();  // Calling the outer class method that uses inner class
    }
}
```

**Output**:

```
Accessing outer class field: Outer Field
```

- **Explanation**: The `InnerClass` is an instance of a non-static inner class. The `display` method inside the inner class has access to the `outerField` variable of the outer class.

---

### **2. Static Nested Class**

- A **static nested class** is a nested class that is declared with the `static` modifier. A static inner class can only access the static members of the outer class.
- You can create an instance of a static nested class without creating an instance of the outer class.

#### **Example**:

```java
class OuterClass {
    static String outerField = "Outer Static Field";

    // Static nested class
    static class StaticNestedClass {
        void display() {
            System.out.println("Accessing outer static field: " + outerField);
        }
    }
}

public class StaticNestedClassExample {
    public static void main(String[] args) {
        // Creating instance of static nested class without outer class instance
        OuterClass.StaticNestedClass nested = new OuterClass.StaticNestedClass();
        nested.display();
    }
}
```

**Output**:

```
Accessing outer static field: Outer Static Field
```

- **Explanation**: The `StaticNestedClass` is a static nested class that accesses the static member `outerField` of the outer class. It does not require an instance of `OuterClass` to be created.

---

### **3. Local Inner Class**

- A **local inner class** is a class defined inside a method or a block of code. It can only be used within that method or block.
- Local inner classes have access to the final or effectively final variables of the enclosing method.

#### **Example**:

```java
class OuterClass {
    void display() {
        // Local inner class inside a method
        class LocalInnerClass {
            void show() {
                System.out.println("Inside local inner class method");
            }
        }

        LocalInnerClass localInner = new LocalInnerClass();  // Creating object of local inner class
        localInner.show();
    }
}

public class LocalInnerClassExample {
    public static void main(String[] args) {
        OuterClass outer = new OuterClass();
        outer.display();
    }
}
```

**Output**:

```
Inside local inner class method
```

- **Explanation**: The `LocalInnerClass` is defined inside the `display` method and can only be used within that method. It does not have access to the outer class’s instance variables unless those variables are final.

---

### **4. Anonymous Inner Class**

- An **anonymous inner class** is a class that doesn’t have a name and is used to instantiate a class that implements an interface or extends a class. Anonymous classes are typically used for implementing interfaces or abstract classes in a concise manner.
- They are usually used when you need a one-time use class for handling a specific event or task.

#### **Example**:

```java
interface Greeting {
    void sayHello();
}

public class AnonymousInnerClassExample {
    public static void main(String[] args) {
        // Anonymous inner class implementing the Greeting interface
        Greeting greeting = new Greeting() {
            public void sayHello() {
                System.out.println("Hello from anonymous inner class!");
            }
        };

        greeting.sayHello();
    }
}
```

**Output**:

```
Hello from anonymous inner class!
```

- **Explanation**: The anonymous inner class implements the `Greeting` interface and overrides the `sayHello` method. This is a one-time use class that doesn’t need a name.

---

### **Key Differences Between Inner Classes and Outer Classes**

| Feature                  | **Inner Class**                                                      | **Outer Class**                            |
| ------------------------ | -------------------------------------------------------------------- | ------------------------------------------ |
| **Declaration Location** | Inside another class                                                 | Outside any class                          |
| **Access**               | Can access outer class members (instance or static)                  | Cannot directly access inner class members |
| **Instantiation**        | Requires an instance of the outer class (for non-static inner class) | Can be instantiated directly               |
| **Visibility**           | Can be private, protected, or public                                 | Can be public, default, or private         |

---

### **Advantages of Using Inner Classes**

1. **Logical Grouping**: Inner classes can logically group classes that are only used in one place, making the code easier to understand.
2. **Encapsulation**: Inner classes can access private members of the outer class, which helps in maintaining tight encapsulation.
3. **Code Organization**: Inner classes are useful when the class should not be visible outside the enclosing class or package.

---

### **Conclusion**

- Java provides **four types** of inner classes: **Member Inner Class**, **Static Nested Class**, **Local Inner Class**, and **Anonymous Inner Class**.
- **Inner classes** are useful for logically grouping related classes and providing functionality closely tied to the outer class.
- Depending on your requirements, you can choose the appropriate type of inner class to organize and structure your code more effectively.

---

---

## Q12: Lambda Expression in Java

### **Lambda Expression in Java**

A **lambda expression** in Java is a concise way to represent an anonymous function (or method) that can be passed around as a parameter to a method or stored in a variable. It enables a more functional programming style in Java and was introduced in **Java 8** to support functional interfaces and make code more readable and concise.

### **Syntax of a Lambda Expression**

The general syntax of a lambda expression is:

```java
(parameters) -> expression
```

- **parameters**: A comma-separated list of input parameters (optional). The types of parameters can be inferred by the compiler (type inference).
- **->**: The arrow token that separates the parameters from the body.
- **expression**: The body of the lambda expression, which can either be a single expression or a block of code.

#### **Types of Lambda Expressions**

1. **Simple Lambda Expression (Single Expression)**
2. **Lambda Expression with Block of Code**
3. **Lambda Expression with Multiple Parameters**
4. **Lambda Expression without Parameters**

---

### **Examples**

#### **1. Simple Lambda Expression**

```java
// Traditional way (using an anonymous class)
Runnable r1 = new Runnable() {
    @Override
    public void run() {
        System.out.println("Hello from Runnable");
    }
};

// Lambda expression
Runnable r2 = () -> System.out.println("Hello from Runnable using Lambda");

public class LambdaExample {
    public static void main(String[] args) {
        r2.run();  // Calling the lambda expression
    }
}
```

**Output**:

```
Hello from Runnable using Lambda
```

- **Explanation**: The lambda expression `() -> System.out.println("Hello from Runnable using Lambda")` is a more concise way of defining the `run` method of `Runnable`.

#### **2. Lambda Expression with Block of Code**

```java
// Lambda with multiple statements
Runnable r2 = () -> {
    System.out.println("Hello from Runnable");
    System.out.println("This is executed in the Lambda expression.");
};

public class LambdaExample {
    public static void main(String[] args) {
        r2.run();
    }
}
```

**Output**:

```
Hello from Runnable
This is executed in the Lambda expression.
```

- **Explanation**: Here, the body of the lambda expression is a block of code enclosed by `{}`. It can contain multiple statements.

#### **3. Lambda Expression with Multiple Parameters**

```java
// Lambda with two parameters
BiFunction<Integer, Integer, Integer> add = (a, b) -> a + b;

public class LambdaExample {
    public static void main(String[] args) {
        System.out.println(add.apply(5, 10));  // Output: 15
    }
}
```

**Output**:

```
15
```

- **Explanation**: The lambda expression `(a, b) -> a + b` takes two parameters `a` and `b` and returns their sum. `BiFunction` is a functional interface that takes two arguments and returns a result.

#### **4. Lambda Expression without Parameters**

```java
// Lambda with no parameters
Runnable r = () -> System.out.println("No parameters lambda");

public class LambdaExample {
    public static void main(String[] args) {
        r.run();  // Output: No parameters lambda
    }
}
```

**Output**:

```
No parameters lambda
```

- **Explanation**: This is a lambda expression with no parameters, similar to the traditional anonymous class.

---

### **Functional Interfaces and Lambda Expressions**

A **functional interface** is an interface that has only one abstract method. Lambda expressions can be used to implement functional interfaces. Common functional interfaces in Java include:

- **Runnable**: `void run()`
- **Callable**: `V call()`
- **Comparator**: `int compare(T o1, T o2)`
- **Consumer**: `void accept(T t)`
- **Supplier**: `T get()`
- **Function**: `R apply(T t)`
- **Predicate**: `boolean test(T t)`
- **BiFunction**: `R apply(T t, U u)`

For example:

```java
@FunctionalInterface
interface MyFunctionalInterface {
    void myMethod();
}

public class LambdaExample {
    public static void main(String[] args) {
        MyFunctionalInterface obj = () -> System.out.println("Lambda expression in action");
        obj.myMethod();  // Output: Lambda expression in action
    }
}
```

- **Explanation**: `MyFunctionalInterface` is a functional interface with one method `myMethod()`. The lambda expression implements this method in a concise way.

---

### **Advantages of Lambda Expressions**

1. **Concise and Readable**: Lambda expressions reduce boilerplate code, making it more concise and readable.
2. **Functional Programming**: They encourage the use of functional programming techniques like passing behavior as arguments to methods.
3. **Parallel Processing**: Lambda expressions make it easier to use parallel streams, improving performance with large data sets.
4. **Less Code**: Reduces the need for anonymous inner classes, making code easier to maintain.

---

### **Use Cases for Lambda Expressions**

- **Event Handling**: Commonly used in GUI applications (like Swing or JavaFX) to handle events.
- **Streams API**: Lambda expressions are heavily used with the Streams API for operations like filtering, mapping, and reducing collections of data.
- **Concurrency**: Used in concurrent programming for writing short, concise callbacks or runnable tasks.

---

### **Example with Java Streams API**

Lambda expressions are widely used with the Java Streams API to process collections in a functional style.

```java
import java.util.Arrays;
import java.util.List;

public class LambdaStreamExample {
    public static void main(String[] args) {
        List<String> names = Arrays.asList("Alice", "Bob", "Charlie", "David");

        // Using lambda expression to print names that start with 'A'
        names.stream()
             .filter(name -> name.startsWith("A"))
             .forEach(name -> System.out.println(name));
    }
}
```

**Output**:

```
Alice
```

- **Explanation**: The `filter` method is used with a lambda expression to filter names starting with "A", and the `forEach` method prints each name.

---

### **Conclusion**

Lambda expressions in Java allow you to write more concise, functional-style code that is easier to read and maintain. They are particularly useful when working with functional interfaces and collections, and they enable more efficient handling of data processing tasks, such as filtering and transforming collections using the Streams API.

---

---

## Q13: Java Exception Hierarchy

### **Java Exception Hierarchy**

In Java, exceptions are used to handle errors or other exceptional conditions that may arise during program execution. The exception handling mechanism in Java is built around the `Throwable` class, which is the root of the exception hierarchy.

Here’s a breakdown of the **Exception Hierarchy** in Java, along with examples of different types of exceptions.

---

### **1. `Throwable` Class**

- **`Throwable`** is the superclass of all errors and exceptions in Java.

  - `Throwable` has two main subclasses:
    - **`Error`**
    - **`Exception`**

- The `Throwable` class is the root of the entire exception hierarchy.

#### **Hierarchy Overview**:

```
Throwable
   |
   +-- Error
   |    (e.g., OutOfMemoryError, StackOverflowError)
   |
   +-- Exception
        |
        +-- RuntimeException
        |    (e.g., NullPointerException, ArrayIndexOutOfBoundsException)
        |
        +-- Checked Exceptions
             (e.g., IOException, SQLException, ClassNotFoundException)
```

---

### **2. `Error` Class**

- **Errors** represent serious problems that a reasonable application should not try to catch. These typically relate to the **Java Virtual Machine (JVM)** and indicate **irrecoverable conditions**.
- Errors are usually not handled by applications because they are out of the application’s control (e.g., running out of memory, JVM crashing).

#### **Common Subclasses of `Error`:**

- **`OutOfMemoryError`**: Raised when the JVM runs out of memory.
- **`StackOverflowError`**: Raised when the stack overflows due to deep recursion.
- **`VirtualMachineError`**: Represents other JVM-related issues.

Example of **`Error`**:

```java
public class ErrorExample {
    public static void main(String[] args) {
        // Example of StackOverflowError
        recursiveMethod();
    }

    public static void recursiveMethod() {
        recursiveMethod(); // This will cause StackOverflowError
    }
}
```

- **Explanation**: The `recursiveMethod()` keeps calling itself, leading to a **`StackOverflowError`** when the stack space is exhausted.

---

### **3. `Exception` Class**

- **Exceptions** are events that disrupt the normal flow of a program’s execution.
- Exceptions are of two types:
  1. **Checked Exceptions**: These exceptions are checked at compile-time, and you must either handle them using a try-catch block or declare them with the `throws` keyword.
  2. **Unchecked Exceptions**: These exceptions occur at runtime, and they are not checked at compile-time.

---

### **4. `Checked Exceptions`**

- **Checked exceptions** are exceptions that the compiler forces you to handle. These exceptions must be either caught or declared in the method signature with the `throws` keyword.
- Common checked exceptions include **`IOException`**, **`SQLException`**, and **`ClassNotFoundException`**.

#### **Example of Checked Exception (`IOException`)**:

```java
import java.io.*;

public class CheckedExceptionExample {
    public static void main(String[] args) {
        try {
            // File reading without exception handling will cause a compile-time error
            FileReader reader = new FileReader("non_existent_file.txt");
            BufferedReader bufferedReader = new BufferedReader(reader);
            System.out.println(bufferedReader.readLine());
        } catch (IOException e) {
            System.out.println("Caught IOException: " + e.getMessage());
        }
    }
}
```

**Output**:

```
Caught IOException: non_existent_file.txt (The system cannot find the file specified)
```

- **Explanation**: `IOException` is a checked exception, so you must either handle it with a try-catch block or declare it with the `throws` keyword. In this case, we handle it with a try-catch block.

---

### **5. `Unchecked Exceptions`**

- **Unchecked exceptions** are exceptions that are not checked at compile-time. These are typically caused by programming bugs, such as accessing a null object or going beyond the array bounds.
- They are subclasses of **`RuntimeException`**.
- Common unchecked exceptions include **`NullPointerException`**, **`ArrayIndexOutOfBoundsException`**, and **`ArithmeticException`**.

#### **Example of Unchecked Exception (`NullPointerException`)**:

```java
public class UncheckedExceptionExample {
    public static void main(String[] args) {
        String str = null;

        // This will throw NullPointerException
        System.out.println(str.length());
    }
}
```

**Output**:

```
Exception in thread "main" java.lang.NullPointerException: Cannot invoke "String.length()" because "str" is null
```

- **Explanation**: The code throws a `NullPointerException` because we try to call `length()` on a `null` object.

---

### **6. `RuntimeException` Class**

- `RuntimeException` is the parent class for all unchecked exceptions.
- These exceptions occur due to programming errors that could have been avoided (e.g., **`ArrayIndexOutOfBoundsException`**, **`ClassCastException`**, **`IllegalArgumentException`**, etc.).

#### **Common Subclasses of `RuntimeException`:**

- **`NullPointerException`**: Thrown when an application attempts to use `null` where an object is required.
- **`ArithmeticException`**: Thrown when an illegal arithmetic operation is performed (e.g., division by zero).
- **`IndexOutOfBoundsException`**: Thrown when an index is out of range for an array or list.

---

### **7. Example of Full Exception Hierarchy with Code**

```java
public class ExceptionHierarchyExample {
    public static void main(String[] args) {
        try {
            // Simulating a checked exception
            checkAge(-1);  // This will cause IllegalArgumentException (RuntimeException)
        } catch (IllegalArgumentException e) {
            System.out.println("Caught Exception: " + e.getMessage());
        }

        try {
            // Simulating an unchecked exception
            FileReader reader = new FileReader("non_existent_file.txt");
        } catch (IOException e) {
            System.out.println("Caught IOException: " + e.getMessage());
        }
    }

    // Example method that throws a checked exception
    public static void checkAge(int age) throws IllegalArgumentException {
        if (age < 0) {
            throw new IllegalArgumentException("Age cannot be negative");
        }
        System.out.println("Age: " + age);
    }
}
```

**Output**:

```
Caught Exception: Age cannot be negative
Caught IOException: non_existent_file.txt (The system cannot find the file specified)
```

- **Explanation**: The first `try-catch` block handles the **`IllegalArgumentException`** (which is a runtime exception). The second block handles the **`IOException`**, which is a checked exception.

---

### **Summary of Exception Types**

| **Type**                 | **Examples**                                  | **Checked or Unchecked** |
| ------------------------ | --------------------------------------------- | ------------------------ |
| **`Error`**              | `OutOfMemoryError`, `StackOverflowError`      | Unchecked                |
| **`Exception`**          |                                               |                          |
| **Checked Exceptions**   | `IOException`, `SQLException`                 | Checked                  |
| **Unchecked Exceptions** | `NullPointerException`, `ArithmeticException` | Unchecked                |

- **Checked exceptions** must be either caught or declared in the method signature.
- **Unchecked exceptions** do not need to be explicitly handled, but it’s a good practice to avoid them in the code through proper validation.

---

### **Conclusion**

In Java, the **exception hierarchy** starts with `Throwable`, which is divided into **Errors** and **Exceptions**. Errors typically indicate problems with the JVM or system, while exceptions are conditions that applications may handle. Exceptions are further categorized into **checked exceptions** (which must be handled) and **unchecked exceptions** (which are runtime errors that may be ignored or handled). Understanding this hierarchy helps in writing robust programs by properly handling errors and exceptions.

---

---
