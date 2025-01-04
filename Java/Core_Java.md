# **Core Java**

- [Q1: Features of Java](#q1-features-of-java)
- [Q2: Compile Time vs Run Time in Java](#q2-compile-time-vs-run-time-in-java)
- [Q3: The `new` keyword](#q3-the-new-keyword)
- [Q4: Reserved Keywords in Java](#q4-reserved-keywords-in-java)
- [Q5: Difference between a **compiler** and an **interpreter**](#q5-difference-between-a-compiler-and-an-interpreter)
- [Q6: Stack and Heap Memory management in Java](#q6-stack-and-heap-memory-management-in-java)
- [Q7: Mutable vs Immutable String in Java](#q7-mutable-vs-immutable-string-in-java)
- [Q8: Instance Variables in Java](#q8-instance-variables-in-java)
- [Q9: Class Variables in Java](#q9-class-variables-in-java)
- [Q10: What is a Compiler?](#q10-what-is-a-compiler)
- [Q11: Classes and Objects in Java](#q11-classes-and-objects-in-java)
- [Q12: Wrapper Classes in Java](#q12-wrapper-classes-in-java)
- [Q13: Packages in Java](#q13-packages-in-java)
- [Q14: What is `static` in Java?](#q14-what-is-static-in-java)
- [Q15: Why static methods cannot directly access non-static members (variables or methods)?](#q15-why-static-methods-cannot-directly-access-non-static-members)
- [Q16: What is `main` in Java?](#q16-what-is-main-in-java)
- [Q17: Implicit and Explicit Type Casting](#q17-implicit-and-explicit-type-casting)
- [Q18: Inner Class in Java](#q18-inner-class-in-java)
- [Q19: Lambda Expression in Java](#q19-lambda-expression-in-java)
- [Q20: Java Exception Hierarchy](#q20-java-exception-hierarchy)
- [Q21: Singleton Class](#q21-singleton-class)
- [Q22: Principles of Object-Oriented Programming (OOP)](#q22-principles-of-object-oriented-programming-oop)
- [Q23: Inheritance](#q23-inheritance)
- [Q24: Types of Inheritance (Single, Multilevel, Hierarchical)](#q24-types-of-inheritance-single-multilevel-hierarchical)
- [Q25: `super` Keyword in Java](#q25-super-keyword-in-java)
- [Q26: Polymorphism in Java](#q26-polymorphism-in-java)
- [Q27: Real-World Examples of Polymorphism](#q27-real-world-examples-of-polymorphism)
- [Q28: Explain this concept `Parent person1 = new Child("Drawing", 12)`; type `Parent person1` is different and object `Child("Drawing", 12)` is different?](#q28-explain-this-concept-parent-person1--new-childdrawing-12-type-parent-person1-is-different-and-object-childdrawing-12-is-different)
- [Q29: Explain this concept `Child person1 = new Parent("Drawing", 12)`; type `Child person1` is a subclass and object `Parent("Drawing", 12)` is from the parent class?](#q29-explain-this-concept-child-person1--new-parentdrawing-12-type-child-person1-is-a-subclass-and-object-parentdrawing-12-is-from-the-parent-class)
- [Q30: Method Overriding in Java](#q30-method-overriding-in-java)
- [Q31: Can we override static methods?](#q31-can-we-override-static-methods)
- [Q32: Encapsulation in Java](#q32-encapsulation-in-java)
- [Q33: Real-World Examples of Encapsulation](#q33-real-world-examples-of-encapsulation)
- [Q34: Abstraction in Java](#q34-abstraction-in-java)
- [Q35: Real-World Examples of Abstraction](#q35-real-world-examples-of-abstraction)
- [Q36: Difference Between Encapsulation and Abstraction](#q36-difference-between-encapsulation-and-abstraction)
- [Q37: Data Hiding in Object-Oriented Programming (OOP)](#q37-data-hiding-in-object-oriented-programming-oop)

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

static: Indicates the variable belongs to the class, not to any specific object.
It can be accessed directly using the class name.
```

---

---

### **Core Java** Table:

| **Aspect**                      | **Core Java**                                                                                  |
| ------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Basic Syntax**                | Basic structure of Java programs, including keywords, identifiers, and statements.             |
| **Data Types**                  | Primitive data types (int, float, char, boolean) and non-primitive types (String, Arrays).     |
| **Control Flow**                | Conditional statements (`if`, `else`, `switch`), loops (`for`, `while`, `do-while`).           |
| **Object-Oriented Programming** | Classes, objects, inheritance, polymorphism, encapsulation, abstraction.                       |
| **Constructors**                | Default and parameterized constructors.                                                        |
| **Exception Handling**          | `try-catch`, `throw`, `throws`, `finally`.                                                     |
| **Multithreading**              | Thread creation and synchronization using `Thread` and `Runnable`.                             |
| **Java Collections Framework**  | `List`, `Set`, `Map`, `Queue`, with implementations like `ArrayList`, `HashMap`, `LinkedList`. |
| **Input/Output (I/O)**          | File I/O using `FileReader`, `BufferedReader`, `PrintWriter`; streams (Byte and Character).    |
| **Java API**                    | Core libraries like `java.lang`, `java.util`, `java.io`, `java.math`, etc.                     |
| **Memory Management**           | Stack vs Heap memory management, garbage collection basics.                                    |
| **String Handling**             | String manipulation using `String`, `StringBuilder`, `StringBuffer`.                           |
| **Utility Classes**             | `Date`, `Math`, `Calendar`, `UUID`, etc.                                                       |

### **Advanced Java** Table:

| **Aspect**                                     | **Advanced Java**                                                                                         |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **Database Connectivity (JDBC)**               | Connecting to databases, CRUD operations using JDBC.                                                      |
| **Servlets**                                   | Handling HTTP requests and responses, creating dynamic web pages.                                         |
| **JavaServer Pages (JSP)**                     | Embedding Java in HTML for creating dynamic content in web applications.                                  |
| **J2EE (Java 2 Enterprise Edition)**           | Enterprise-level Java applications using Servlets, JSP, EJB, JMS, and more.                               |
| **Web Services (SOAP/REST)**                   | Creating and consuming web services using SOAP and REST APIs.                                             |
| **JavaMail API**                               | Sending, receiving, and processing emails in Java applications.                                           |
| **JNDI (Java Naming and Directory Interface)** | Resource management, service lookups, and accessing distributed resources like databases and EJBs.        |
| **Java Security**                              | Cryptography, SSL/TLS, authentication, authorization, and secure coding practices.                        |
| **EJB (Enterprise JavaBeans)**                 | Building distributed enterprise applications using session beans, entity beans, and message-driven beans. |
| **JavaFX**                                     | GUI development for building rich desktop applications.                                                   |
| **Spring Framework**                           | Dependency Injection (DI), Aspect-Oriented Programming (AOP), Spring Boot, Spring MVC, and Spring Data.   |
| **Hibernate (ORM)**                            | Object-relational mapping, database interaction via Java objects, and managing persistence.               |
| **Microservices**                              | Building microservices with Spring Boot and deploying them in cloud environments.                         |
| **Message-Oriented Middleware (MOM)**          | Asynchronous communication with JMS (Java Message Service).                                               |
| **Transactions (JTA)**                         | Managing transactions in distributed environments using Java Transaction API (JTA).                       |
| **Cloud and Web Applications**                 | Developing cloud-based solutions, integrating Java with cloud platforms.                                  |

---

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

## Q2: Compile Time vs Run Time in Java

the distinction between compile time and run time is essential for understanding how a program is executed. Here's an explanation with examples:

### 1. **Compile Time**:

Compile time refers to the period when the source code is being compiled into bytecode by the Java compiler (i.e., `javac`). This is where syntax errors, type checking, and other compile-time issues are caught.

**Example:**

```java
public class CompileTimeExample {
    public static void main(String[] args) {
        int x = "Hello"; // Compile-time error: incompatible types
        System.out.println(x);
    }
}
```

**Explanation**:

- The error in the above code will be caught **during compilation** because you're trying to assign a `String` to an `int` variable, which is not allowed.
- This error is detected by the Java compiler when you run `javac CompileTimeExample.java`.

**Compile-time errors** are syntax errors, type mismatch, missing semicolons, etc.

### 2. **Run Time**:

Run time refers to the period when the program is actually running (after it has been compiled). Any errors that occur during execution (such as trying to access an element in an array that doesn't exist, dividing by zero, or causing memory issues) are **run-time errors**.

**Example:**

```java
public class RunTimeExample {
    public static void main(String[] args) {
        int[] numbers = new int[2];
        numbers[3] = 10; // Run-time error: ArrayIndexOutOfBoundsException
    }
}
```

**Explanation**:

- This code will compile without errors, but during execution (when the program runs), trying to access `numbers[3]` will cause a `ArrayIndexOutOfBoundsException` because the array only has 2 elements (indices 0 and 1).
- **Run-time errors** are exceptions like `NullPointerException`, `ArrayIndexOutOfBoundsException`, etc.

### Key Differences:

| Aspect             | Compile Time                                      | Run Time                                                                   |
| ------------------ | ------------------------------------------------- | -------------------------------------------------------------------------- |
| **When It Occurs** | During the compilation of source code             | During the execution of the program                                        |
| **Errors**         | Syntax errors, type errors, missing imports, etc. | Logical errors, exceptions (e.g., null pointer, array index out of bounds) |
| **Fixing Errors**  | Fixed by correcting code before compiling         | Fixed by fixing the logic or handling exceptions in code                   |
| **Example**        | `int x = "Hello";` (incompatible types)           | `numbers[3] = 10;` (Array index out of bounds)                             |

### Summary:

- **Compile-time errors** prevent the program from compiling and are found before execution.
- **Run-time errors** occur during the program's execution and are typically handled with exception handling mechanisms (e.g., `try-catch` blocks).

---

---

## Q3: the `new` keyword

In Java, the **`new`** keyword is used to create new objects or instances of classes. It is essential to understand that the `new` keyword allocates memory for an object on the heap, initializes the object using the class constructor, and returns a reference to that object. This makes the `new` keyword a fundamental part of object creation and memory management in Java.

### **1. Creating Objects with the `new` Keyword**

When you want to create an instance of a class, you use the `new` keyword followed by the class constructor. The syntax for creating an object using `new` is:

```java
ClassName objectName = new ClassName();
```

Here, `ClassName` is the name of the class you want to instantiate, and `objectName` is the reference variable that will hold the object.

**Example:**

```java
public class Car {
    String color;
    String model;

    // Constructor
    public Car(String color, String model) {
        this.color = color;
        this.model = model;
    }

    public void displayInfo() {
        System.out.println("Car Model: " + model + ", Color: " + color);
    }
}

public class Main {
    public static void main(String[] args) {
        // Creating an object of the Car class using the 'new' keyword
        Car myCar = new Car("Red", "Tesla");
        myCar.displayInfo(); // Outputs: Car Model: Tesla, Color: Red
    }
}
```

### **Detailed Explanation of the `new` Keyword**

1. **Memory Allocation**:  
   When you create an object using the `new` keyword, memory is allocated on the **heap** for the object. The heap is an area of memory reserved for objects during program execution.

   - For example, in the `Car myCar = new Car("Red", "Tesla");` statement, memory for the `Car` object is allocated on the heap.
   - The constructor of the `Car` class is called to initialize the object with the specified values (e.g., `"Red"` for color and `"Tesla"` for model).

2. **Calling the Constructor**:  
   After allocating memory, the `new` keyword invokes the class constructor. This constructor is responsible for initializing the newly created object with default or provided values.

   - In the example above, the constructor `Car(String color, String model)` is invoked, and it initializes the `color` and `model` fields of the object.

3. **Reference Assignment**:  
   The reference variable (`myCar` in the example) is assigned the memory address (reference) of the newly created object. This reference is used to access the object’s properties and methods.

4. **Object Initialization**:  
   The `new` keyword calls the class constructor to initialize the newly created object. If no constructor is explicitly defined in the class, Java provides a default constructor that initializes the object with default values (e.g., `null` for objects, `0` for numeric types).

### **2. Using `new` with Arrays**

In addition to creating instances of classes, the `new` keyword is also used to create arrays. An array is essentially an object in Java, and memory for it is allocated on the heap.

**Syntax for creating an array:**

```java
type[] arrayName = new type[size];
```

**Example:**

```java
public class Main {
    public static void main(String[] args) {
        // Creating an array of integers using the 'new' keyword
        int[] numbers = new int[5]; // Array of size 5
        numbers[0] = 10; // Assigning values to the array elements
        numbers[1] = 20;

        System.out.println(numbers[0]); // Outputs: 10
        System.out.println(numbers[1]); // Outputs: 20
    }
}
```

### **3. Default Initialization with `new`**

When you use `new` to create an object or array, Java automatically initializes its fields or elements to default values if no explicit initialization is provided. For example:

- **Primitive Data Types** (for arrays):
  - `int` → `0`
  - `boolean` → `false`
  - `char` → `'\u0000'`
  - `double` → `0.0`
- **Object References**:
  - All object references are initialized to `null` by default.

**Example:**

```java
public class Main {
    public static void main(String[] args) {
        int[] numbers = new int[3]; // Array of 3 integers
        System.out.println(numbers[0]); // Outputs: 0 (default value for int)
        System.out.println(numbers[1]); // Outputs: 0
        System.out.println(numbers[2]); // Outputs: 0
    }
}
```

### **4. No `new` Keyword for Primitive Types**

Primitive data types (like `int`, `char`, `boolean`, etc.) do not require the `new` keyword because they are not objects. They are allocated on the **stack** and directly hold values.

**Example of primitive type initialization (without `new` keyword):**

```java
public class Main {
    public static void main(String[] args) {
        int x = 10; // No need for 'new' as 'int' is a primitive type
        System.out.println(x); // Outputs: 10
    }
}
```

### **5. Constructor Overloading**

In Java, you can have multiple constructors for a class, each having a different parameter list. When you use `new`, the appropriate constructor is invoked based on the arguments provided.

**Example:**

```java
public class Car {
    String color;
    String model;

    // Constructor with two parameters
    public Car(String color, String model) {
        this.color = color;
        this.model = model;
    }

    // Constructor with one parameter
    public Car(String color) {
        this.color = color;
        this.model = "Unknown";
    }
}

public class Main {
    public static void main(String[] args) {
        // Using the constructor with two parameters
        Car myCar = new Car("Red", "Tesla");
        System.out.println(myCar.color + " " + myCar.model); // Outputs: Red Tesla

        // Using the constructor with one parameter
        Car anotherCar = new Car("Blue");
        System.out.println(anotherCar.color + " " + anotherCar.model); // Outputs: Blue Unknown
    }
}
```

### **6. The `new` Keyword and Garbage Collection**

In Java, when an object is no longer referenced, it becomes eligible for garbage collection. Java's garbage collector automatically reclaims memory used by objects that are no longer in use.

**Example of garbage collection:**

```java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car("Red", "Tesla");
        myCar = null; // Now myCar doesn't refer to the object anymore

        // The object is eligible for garbage collection here
    }
}
```

When the reference variable `myCar` is set to `null`, the object becomes eligible for garbage collection, and memory used by that object can be reclaimed later.

### **Summary of `new` Keyword Usage**

- **Object Creation**: `new` is used to instantiate objects from a class.
- **Array Creation**: `new` is used to create arrays in Java.
- **Memory Allocation**: `new` allocates memory for the object on the heap.
- **Constructor Invocation**: `new` invokes the constructor to initialize the object.
- **Default Initialization**: Objects are initialized to default values when created with `new`.

The `new` keyword is critical for object creation and memory management in Java. It allows you to instantiate and initialize objects and arrays dynamically during program execution.

---

---

## Q4: reserved keywords in Java ?

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

## Q5: Difference between a **compiler** and an **interpreter**

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

## Q6: Stack and Heap Memory management in Java

### **Stack and Heap in Java**

In Java, memory is managed in two primary areas:

1. **Stack**: Used for storing local variables, method calls, and references to objects.
2. **Heap**: Used for storing objects and arrays created dynamically at runtime.

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

### **Conclusion**

- **Stack** is used for storing temporary data (local variables, method calls) and is limited in size.
- **Heap** is used for dynamically created objects and arrays and has a larger and more flexible memory space.
- Understanding how stack and heap memory work is essential for optimizing memory usage and preventing issues like **stack overflow** or **memory leaks**.

---

---

## Q7: Mutable vs Immutable String in Java

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

### **When to Use Immutable vs Mutable Strings**

1. **Use Immutable Strings** (`String`):

   - When string content does not need to be changed frequently.
   - When working with **hash-based collections** (`HashMap`, `HashSet`), since the immutability guarantees that the hash code does not change.
   - In multi-threaded applications where thread safety is critical.

2. **Use Mutable Strings** (`StringBuilder` or `StringBuffer`):
   - When performing many modifications or concatenations on strings (e.g., inside loops or when building large strings).
   - In performance-critical sections where the overhead of creating new string objects every time is inefficient.

### **Conclusion**

- **Immutable strings** (`String`) are safe, thread-friendly, and commonly used in scenarios where string values don’t change often.
- **Mutable strings** (`StringBuilder`/`StringBuffer`) are more performance-efficient when strings undergo frequent modifications.
- Understanding when to use **String** and when to use **StringBuilder** or **StringBuffer** can significantly improve performance in Java applications.

---

---

## Q8: Instance Variables in Java?

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

## Q9: Class Variables in Java?

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

## Q10: What is a Compiler?

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

## Q11: classes and objects in Java

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

## Q12: wrapper classes in Java?

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

## Q13: Packages in Java ?

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

## Q14: What is `static` in Java?

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

## Q15: why static methods cannot directly access non-static members (variables or methods) ?

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

## Q16: What is `main` in Java ?

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

## Q17: Implicit and Explicit Type Casting

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

## Q18: Inner Class in Java

### **Inner Class in Java**

An **inner class** in Java is a class that is defined within another class. Inner classes are useful when you want to logically group classes that are used only in one place or need to interact closely with the outer class. Java provides several types of inner classes, each with different characteristics and use cases.

### **Types of Inner Classes in Java**

1. **Member Inner Class** (Non-static Inner Class)
2. **Static Nested Class**
3. **Local Inner Class**
4. **Anonymous Inner Class**

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

### **Key Differences Between Inner Classes and Outer Classes**

| Feature                  | **Inner Class**                                                      | **Outer Class**                            |
| ------------------------ | -------------------------------------------------------------------- | ------------------------------------------ |
| **Declaration Location** | Inside another class                                                 | Outside any class                          |
| **Access**               | Can access outer class members (instance or static)                  | Cannot directly access inner class members |
| **Instantiation**        | Requires an instance of the outer class (for non-static inner class) | Can be instantiated directly               |
| **Visibility**           | Can be private, protected, or public                                 | Can be public, default, or private         |

### **Advantages of Using Inner Classes**

1. **Logical Grouping**: Inner classes can logically group classes that are only used in one place, making the code easier to understand.
2. **Encapsulation**: Inner classes can access private members of the outer class, which helps in maintaining tight encapsulation.
3. **Code Organization**: Inner classes are useful when the class should not be visible outside the enclosing class or package.

### **Conclusion**

- Java provides **four types** of inner classes: **Member Inner Class**, **Static Nested Class**, **Local Inner Class**, and **Anonymous Inner Class**.
- **Inner classes** are useful for logically grouping related classes and providing functionality closely tied to the outer class.
- Depending on your requirements, you can choose the appropriate type of inner class to organize and structure your code more effectively.

---

---

## Q19: Lambda Expression in Java

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

### **Advantages of Lambda Expressions**

1. **Concise and Readable**: Lambda expressions reduce boilerplate code, making it more concise and readable.
2. **Functional Programming**: They encourage the use of functional programming techniques like passing behavior as arguments to methods.
3. **Parallel Processing**: Lambda expressions make it easier to use parallel streams, improving performance with large data sets.
4. **Less Code**: Reduces the need for anonymous inner classes, making code easier to maintain.

### **Use Cases for Lambda Expressions**

- **Event Handling**: Commonly used in GUI applications (like Swing or JavaFX) to handle events.
- **Streams API**: Lambda expressions are heavily used with the Streams API for operations like filtering, mapping, and reducing collections of data.
- **Concurrency**: Used in concurrent programming for writing short, concise callbacks or runnable tasks.

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

### **Conclusion**

Lambda expressions in Java allow you to write more concise, functional-style code that is easier to read and maintain. They are particularly useful when working with functional interfaces and collections, and they enable more efficient handling of data processing tasks, such as filtering and transforming collections using the Streams API.

---

---

## Q20: Java Exception Hierarchy

### **Java Exception Hierarchy**

In Java, exceptions are used to handle errors or other exceptional conditions that may arise during program execution. The exception handling mechanism in Java is built around the `Throwable` class, which is the root of the exception hierarchy.

Here’s a breakdown of the **Exception Hierarchy** in Java, along with examples of different types of exceptions.

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

### **3. `Exception` Class**

- **Exceptions** are events that disrupt the normal flow of a program’s execution.
- Exceptions are of two types:
  1. **Checked Exceptions**: These exceptions are checked at compile-time, and you must either handle them using a try-catch block or declare them with the `throws` keyword.
  2. **Unchecked Exceptions**: These exceptions occur at runtime, and they are not checked at compile-time.

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

### **6. `RuntimeException` Class**

- `RuntimeException` is the parent class for all unchecked exceptions.
- These exceptions occur due to programming errors that could have been avoided (e.g., **`ArrayIndexOutOfBoundsException`**, **`ClassCastException`**, **`IllegalArgumentException`**, etc.).

#### **Common Subclasses of `RuntimeException`:**

- **`NullPointerException`**: Thrown when an application attempts to use `null` where an object is required.
- **`ArithmeticException`**: Thrown when an illegal arithmetic operation is performed (e.g., division by zero).
- **`IndexOutOfBoundsException`**: Thrown when an index is out of range for an array or list.

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

### **Summary of Exception Types**

| **Type**                 | **Examples**                                  | **Checked or Unchecked** |
| ------------------------ | --------------------------------------------- | ------------------------ |
| **`Error`**              | `OutOfMemoryError`, `StackOverflowError`      | Unchecked                |
| **`Exception`**          |                                               |                          |
| **Checked Exceptions**   | `IOException`, `SQLException`                 | Checked                  |
| **Unchecked Exceptions** | `NullPointerException`, `ArithmeticException` | Unchecked                |

- **Checked exceptions** must be either caught or declared in the method signature.
- **Unchecked exceptions** do not need to be explicitly handled, but it’s a good practice to avoid them in the code through proper validation.

### **Conclusion**

In Java, the **exception hierarchy** starts with `Throwable`, which is divided into **Errors** and **Exceptions**. Errors typically indicate problems with the JVM or system, while exceptions are conditions that applications may handle. Exceptions are further categorized into **checked exceptions** (which must be handled) and **unchecked exceptions** (which are runtime errors that may be ignored or handled). Understanding this hierarchy helps in writing robust programs by properly handling errors and exceptions.

---

---

## Q21: Singleton class

A **Singleton class** is a design pattern in object-oriented programming that ensures a class has only **one instance** throughout the lifetime of an application and provides a global point of access to that instance. This is useful when you need to control the access to shared resources, like a database connection, configuration settings, or a logging service.

### **Key Characteristics of a Singleton Class:**

1. **Single Instance**: Only one instance of the class exists during the application's execution.
2. **Global Access**: The instance can be accessed globally by other parts of the program.
3. **Lazy Instantiation**: The instance is created only when it is first needed (in some implementations).
4. **Thread Safety**: In multi-threaded applications, a thread-safe implementation ensures that multiple threads do not create multiple instances simultaneously.

### **Steps to Create a Singleton Class in Java**

1. **Private Constructor**: The constructor of the Singleton class is made **private** so that it cannot be instantiated directly outside the class.
2. **Static Instance**: A static reference to the single instance of the class is created.
3. **Public Method for Access**: A public static method (often called `getInstance()`) is provided to return the single instance of the class.

### **Example of Singleton Class in Java**

#### **Eager Initialization Singleton:**

In this approach, the instance is created when the class is loaded.

```java
public class Singleton {
    // Step 1: Create a static instance of the class (eager initialization)
    private static final Singleton instance = new Singleton();

    // Step 2: Private constructor to prevent instantiation from outside the class
    private Singleton() {
        // Initialize any resources if necessary
    }

    // Step 3: Public method to provide access to the instance
    public static Singleton getInstance() {
        return instance;
    }

    public void showMessage() {
        System.out.println("Hello from Singleton!");
    }
}

public class Main {
    public static void main(String[] args) {
        // Access the Singleton instance
        Singleton singleton = Singleton.getInstance();
        singleton.showMessage(); // Outputs: Hello from Singleton!
    }
}
```

**Explanation**:

- The instance `instance` is created when the class is loaded (eager initialization), ensuring only one instance exists.
- The constructor is private, so no other class can create a new instance using `new`.
- The static `getInstance()` method provides the global access point for getting the single instance.

#### **Lazy Initialization Singleton:**

In this approach, the instance is created only when it is needed for the first time.

```java
public class Singleton {
    // Step 1: Declare a static instance (not initialized immediately)
    private static Singleton instance;

    // Step 2: Private constructor to prevent instantiation from outside the class
    private Singleton() {
        // Initialize any resources if necessary
    }

    // Step 3: Public method to provide access to the instance
    public static Singleton getInstance() {
        if (instance == null) {
            // Lazy initialization: create the instance only when needed
            instance = new Singleton();
        }
        return instance;
    }

    public void showMessage() {
        System.out.println("Hello from Singleton!");
    }
}

public class Main {
    public static void main(String[] args) {
        // Access the Singleton instance
        Singleton singleton = Singleton.getInstance();
        singleton.showMessage(); // Outputs: Hello from Singleton!
    }
}
```

**Explanation**:

- The instance is **created lazily** (only when it is accessed for the first time) to save memory if it is not needed immediately.
- The `getInstance()` method checks if the instance is `null`, and if it is, it creates the instance.

#### **Thread-Safe Singleton (Double-Checked Locking)**

In a multi-threaded environment, it’s important to ensure that the Singleton class remains thread-safe, i.e., multiple threads don't create separate instances of the class.

```java
public class Singleton {
    // Step 1: Declare a static instance (not initialized immediately)
    private static volatile Singleton instance;

    // Step 2: Private constructor to prevent instantiation from outside the class
    private Singleton() {
        // Initialize any resources if necessary
    }

    // Step 3: Public method to provide access to the instance with thread safety
    public static Singleton getInstance() {
        if (instance == null) {
            synchronized (Singleton.class) {
                if (instance == null) {
                    instance = new Singleton();
                }
            }
        }
        return instance;
    }

    public void showMessage() {
        System.out.println("Hello from Singleton!");
    }
}

public class Main {
    public static void main(String[] args) {
        // Access the Singleton instance
        Singleton singleton = Singleton.getInstance();
        singleton.showMessage(); // Outputs: Hello from Singleton!
    }
}
```

**Explanation**:

- The `volatile` keyword ensures that the instance is visible across all threads.
- The `synchronized` block ensures that only one thread can enter the critical section of code at a time and create the instance, ensuring that multiple threads don't create separate instances.

### **Why Use a Singleton?**

- **Global Access**: The Singleton pattern provides a global access point for accessing a shared resource or functionality (like logging, configuration settings, database connections).
- **Controlled Instantiation**: It restricts the creation of multiple instances, preventing the wastage of resources and ensuring a consistent state.
- **Efficiency**: The singleton object is created only once and is reused throughout the program, saving memory and resources.

### **When Not to Use Singleton?**

- **Testing Challenges**: Singletons can make unit testing difficult because they maintain a global state, making it harder to test classes in isolation.
- **Concurrency Issues**: In multi-threaded applications, if not implemented correctly, the Singleton pattern can lead to issues like race conditions.
- **Overuse**: Sometimes using a Singleton pattern unnecessarily can introduce complexity or unnecessary global state.

### **Summary**

- A **Singleton class** ensures that only one instance of a class exists and provides a global point of access.
- The instance is created using a **private constructor** and accessed via a **public static method**.
- The Singleton can be implemented using **eager initialization**, **lazy initialization**, or **thread-safe techniques** such as **double-checked locking**.

---

---

## Q22: principles of Object-Oriented Programming (OOP)

1. **Encapsulation**:

   - Encapsulation is the concept of wrapping data (variables) and methods (functions) together as a single unit. It restricts access to certain details of an object and allows only controlled access through public methods (getters and setters).

2. **Abstraction**:

   - Abstraction is the process of hiding the implementation details and showing only the essential features of an object. It allows focusing on what an object does, rather than how it does it.

3. **Inheritance**:

   - Inheritance is a mechanism where a new class (subclass/child class) inherits properties and behaviors (methods) from an existing class (superclass/parent class), enabling code reuse and creating a hierarchy of classes.

4. **Polymorphism**:
   - Polymorphism allows objects of different classes to be treated as objects of a common superclass. It enables methods to be used in different ways, such as method overloading (same method name with different parameters) and method overriding (redefining a method in a subclass).

---

---

## Q23: Inheritance

### **Inheritance in Object-Oriented Programming (OOP)**

**Inheritance** is one of the fundamental concepts in object-oriented programming (OOP) that allows a new class (child or subclass) to inherit the properties and behaviors (fields and methods) from an existing class (parent or superclass). It enables code reuse, allows for hierarchical relationships between classes, and facilitates the creation of more specialized versions of a class.

### **1. What is Inheritance?**

Inheritance is a mechanism by which one class acquires the properties (fields) and behaviors (methods) of another class. The class that inherits is called the **subclass** (or **child class**), and the class being inherited from is called the **superclass** (or **parent class**). This allows the subclass to access and use the fields and methods of the superclass, extending or modifying them as needed.

In Java, inheritance is implemented using the `extends` keyword.

**Example**:

```java
// Parent class (Superclass)
class Animal {
    String name;

    public void speak() {
        System.out.println("Animal makes a sound");
    }
}

// Child class (Subclass)
class Dog extends Animal {
    public void speak() {
        System.out.println("Dog barks");
    }
}
```

In this example, the `Dog` class inherits the `speak()` method from the `Animal` class but overrides it to provide a specific implementation.

### **2. Why Use Inheritance?**

#### **Benefits of Inheritance**:

1. **Code Reusability**: Inheritance promotes code reuse by allowing a subclass to reuse the fields and methods defined in the superclass without having to rewrite the code.
2. **Extensibility**: You can easily extend existing classes with new functionality. If you have a base class with general behavior, you can create subclasses that inherit this behavior and add more specific functionality.

3. **Maintainability**: Inheritance makes it easier to update and maintain code because common features are centralized in the superclass. Changes made to the superclass can automatically reflect in all its subclasses.

4. **Hierarchical Class Structure**: Inheritance allows you to create a hierarchy of classes, where more specialized classes can be derived from more general classes. This structure models real-world relationships and is easier to understand and maintain.

5. **Polymorphism**: Inheritance enables polymorphism, where an object of a subclass can be treated as an object of its superclass. This allows for flexibility in code and the ability to use subclasses interchangeably in some situations.

### **3. How Does Inheritance Work?**

When a subclass inherits from a superclass, the subclass inherits the following:

- **Fields/Properties**: All non-private fields of the superclass (except static fields) are inherited by the subclass.
- **Methods**: The subclass inherits all non-private methods of the superclass. It can then:
  - **Override** methods to change their behavior.
  - **Use** methods as is.
  - **Call** superclass methods using the `super` keyword.

**Key Concepts in Inheritance**:

- **Method Overriding**: A subclass can provide its own implementation of a method that is already defined in its superclass.
- **`super` Keyword**: The `super` keyword is used to refer to the superclass. It can be used to:
  - Call a constructor of the superclass.
  - Access methods or fields from the superclass that are hidden or overridden.

**Example**:

```java
// Parent class (Superclass)
class Animal {
    String name;

    public Animal(String name) {
        this.name = name;
    }

    public void speak() {
        System.out.println("Animal makes a sound");
    }
}

// Child class (Subclass)
class Dog extends Animal {
    public Dog(String name) {
        super(name);  // Call the superclass constructor
    }

    public void speak() {
        System.out.println("Dog barks");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog("Buddy");
        dog.speak(); // Outputs: Dog barks
    }
}
```

- **Constructor**: The subclass can call the constructor of the superclass using `super()`.
- **Method Overriding**: The `speak()` method is overridden in the `Dog` class, and the specific implementation is called.

### **4. When Should You Use Inheritance?**

#### **When to Use Inheritance**:

1. **"Is-a" Relationship**: Inheritance is appropriate when there is a clear **"is-a"** relationship between the parent and child class. The subclass should be a specialized type of the superclass.

   - Example: A `Dog` is an `Animal`, so `Dog` should inherit from `Animal`.

2. **Code Reuse**: If you have common functionality that is shared across multiple classes, you can define it in the superclass and inherit it in the subclasses to avoid code duplication.

3. **Specialization**: When you want to create more specialized versions of an existing class, you can extend it to add specific behavior or attributes.

   - Example: A `Car` class could be the superclass, and `ElectricCar` or `SportsCar` can be specialized subclasses.

4. **Polymorphism**: Inheritance is often used in conjunction with polymorphism to allow objects of different subclasses to be treated as objects of the superclass, which can improve flexibility and extensibility.

#### **When Not to Use Inheritance**:

1. **"Has-a" Relationship**: If the relationship between classes is more of a **"has-a"** relationship (composition), inheritance may not be appropriate.
   - Example: A `Car` class does not **"is a"** `Engine` but **"has an"** `Engine`. In this case, composition (using objects as fields) is a better choice.
2. **Over-Extending**: Inheritance should not be used to force a class to inherit from another class if it doesn’t make sense in the context of the application. Avoid unnecessary deep inheritance hierarchies.

3. **Encapsulation Issues**: If you expose too much functionality through inheritance, it may compromise the encapsulation of your class, making the system more difficult to maintain or extend.

4. **Circular Inheritance**: Avoid circular inheritance, where Class A inherits from Class B and Class B inherits from Class A. This is not allowed in Java and can lead to problems.

### **Types of Inheritance in Java**

1. **Single Inheritance**: A class can inherit from only one superclass.

   - Example: `class Dog extends Animal`.

2. **Multilevel Inheritance**: A class can inherit from another class, which itself is a subclass of another class.

   - Example: `class Dog extends Animal`, and `class Labrador extends Dog`.

3. **Hierarchical Inheritance**: Multiple classes inherit from a single superclass.

   - Example: `class Dog extends Animal` and `class Cat extends Animal`.

4. **Multiple Inheritance (Not Allowed in Java)**: Java does not allow a class to inherit from more than one class directly to avoid ambiguity. However, multiple inheritance can be achieved using interfaces.

### **Summary**:

- **Inheritance** enables the creation of a new class from an existing class, promoting code reuse and providing a hierarchical relationship between classes.
- It is used to represent "is-a" relationships, create specialized versions of existing classes, and enable polymorphism.
- Inheritance works through the use of the `extends` keyword, and it allows subclasses to inherit fields and methods from the superclass.
- It should be used when the relationship between classes is logical and hierarchical, but it should not be overused or misapplied to avoid complex or difficult-to-maintain code.

---

---

## Q24: Types of Inheritance (Single, Multilevel, Hierarchical)

### **1. Single Inheritance**

**Definition**:  
Single inheritance is the simplest form of inheritance where a class (child class or subclass) inherits properties and methods from a single class (parent class or superclass). In this type of inheritance, the child class inherits all the public and protected members of the parent class and can add or override behavior as needed.

**Example**:  
In single inheritance, one class directly extends another class. The subclass can access the inherited properties and methods of the superclass, and it can also have its own additional functionality.

```java
// Parent class (Superclass)
class Animal {
    public void sound() {
        System.out.println("Animal makes a sound");
    }
}

// Child class (Subclass) inherits from Animal
class Dog extends Animal {
    public void sound() {
        System.out.println("Dog barks");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.sound(); // Outputs: Dog barks
    }
}
```

**Explanation**:

- The `Dog` class **inherits** the `sound()` method from the `Animal` class.
- The `Dog` class can override the inherited `sound()` method to provide its own behavior, as shown in the example.
- **Single inheritance** allows the `Dog` class to directly extend `Animal` and reuse its functionality.

**Key Points**:

- **Single inheritance** ensures a simpler, direct inheritance path.
- A subclass can inherit all public and protected properties and methods from a single superclass.

### **2. Multilevel Inheritance**

**Definition**:  
Multilevel inheritance occurs when a class (child class or subclass) inherits from another class, which is also a subclass of a third class. In other words, a class extends another class, which in turn extends a third class. This creates a **multi-level chain of inheritance**.

In Java, multilevel inheritance is supported, but Java does not support multiple inheritance (where a class inherits from more than one class).

**Example**:

```java
// Parent class (Superclass)
class Animal {
    public void sound() {
        System.out.println("Animal makes a sound");
    }
}

// Child class (Subclass) inherits from Animal
class Dog extends Animal {
    public void sound() {
        System.out.println("Dog barks");
    }
}

// Grandchild class (Sub-subclass) inherits from Dog
class Puppy extends Dog {
    public void sound() {
        System.out.println("Puppy whines");
    }
}

public class Main {
    public static void main(String[] args) {
        Puppy puppy = new Puppy();
        puppy.sound(); // Outputs: Puppy whines
    }
}
```

**Explanation**:

- The `Puppy` class inherits from `Dog`, which itself inherits from `Animal`.
- The `sound()` method is inherited from `Animal` and `Dog`, but it is overridden in `Puppy` to provide a specific implementation.
- **Multilevel inheritance** allows the `Puppy` class to access methods from both the `Dog` and `Animal` classes through the inheritance chain.

**Key Points**:

- **Multilevel inheritance** creates a hierarchy of classes, where a subclass can inherit from another subclass, and so on.
- The child class inherits not only from the direct superclass but also from the "ancestor" classes in the chain.
- This allows more specialized behavior to be added progressively in the chain.

### **3. Hierarchical Inheritance**

**Definition**:  
In hierarchical inheritance, multiple classes inherit from a **single parent class**. The parent class provides common functionality, and all the child classes (subclasses) inherit this functionality and can extend it with their own unique behaviors.

**Example**:

```java
// Parent class (Superclass)
class Animal {
    public void sound() {
        System.out.println("Animal makes a sound");
    }
}

// Child class 1 (Subclass) inherits from Animal
class Dog extends Animal {
    public void sound() {
        System.out.println("Dog barks");
    }
}

// Child class 2 (Subclass) inherits from Animal
class Cat extends Animal {
    public void sound() {
        System.out.println("Cat meows");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.sound(); // Outputs: Dog barks

        Cat cat = new Cat();
        cat.sound(); // Outputs: Cat meows
    }
}
```

**Explanation**:

- The `Dog` and `Cat` classes **inherit** the `sound()` method from the `Animal` class.
- Each subclass provides its own implementation of the `sound()` method, thus exhibiting **polymorphism** (same method name but different behaviors).
- **Hierarchical inheritance** allows multiple classes to share the functionality of a common superclass.

**Key Points**:

- **Hierarchical inheritance** involves one parent class having multiple child classes that inherit from it.
- All child classes inherit the properties and methods from the parent class, but each subclass can have its own unique behavior.
- This pattern is useful when you have several different types of objects that share common behavior.

### **Comparison of Single, Multilevel, and Hierarchical Inheritance**

| **Feature**               | **Single Inheritance**                         | **Multilevel Inheritance**                                              | **Hierarchical Inheritance**                                        |
| ------------------------- | ---------------------------------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------- |
| **Definition**            | A class inherits from a single parent class.   | A class inherits from another subclass, forming a chain of inheritance. | Multiple classes inherit from a single parent class.                |
| **Example**               | `class Dog extends Animal;`                    | `class Puppy extends Dog;`                                              | `class Dog extends Animal; class Cat extends Animal;`               |
| **Inheritance Hierarchy** | Direct parent-child relationship.              | Multiple levels of inheritance forming a chain.                         | A common parent class shared by multiple child classes.             |
| **Use Case**              | Simple inheritance for basic use cases.        | Specializing behavior progressively in a hierarchy.                     | Shared functionality among multiple subclasses.                     |
| **Polymorphism**          | Yes (methods can be overridden).               | Yes (methods can be overridden in any level).                           | Yes (methods can be overridden in each subclass).                   |
| **Code Reusability**      | Allows reuse of code from a single superclass. | Reuses code from all the ancestors in the chain.                        | Reuses common code from a single superclass in multiple subclasses. |

### **When to Use Each Type of Inheritance?**

1. **Single Inheritance**:

   - Use when there is a direct "is-a" relationship between the classes.
   - Example: A `Dog` is an `Animal`. It makes sense for `Dog` to inherit from `Animal`.

2. **Multilevel Inheritance**:

   - Use when you need to build upon a class incrementally, adding more specific behaviors at each level.
   - Example: A `Puppy` is a `Dog`, and a `Dog` is an `Animal`.

3. **Hierarchical Inheritance**:
   - Use when several classes share common behavior and can be generalized under a single superclass.
   - Example: Both `Dog` and `Cat` are `Animals`, so they share common properties and behaviors from the `Animal` class.

### **Conclusion**

- **Single Inheritance** is the simplest form of inheritance where one class extends another.
- **Multilevel Inheritance** forms a chain of inheritance where a subclass inherits from another subclass.
- **Hierarchical Inheritance** allows multiple subclasses to inherit from a single parent class, promoting code reuse across various classes.

Each type of inheritance has its use cases and helps to create a more organized, modular, and extensible codebase by leveraging the hierarchical nature of classes.

---

---

## Q25: super Keyword in Java

### **`super` Keyword in Java**

The `super` keyword in Java is used in the context of inheritance. It is a reference variable used to refer to the **parent class** (superclass) in the following cases:

1. **To access parent class methods**: It is used to call methods from the parent class, especially if they are overridden by the subclass.
2. **To access parent class constructor**: It is used to call the constructor of the parent class.
3. **To access parent class fields**: It can be used to refer to parent class variables if they are shadowed by subclass variables.

### **1. Accessing Parent Class Methods Using `super`**

If a method in the subclass overrides a method in the parent class, and you still want to call the parent class’s version of the method, you can use `super` to refer to the parent class method.

**Example**:

```java
class Animal {
    public void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("Dog barks");
    }

    public void callSuperMethod() {
        super.sound();  // Calls the sound() method of Animal (parent class)
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.sound();  // Outputs: Dog barks
        dog.callSuperMethod();  // Outputs: Animal makes a sound
    }
}
```

**Explanation**:

- The `Dog` class overrides the `sound()` method.
- Inside the `callSuperMethod()` of the `Dog` class, we use `super.sound()` to call the `sound()` method from the `Animal` class, which is the superclass.

### **2. Accessing Parent Class Constructor Using `super`**

The `super()` keyword is used to call the constructor of the parent class. This is especially useful when the parent class has a constructor with arguments that needs to be called by the subclass constructor.

If you don't explicitly call a parent class constructor using `super()`, Java automatically inserts a default call to `super()` (no-argument constructor) in the subclass constructor.

**Example**:

```java
class Animal {
    String name;

    // Constructor of parent class
    public Animal(String name) {
        this.name = name;
    }

    public void showName() {
        System.out.println("Animal name: " + name);
    }
}

class Dog extends Animal {

    // Constructor of child class
    public Dog(String name) {
        super(name);  // Calls the constructor of Animal
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog("Buddy");
        dog.showName();  // Outputs: Animal name: Buddy
    }
}
```

**Explanation**:

- The `Animal` class has a constructor that takes a `String name` argument.
- In the `Dog` class, the constructor `super(name)` is used to call the constructor of the `Animal` class and initialize the `name` property.
- This way, the subclass (`Dog`) can invoke the constructor of the superclass (`Animal`).

### **3. Accessing Parent Class Fields Using `super`**

If the subclass has a field with the same name as a field in the parent class (a concept known as **shadowing**), `super` can be used to refer to the parent class field.

**Example**:

```java
class Animal {
    String name = "Generic Animal";
}

class Dog extends Animal {
    String name = "Buddy";

    public void displayNames() {
        System.out.println("Child class name: " + name);      // Prints "Buddy"
        System.out.println("Parent class name: " + super.name); // Prints "Generic Animal"
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.displayNames();
    }
}
```

**Explanation**:

- Both the `Animal` and `Dog` classes have a `name` field.
- The `super.name` is used to refer to the `name` field of the `Animal` class (the parent class), while just `name` refers to the `name` field in the `Dog` class (the child class).

### **4. Important Points About `super`**

- **Calling parent constructor**: If the superclass has a constructor with parameters, you can use `super(parameters)` to invoke it. If the superclass doesn't have a no-argument constructor, you **must** call a constructor of the superclass with arguments using `super()` in the subclass constructor.
- **Invoking overridden methods**: If a method is overridden in a subclass and you want to call the original method from the superclass, you can use `super.methodName()`.

- **Accessing parent fields**: If a field in the subclass shadows a field in the superclass, you can access the superclass’s field using `super.fieldName`.

- **Super in Constructor Chaining**: In the constructor of a subclass, the `super()` call can be used to pass arguments to the parent class’s constructor. It must be the first statement in the subclass constructor.

- **Accessing super-class variables**: You can also use `super` to access non-private variables of the superclass.

### **Example: Using `super` for Constructor Chaining and Method Access**

```java
class Person {
    String name;

    public Person(String name) {
        this.name = name;
    }

    public void greet() {
        System.out.println("Hello, my name is " + name);
    }
}

class Employee extends Person {
    String designation;

    // Constructor chaining
    public Employee(String name, String designation) {
        super(name);  // Call the constructor of Person
        this.designation = designation;
    }

    // Overriding greet method
    @Override
    public void greet() {
        super.greet();  // Call greet method of Person
        System.out.println("I work as " + designation);
    }
}

public class Main {
    public static void main(String[] args) {
        Employee employee = new Employee("John", "Software Engineer");
        employee.greet();
    }
}
```

**Output**:

```
Hello, my name is John
I work as Software Engineer
```

**Explanation**:

- The `Employee` class constructor calls the `super(name)` constructor of the `Person` class to initialize the `name` property.
- The `greet()` method is overridden in the `Employee` class, but it first calls the `greet()` method of the `Person` class using `super.greet()` to maintain the base functionality.

### **Summary of `super` Uses**:

- **Calling parent class methods**: `super.methodName()`
- **Calling parent class constructor**: `super(parameters)` (must be the first statement in the subclass constructor)
- **Accessing parent class fields**: `super.fieldName`
- **Constructor chaining**: `super()` to invoke the constructor of the parent class.

The `super` keyword is crucial for working with inheritance in Java, allowing subclasses to leverage the functionality and fields of the parent class while also allowing them to extend or modify that functionality.

---

---

## Q26: Polymorphism in Java

Polymorphism is one of the fundamental concepts in **Object-Oriented Programming (OOP)**. It allows one interface to be used for different data types, meaning the same method or function can behave differently based on the object calling it. Polymorphism enhances the flexibility and reusability of code.

The term "polymorphism" is derived from Greek, meaning "many shapes" (poly = many, morph = form/shape). In Java, polymorphism allows you to perform the same operation on different objects, but each object can respond differently to the operation.

### **Types of Polymorphism in Java**

There are **two main types of polymorphism** in Java:

1. **Compile-Time Polymorphism** (also called **Static Polymorphism**)
2. **Run-Time Polymorphism** (also called **Dynamic Polymorphism**)

### **1. Compile-Time Polymorphism (Static Polymorphism)**

**Definition**:  
Compile-time polymorphism occurs when the method to be called is determined at compile time. This type of polymorphism is achieved using **method overloading** and **operator overloading**. However, Java doesn't support operator overloading, so we focus on **method overloading**.

**Method Overloading**:  
Method overloading is when two or more methods in the same class have the same name but different parameters (either in the number of parameters or their types).

**Key Characteristics**:

- Occurs at compile-time.
- Achieved through method overloading (same method name, different parameters).
- The decision about which method to invoke is made at the time of compilation.

**Example**:

```java
class Printer {
    // Overloaded method for printing a string
    public void print(String s) {
        System.out.println(s);
    }

    // Overloaded method for printing an integer
    public void print(int num) {
        System.out.println(num);
    }

    // Overloaded method for printing a double
    public void print(double d) {
        System.out.println(d);
    }
}

public class Main {
    public static void main(String[] args) {
        Printer printer = new Printer();
        printer.print("Hello, World!");  // Calls the print(String) method
        printer.print(100);              // Calls the print(int) method
        printer.print(99.99);            // Calls the print(double) method
    }
}
```

**Explanation**:

- The `Printer` class has three overloaded methods named `print()`, each accepting different parameter types (String, int, and double).
- When you call `printer.print()`, Java will determine which version of the `print()` method to invoke based on the type of argument passed at compile-time.

**Output**:

```
Hello, World!
100
99.99
```

**Key Point**:

- The method that gets invoked is determined at compile-time based on the arguments passed.

### **2. Run-Time Polymorphism (Dynamic Polymorphism)**

**Definition**:  
Run-time polymorphism is when the method to be called is determined at **runtime**. It occurs when a subclass overrides a method from the parent class, and the method invocation is resolved at runtime depending on the object type (not the reference type).

**Method Overriding**:  
Method overriding occurs when a subclass provides its own implementation of a method that is already defined in its superclass. The version of the overridden method that gets invoked is determined at runtime based on the object type, not the reference type.

**Key Characteristics**:

- Occurs at runtime.
- Achieved through method overriding (same method signature in both parent and child classes).
- The method that gets invoked is determined dynamically based on the object type at runtime.

**Example**:

```java
class Animal {
    public void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("Dog barks");
    }
}

class Cat extends Animal {
    @Override
    public void sound() {
        System.out.println("Cat meows");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal1 = new Dog();  // Reference of Animal, object of Dog
        Animal animal2 = new Cat();  // Reference of Animal, object of Cat

        animal1.sound();  // Outputs: Dog barks (Method resolved at runtime)
        animal2.sound();  // Outputs: Cat meows (Method resolved at runtime)
    }
}
```

**Explanation**:

- The `sound()` method is overridden in both the `Dog` and `Cat` classes.
- Even though the reference type is `Animal` for both `animal1` and `animal2`, the actual method that gets called depends on the object type (`Dog` or `Cat`) at runtime.

**Output**:

```
Dog barks
Cat meows
```

**Key Point**:

- The method that gets invoked is determined at runtime, depending on the actual object type (not the reference type).

### **Key Differences Between Compile-Time and Run-Time Polymorphism**

| **Feature**              | **Compile-Time Polymorphism**                                | **Run-Time Polymorphism**                                            |
| ------------------------ | ------------------------------------------------------------ | -------------------------------------------------------------------- |
| **Method**               | Achieved by **method overloading**.                          | Achieved by **method overriding**.                                   |
| **Time of Binding**      | The method to be called is bound during **compile-time**.    | The method to be called is bound during **runtime**.                 |
| **Polymorphic Behavior** | Method resolution is based on the **method signature**.      | Method resolution is based on the **object type** at runtime.        |
| **Example**              | Method overloading (same method name, different parameters). | Method overriding (same method signature, different implementation). |
| **Type of Binding**      | **Static binding** (early binding).                          | **Dynamic binding** (late binding).                                  |

### **Advantages of Polymorphism**

1. **Flexibility**: Polymorphism allows a single method to perform different tasks based on the object type, making it easier to extend and maintain the code.
2. **Code Reusability**: With polymorphism, the same code can work with different objects, which reduces redundancy.
3. **Ease of Maintenance**: If you need to change the behavior of a method, you only need to update the method in the subclass instead of all places the method is used.
4. **Simplified Code**: Polymorphism helps in reducing the complexity of code by enabling a more generic and reusable interface.

### **Real-World Example of Polymorphism**

Consider a scenario where you have multiple shapes (circle, rectangle, etc.), and each shape needs to calculate its area. You can create a common interface (or abstract class) `Shape` and use polymorphism to handle different shapes without changing the code structure.

```java
abstract class Shape {
    abstract void area();  // Abstract method to be overridden by subclasses
}

class Circle extends Shape {
    double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    @Override
    void area() {
        System.out.println("Area of Circle: " + (Math.PI * radius * radius));
    }
}

class Rectangle extends Shape {
    double length, width;

    public Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    @Override
    void area() {
        System.out.println("Area of Rectangle: " + (length * width));
    }
}

public class Main {
    public static void main(String[] args) {
        Shape shape1 = new Circle(5);  // Create a Circle object
        Shape shape2 = new Rectangle(4, 6);  // Create a Rectangle object

        shape1.area();  // Outputs: Area of Circle: 78.53981633974483
        shape2.area();  // Outputs: Area of Rectangle: 24.0
    }
}
```

**Explanation**:

- The `Shape` class is abstract and contains an abstract method `area()`.
- The `Circle` and `Rectangle` classes implement the `area()` method in their own way.
- The method `area()` is called polymorphically on different types of `Shape` objects (`Circle` and `Rectangle`).

**Output**:

```
Area of Circle: 78.53981633974483
Area of Rectangle: 24.0
```

### **Conclusion**

Polymorphism is a powerful concept in Java that allows the same method to behave differently based on the object it is invoked on. It provides flexibility, maintainability, and extensibility to object-oriented systems by enabling dynamic method resolution. Polymorphism can be achieved through **method overloading** (compile-time) and **method overriding** (run-time).

---

---

## Q27: Real-World Examples of Polymorphism

Here are **multiple scenarios** demonstrating **Polymorphism** in Java, showcasing different use cases:

### **1. Scenario: Polymorphism with Method Overloading (Compile-Time Polymorphism)**

**Scenario**: A calculator that can perform addition on different data types (int, double, and String).

**Example**:

```java
class Calculator {
    // Method for adding two integers
    public int add(int a, int b) {
        return a + b;
    }

    // Overloaded method for adding two doubles
    public double add(double a, double b) {
        return a + b;
    }

    // Overloaded method for concatenating two strings
    public String add(String a, String b) {
        return a + b;
    }
}

public class Main {
    public static void main(String[] args) {
        Calculator calculator = new Calculator();

        // Using method with integer arguments
        System.out.println("Addition of integers: " + calculator.add(5, 10));

        // Using method with double arguments
        System.out.println("Addition of doubles: " + calculator.add(5.5, 10.5));

        // Using method with string arguments
        System.out.println("Concatenation of strings: " + calculator.add("Hello, ", "World!"));
    }
}
```

**Explanation**:

- This example shows **method overloading**, where the `add()` method is defined multiple times with different argument types (int, double, String).
- The correct method is selected at **compile-time** based on the argument types passed.

**Output**:

```
Addition of integers: 15
Addition of doubles: 16.0
Concatenation of strings: Hello, World!
```

### **2. Scenario: Polymorphism with Method Overriding (Run-Time Polymorphism)**

**Scenario**: A zoo where animals (such as a Dog and a Cat) make different sounds, but we use a common reference to call the sound method.

**Example**:

```java
class Animal {
    public void sound() {
        System.out.println("Animals make sounds");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("Dog barks");
    }
}

class Cat extends Animal {
    @Override
    public void sound() {
        System.out.println("Cat meows");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal1 = new Dog();  // Reference of Animal, object of Dog
        Animal animal2 = new Cat();  // Reference of Animal, object of Cat

        animal1.sound();  // Outputs: Dog barks (Method resolved at runtime)
        animal2.sound();  // Outputs: Cat meows (Method resolved at runtime)
    }
}
```

**Explanation**:

- **Method overriding** is used in this example, where the `sound()` method is overridden in both the `Dog` and `Cat` classes.
- At runtime, the **actual object type** (`Dog` or `Cat`) determines which `sound()` method gets called, even though the reference type is `Animal`.

**Output**:

```
Dog barks
Cat meows
```

### **3. Scenario: Polymorphism with Abstract Classes (Run-Time Polymorphism)**

**Scenario**: An abstract class `Shape` with different shapes (Circle, Rectangle) that calculate their area.

**Example**:

```java
abstract class Shape {
    // Abstract method to calculate area
    abstract void area();
}

class Circle extends Shape {
    double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    @Override
    void area() {
        System.out.println("Area of Circle: " + (Math.PI * radius * radius));
    }
}

class Rectangle extends Shape {
    double length, width;

    public Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    @Override
    void area() {
        System.out.println("Area of Rectangle: " + (length * width));
    }
}

public class Main {
    public static void main(String[] args) {
        Shape shape1 = new Circle(5);     // Reference of Shape, object of Circle
        Shape shape2 = new Rectangle(4, 6); // Reference of Shape, object of Rectangle

        shape1.area();  // Outputs: Area of Circle: 78.53981633974483
        shape2.area();  // Outputs: Area of Rectangle: 24.0
    }
}
```

**Explanation**:

- An abstract class `Shape` defines an abstract method `area()`, which is implemented in the subclasses (`Circle`, `Rectangle`).
- The actual method `area()` is determined at **runtime** based on the object type (`Circle` or `Rectangle`).

**Output**:

```
Area of Circle: 78.53981633974483
Area of Rectangle: 24.0
```

### **4. Scenario: Polymorphism in Interface Implementation (Run-Time Polymorphism)**

**Scenario**: A `Payment` interface that defines a method `pay()`, and different payment methods like `CreditCard` and `PayPal` that implement the `pay()` method.

**Example**:

```java
interface Payment {
    void pay();
}

class CreditCard implements Payment {
    @Override
    public void pay() {
        System.out.println("Payment made using Credit Card");
    }
}

class PayPal implements Payment {
    @Override
    public void pay() {
        System.out.println("Payment made using PayPal");
    }
}

public class Main {
    public static void main(String[] args) {
        Payment payment1 = new CreditCard();  // Reference of Payment, object of CreditCard
        Payment payment2 = new PayPal();      // Reference of Payment, object of PayPal

        payment1.pay();  // Outputs: Payment made using Credit Card
        payment2.pay();  // Outputs: Payment made using PayPal
    }
}
```

**Explanation**:

- The `Payment` interface defines the `pay()` method.
- Both `CreditCard` and `PayPal` classes implement the `pay()` method in their own way.
- The method `pay()` is determined at **runtime** based on the actual object (`CreditCard` or `PayPal`).

**Output**:

```
Payment made using Credit Card
Payment made using PayPal
```

### **5. Scenario: Polymorphism in Constructor Overloading (Compile-Time Polymorphism)**

**Scenario**: A `Person` class with different constructors that accept various parameters.

**Example**:

```java
class Person {
    String name;
    int age;

    // Constructor with name parameter
    public Person(String name) {
        this.name = name;
    }

    // Constructor with name and age parameters
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public void display() {
        System.out.println("Name: " + name + ", Age: " + age);
    }
}

public class Main {
    public static void main(String[] args) {
        Person person1 = new Person("Alice");           // Using constructor with name only
        Person person2 = new Person("Bob", 30);         // Using constructor with name and age

        person1.display();  // Outputs: Name: Alice, Age: 0
        person2.display();  // Outputs: Name: Bob, Age: 30
    }
}
```

**Explanation**:

- The `Person` class has two constructors: one accepts only the name, and the other accepts both the name and age.
- The appropriate constructor is chosen based on the number of arguments at **compile-time**.

**Output**:

```
Name: Alice, Age: 0
Name: Bob, Age: 30
```

### **6. Scenario: Polymorphism in Collections (Run-Time Polymorphism)**

**Scenario**: Storing different types of animals in a list and invoking their `sound()` method.

**Example**:

```java
import java.util.ArrayList;

class Animal {
    public void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("Dog barks");
    }
}

class Cat extends Animal {
    @Override
    public void sound() {
        System.out.println("Cat meows");
    }
}

public class Main {
    public static void main(String[] args) {
        ArrayList<Animal> animals = new ArrayList<>();
        animals.add(new Dog());
        animals.add(new Cat());

        for (Animal animal : animals) {
            animal.sound();  // The correct method is called based on the actual object type
        }
    }
}
```

**Explanation**:

- In this scenario, different animal types (`Dog` and `Cat`) are stored in a **single collection** (`ArrayList<Animal>`).
- The method `sound()` is invoked polymorphically, and the correct method (based on the actual object) is called at **runtime**.

**Output**:

```
Dog barks
Cat meows
```

### **Summary**

- **Compile-Time Polymorphism (Method Overloading)**: Allows the same method to behave differently based on the number or type of parameters.
- **Run-Time Polymorphism (Method Overriding)**: Allows a method to be dynamically dispatched based on the actual object type, even when accessed via a superclass reference.

These different scenarios show how polymorphism allows you to write more flexible and reusable code, whether by choosing methods at compile time or resolving method calls at runtime.

---

---

## Q28: Explain this concept `Parent person1 = new Child("Drawing", 12);` type `Parent person1` is different and object `Child("Drawing", 12)` is different ?

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

## Q29: Explain this concept `Child person1 = new Parent("Drawing", 12);` type `Child person1` is different subclass and object `Parent("Drawing", 12)` is different parent class ?

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

## Q30: Method Overriding in Java

### **Method Overriding in Java**

**Method Overriding** is a feature in Java that allows a subclass to provide a specific implementation of a method that is already defined in its superclass. The **overridden method** in the subclass should have the same method signature (name, return type, and parameters) as the method in the superclass.

### **Key Points of Method Overriding:**

1. **Same Method Signature**: The method in the subclass must have the same name, return type, and parameters as the method in the superclass.
2. **Runtime Polymorphism**: Overriding is related to **runtime polymorphism**, where the actual method to be called is determined at runtime based on the object’s type (the instance on which the method is called).
3. **Inheritance**: Overriding works in the context of inheritance. The subclass inherits the method from the superclass but can choose to override it to provide a different behavior.
4. **@Override Annotation**: In Java, you can use the `@Override` annotation to explicitly indicate that a method is overriding a method from the superclass. This helps to avoid errors like mismatching method signatures.

### **How Overriding Works**

When you call a method on an object, Java first checks the actual class of the object, not the reference type, to determine which version of the method to invoke. If the method is overridden in the subclass, the version in the subclass is invoked. If it is not overridden, the method in the superclass is called.

### **Syntax of Method Overriding**

```java
class Superclass {
    public void display() {
        System.out.println("Display method from Superclass");
    }
}

class Subclass extends Superclass {
    @Override
    public void display() {
        System.out.println("Display method from Subclass");
    }
}

public class Main {
    public static void main(String[] args) {
        Superclass obj = new Subclass();
        obj.display();  // Output: Display method from Subclass
    }
}
```

### **Explanation:**

1. **Superclass** has a method `display()`.
2. **Subclass** overrides this method using the same signature and provides its own implementation.
3. In the `main` method, we create an object of type `Superclass`, but it actually refers to an object of type `Subclass` (`Superclass obj = new Subclass();`).
4. When the `display()` method is called on this object (`obj.display();`), Java uses the **actual object type** (`Subclass`) to determine the method to invoke.
5. The output will be **"Display method from Subclass"**, as the `display()` method is overridden in `Subclass`.

### **When is Method Overriding Used?**

1. **Behavior Modification**: When you want to modify or extend the behavior of a superclass method in a subclass.
2. **Runtime Polymorphism**: To allow different behaviors for the same method call, depending on the object’s actual class.
3. **Method Signature Consistency**: In situations where you need to ensure that a method's signature in the subclass remains the same as the superclass.

### **Important Rules of Method Overriding**

1. **Access Modifiers**: The access level of the overriding method in the subclass cannot be more restrictive than the overridden method in the superclass. For example, if the superclass method is `public`, the subclass method must also be `public` (or more permissive). It cannot be `private` or `protected`.

   - Valid:

     ```java
     class Superclass {
         public void display() { ... }
     }

     class Subclass extends Superclass {
         public void display() { ... }  // Valid: same access level
     }
     ```

   - Invalid:

     ```java
     class Superclass {
         public void display() { ... }
     }

     class Subclass extends Superclass {
         private void display() { ... }  // Invalid: cannot be more restrictive
     }
     ```

2. **Return Type**: The return type of the overridden method must be the same as or a subtype of the return type of the original method (covariant return type).

   - Valid:

     ```java
     class Superclass {
         public Number getNumber() {
             return 5;
         }
     }

     class Subclass extends Superclass {
         @Override
         public Integer getNumber() {  // Valid: Integer is a subtype of Number
             return 10;
         }
     }
     ```

   - Invalid:

     ```java
     class Superclass {
         public Number getNumber() {
             return 5;
         }
     }

     class Subclass extends Superclass {
         @Override
         public String getNumber() {  // Invalid: String is not a subtype of Number
             return "Hello";
         }
     }
     ```

3. **Static Methods**: Static methods cannot be overridden. They can be **shadowed** in the subclass, but they are not polymorphic and are resolved at compile time based on the reference type.

   - Example of **method hiding** (not overriding):

     ```java
     class Superclass {
         public static void display() {
             System.out.println("Display from Superclass");
         }
     }

     class Subclass extends Superclass {
         public static void display() {
             System.out.println("Display from Subclass");
         }
     }

     public class Main {
         public static void main(String[] args) {
             Superclass obj = new Subclass();
             obj.display();  // Output: Display from Superclass (resolved at compile-time)
         }
     }
     ```

4. **Final Methods**: A method that is marked `final` cannot be overridden in the subclass.

   - Example:

     ```java
     class Superclass {
         public final void display() {
             System.out.println("Display from Superclass");
         }
     }

     class Subclass extends Superclass {
         // Error: Cannot override the final method from Superclass
         public void display() {
             System.out.println("Display from Subclass");
         }
     }
     ```

### **Advantages of Method Overriding**

1. **Flexibility**: Method overriding enables the creation of flexible and reusable code by allowing subclass-specific behaviors while maintaining the common interface from the superclass.
2. **Runtime Polymorphism**: Allows the use of the same method name for different objects, enabling dynamic behavior depending on the object’s actual class at runtime.
3. **Extensibility**: Overriding allows the behavior of an existing method to be changed without modifying the superclass code, making it easier to extend functionality.

### **Conclusion**

Method overriding is a fundamental concept in object-oriented programming, promoting **runtime polymorphism** and **code reusability**. It allows subclasses to define specific implementations of methods that are already defined in the superclass, providing a way to alter or extend the behavior of inherited methods.

---

---

## Q31: Can we override static methods

In Java, **static methods cannot be overridden**. However, static methods can be **hidden** in a subclass. This is an important distinction.

### **Why Static Methods Cannot Be Overridden**

1. **Static methods are resolved at compile-time**: Static methods are associated with the class itself, not with an instance of the class. When you call a static method, the method that is invoked is determined at **compile-time** based on the reference type, not the actual object type.
2. **No polymorphism with static methods**: Since static methods are not tied to object instances, they do not exhibit polymorphism. Overriding in Java is based on dynamic method dispatch, which works with instance methods, not static ones.

### **Static Method Hiding**

While static methods cannot be overridden, they can be **hidden** by a subclass. This means that if a subclass defines a static method with the same signature as a static method in its superclass, it will "hide" the superclass method. However, the method resolution will still depend on the reference type, not the object type, and it will be resolved at **compile-time**.

### **Example of Static Method Hiding**

```java
class Superclass {
    // Static method in superclass
    public static void display() {
        System.out.println("Display from Superclass");
    }
}

class Subclass extends Superclass {
    // Static method in subclass with the same signature (method hiding)
    public static void display() {
        System.out.println("Display from Subclass");
    }
}

public class Main {
    public static void main(String[] args) {
        Superclass obj1 = new Superclass();
        Superclass obj2 = new Subclass();
        Subclass obj3 = new Subclass();

        obj1.display(); // Output: Display from Superclass
        obj2.display(); // Output: Display from Superclass (resolved at compile-time)
        obj3.display(); // Output: Display from Subclass
    }
}
```

### **Explanation of the Example**:

- **`obj1.display();`** calls the `display()` method from `Superclass`, as the reference is of type `Superclass`.
- **`obj2.display();`** calls the `display()` method from `Superclass`, even though the actual object is of type `Subclass`. This happens because the reference type is `Superclass`, and static methods are resolved based on the reference type at compile-time.
- **`obj3.display();`** calls the `display()` method from `Subclass`, because the reference is of type `Subclass`.

### **Key Takeaways**:

1. **Static methods are not overridden**, but they can be **hidden** in the subclass by defining a static method with the same signature.
2. **Method hiding** with static methods is resolved at **compile-time** based on the reference type, not at runtime like instance methods.
3. Static methods do not exhibit the behavior of **polymorphism** and **dynamic dispatch**, which are central to method overriding.

In summary, static methods can be hidden, but not overridden, in Java. The choice between method hiding and overriding depends on whether the method is static or instance-based.

---

---

## Q32: Encapsulation in Java

### **Encapsulation in Java**

**Encapsulation** is one of the fundamental principles of Object-Oriented Programming (OOP). It refers to the concept of **bundling** the data (variables) and the methods (functions) that operate on the data into a single unit, typically a **class**, and restricting access to certain details of the object’s implementation. This helps in protecting the internal state of an object and only exposing what is necessary for the outside world.

### **Key Concepts of Encapsulation:**

1. **Data Hiding**: Encapsulation allows you to hide the internal details of an object and only expose a controlled interface for interaction with the object. This ensures that the object's state cannot be directly modified by outside entities, which helps to maintain data integrity.

2. **Access Control**: Through encapsulation, you can control the access level to the object's data using **access modifiers** such as `private`, `protected`, and `public`. This allows you to restrict direct access to some fields while providing controlled access via methods.

3. **Getter and Setter Methods**: To expose the internal data in a safe manner, we provide **getter** and **setter** methods. These methods allow controlled access to private variables, either for reading (getter) or modifying (setter).

4. **Abstraction**: Encapsulation also helps in abstraction by hiding the implementation details. The user of the object doesn’t need to know how the data is being stored or modified, only how to interact with the object through the provided methods.

### **Why Encapsulation is Important:**

1. **Control over data**: It provides more control over the data by preventing external code from directly modifying the object's internal state.
2. **Data Integrity**: By controlling how the internal data is accessed and modified, encapsulation helps to ensure that the object’s state remains valid and consistent.
3. **Security**: Sensitive information can be hidden and access to it can be restricted. Only the necessary methods are exposed to interact with the object.

4. **Modularity**: The internal implementation of the object can be changed without affecting the code that uses the object. Only the public interface (methods) needs to remain consistent.

5. **Ease of Maintenance**: Since the internal workings of the class are hidden, you can change the internal implementation without affecting other parts of the application.

### **How Encapsulation Works:**

1. **Private Fields**: The instance variables (fields) of a class are marked as `private` so that they cannot be directly accessed from outside the class.
2. **Public Getter/Setter Methods**: Public methods are provided to access and modify these private fields. These methods serve as the interface to interact with the object.

### **Example of Encapsulation in Java:**

```java
class Person {
    // Private fields (data is hidden)
    private String name;
    private int age;

    // Getter for 'name'
    public String getName() {
        return name;
    }

    // Setter for 'name'
    public void setName(String name) {
        this.name = name;
    }

    // Getter for 'age'
    public int getAge() {
        return age;
    }

    // Setter for 'age'
    public void setAge(int age) {
        if (age > 0) {  // Ensuring age is positive
            this.age = age;
        } else {
            System.out.println("Age must be positive.");
        }
    }
}

public class Main {
    public static void main(String[] args) {
        // Creating an object of Person
        Person person = new Person();

        // Using setter methods to set values
        person.setName("John");
        person.setAge(25);

        // Using getter methods to get values
        System.out.println("Name: " + person.getName());
        System.out.println("Age: " + person.getAge());
    }
}
```

### **Explanation of the Example:**

1. **Private Fields**: The fields `name` and `age` are declared `private`, so they cannot be accessed directly from outside the `Person` class.
2. **Public Getter/Setter Methods**:

   - The `setName()` method allows us to modify the `name` field.
   - The `setAge()` method allows us to modify the `age` field, but it also contains validation to ensure that the age is positive.
   - The `getName()` and `getAge()` methods provide access to these private fields.

3. **Encapsulation in Action**: Outside of the `Person` class, we are not able to directly change the `name` or `age` fields. Instead, we use the provided setter and getter methods to interact with the object's data.

### **Advantages of Encapsulation:**

1. **Better Control Over Data**: By restricting access to the data fields and using getter/setter methods, we have full control over how the data is accessed or modified. This can help us validate input or change the data format before storing it.

2. **Increased Flexibility and Maintainability**: The internal implementation of a class can change without affecting external code. For example, you can change the way the data is stored (e.g., change from an `int` to a `double`) without modifying the code that uses the class, as long as the getter/setter methods stay the same.

3. **Improved Security**: Sensitive information can be kept private, and access can be controlled more securely. For example, you can restrict writing to a particular field while still allowing reading.

4. **Easy Debugging**: Since data is accessed and modified only through setter and getter methods, you can insert breakpoints, log statements, or validation checks within these methods to track or debug issues easily.

5. **Reduced Complexity**: The user of a class does not need to know the internal details of how data is stored. They only interact with the exposed methods, which reduces complexity and makes the code easier to understand.

### **Disadvantages of Encapsulation:**

1. **More Code**: Encapsulation requires writing additional getter and setter methods, which can increase the lines of code and make the code more verbose.
2. **Potential for Overhead**: If there is too much encapsulation with unnecessary getter and setter methods, it might add some complexity or unnecessary overhead to the design.

3. **Not Always Necessary**: In certain cases, direct access to fields might be more straightforward, especially for small programs or for classes that do not require complex data validation.

### **Real-world Example of Encapsulation**

Consider a **Bank Account** class:

- The bank account balance (`balance`) should not be directly accessible, as it needs to be manipulated in a controlled way (e.g., adding money or withdrawing money).
- You would provide methods like `deposit()` and `withdraw()` to interact with the balance and ensure that the balance never goes below zero or some other business rule.

```java
class BankAccount {
    private double balance;

    public double getBalance() {
        return balance;
    }

    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        } else {
            System.out.println("Deposit amount must be positive.");
        }
    }

    public void withdraw(double amount) {
        if (amount > 0 && balance >= amount) {
            balance -= amount;
        } else {
            System.out.println("Invalid withdrawal amount.");
        }
    }
}

public class Main {
    public static void main(String[] args) {
        BankAccount account = new BankAccount();

        account.deposit(500);
        account.withdraw(100);

        System.out.println("Current balance: " + account.getBalance());
    }
}
```

In this case, the `balance` is encapsulated. It can only be accessed and modified via the `deposit()` and `withdraw()` methods, ensuring the account balance remains consistent and following the necessary business logic.

### **Conclusion**

Encapsulation is a key concept in Java that improves data security, modularity, and code maintainability. By hiding the internal details of an object and exposing only necessary methods to interact with it, encapsulation allows for controlled access to the object's data and ensures that the object remains in a valid state. It leads to cleaner, more maintainable, and flexible code, making it easier to modify and extend the system without affecting other components.

---

---

## Q34: Real-World Examples of Encapsulation

### **Real-World Examples of Encapsulation**

Here are a few real-world scenarios that demonstrate the concept of **Encapsulation** in an easy-to-understand manner:

### **1. Bank Account**

In the real world, when you open a bank account, you can't directly change your balance by yourself. Instead, you interact with the bank through methods like **deposit** and **withdraw**, which control how your balance is updated.

#### **Encapsulation Concept in Bank Account:**

- **Private Fields**: The bank account balance should be private and not directly accessible from outside the class.
- **Public Methods (Getter/Setter)**: Methods like `deposit()` and `withdraw()` control how the balance is modified.

```java
class BankAccount {
    private double balance;

    // Getter method to access balance
    public double getBalance() {
        return balance;
    }

    // Method to deposit money
    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        } else {
            System.out.println("Amount to deposit must be positive.");
        }
    }

    // Method to withdraw money
    public void withdraw(double amount) {
        if (amount > 0 && balance >= amount) {
            balance -= amount;
        } else {
            System.out.println("Invalid withdrawal or insufficient balance.");
        }
    }
}

public class Main {
    public static void main(String[] args) {
        BankAccount account = new BankAccount();
        account.deposit(500);
        account.withdraw(200);
        System.out.println("Balance: " + account.getBalance());
    }
}
```

### **Explanation**:

- The `balance` is hidden and can't be directly accessed.
- The `deposit()` and `withdraw()` methods ensure that balance is updated correctly, following business rules (e.g., not allowing negative deposits or withdrawals exceeding available funds).

### **2. Car Engine**

In a real car, the engine, fuel system, and electrical components are all hidden from the driver. The driver doesn't need to know the exact details of how the engine works. Instead, the driver interacts with the car through public methods like `start()`, `accelerate()`, or `brake()`.

#### **Encapsulation Concept in Car:**

- **Private Fields**: Internal variables like `engineStatus`, `fuelLevel`, etc., should be private.
- **Public Methods**: Methods like `start()`, `accelerate()`, and `brake()` are used to interact with the car.

```java
class Car {
    private boolean engineStatus;
    private double fuelLevel;

    // Getter for engine status
    public boolean isEngineRunning() {
        return engineStatus;
    }

    // Getter for fuel level
    public double getFuelLevel() {
        return fuelLevel;
    }

    // Method to start the car
    public void startEngine() {
        if (fuelLevel > 0) {
            engineStatus = true;
            System.out.println("Engine started.");
        } else {
            System.out.println("Insufficient fuel to start the engine.");
        }
    }

    // Method to accelerate
    public void accelerate() {
        if (engineStatus && fuelLevel > 0) {
            fuelLevel -= 0.5;  // Decreases fuel as the car accelerates
            System.out.println("Car is accelerating. Fuel level: " + fuelLevel);
        } else {
            System.out.println("Can't accelerate. Engine is off or fuel is empty.");
        }
    }

    // Method to stop the car
    public void stopEngine() {
        engineStatus = false;
        System.out.println("Engine stopped.");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();
        myCar.startEngine();
        myCar.accelerate();
        myCar.stopEngine();
    }
}
```

### **Explanation**:

- The internal working of the car (like how the engine starts or fuel consumption) is hidden.
- The driver interacts with the car using public methods like `startEngine()`, `accelerate()`, and `stopEngine()`, which ensures that the car operates correctly and prevents the driver from interacting with the internals directly.

### **3. ATM Machine**

An ATM (Automated Teller Machine) allows you to withdraw money, check your balance, or transfer funds. You don’t have direct access to the ATM’s internal systems or bank account details. You interact with the ATM via a **user interface** (PIN entry, transaction options), and the machine handles the rest internally.

#### **Encapsulation Concept in ATM:**

- **Private Fields**: The bank account balance and PIN are private.
- **Public Methods**: You interact with the ATM through public methods like `checkBalance()`, `withdraw()`, or `deposit()`.

```java
class ATM {
    private double balance;
    private String pin;

    public ATM(String pin) {
        this.pin = pin;
        this.balance = 1000;  // Initial balance
    }

    // Method to check balance
    public double checkBalance(String enteredPin) {
        if (enteredPin.equals(pin)) {
            return balance;
        } else {
            System.out.println("Incorrect PIN");
            return -1;
        }
    }

    // Method to withdraw money
    public void withdraw(String enteredPin, double amount) {
        if (enteredPin.equals(pin) && balance >= amount) {
            balance -= amount;
            System.out.println("Withdrawal successful. New balance: " + balance);
        } else {
            System.out.println("Invalid PIN or insufficient balance.");
        }
    }

    // Method to deposit money
    public void deposit(String enteredPin, double amount) {
        if (enteredPin.equals(pin) && amount > 0) {
            balance += amount;
            System.out.println("Deposit successful. New balance: " + balance);
        } else {
            System.out.println("Invalid PIN or invalid deposit amount.");
        }
    }
}

public class Main {
    public static void main(String[] args) {
        ATM myATM = new ATM("1234");

        // User enters PIN
        System.out.println("Balance: " + myATM.checkBalance("1234"));
        myATM.withdraw("1234", 500);
        myATM.deposit("1234", 200);
    }
}
```

### **Explanation**:

- The **ATM balance** and **PIN** are private and not directly accessible.
- Public methods like `checkBalance()`, `withdraw()`, and `deposit()` allow interaction with the ATM but control the flow and validation internally.

### **4. Online Shopping System**

In an online shopping system, a `Cart` object might have an internal list of items. The `Cart` class should not expose the items directly but should allow customers to add items, view the total, or checkout through public methods. The internal details of managing the list of items are hidden.

#### **Encapsulation Concept in Shopping Cart:**

- **Private Fields**: The list of items in the cart and the total amount are private.
- **Public Methods**: Methods like `addItem()`, `removeItem()`, and `getTotalAmount()` expose functionality to the outside.

```java
import java.util.ArrayList;
import java.util.List;

class ShoppingCart {
    private List<String> items;
    private double totalAmount;

    public ShoppingCart() {
        items = new ArrayList<>();
        totalAmount = 0.0;
    }

    // Method to add item to cart
    public void addItem(String item, double price) {
        items.add(item);
        totalAmount += price;
        System.out.println(item + " added to the cart. Total: " + totalAmount);
    }

    // Method to get the total amount
    public double getTotalAmount() {
        return totalAmount;
    }

    // Method to display all items
    public void displayItems() {
        System.out.println("Items in cart: " + items);
    }
}

public class Main {
    public static void main(String[] args) {
        ShoppingCart cart = new ShoppingCart();
        cart.addItem("Laptop", 1000.0);
        cart.addItem("Mouse", 20.0);
        cart.displayItems();
        System.out.println("Total amount: " + cart.getTotalAmount());
    }
}
```

### **Explanation**:

- The **items list** and **total amount** are private and cannot be directly accessed.
- Customers interact with the `ShoppingCart` class via public methods like `addItem()`, `getTotalAmount()`, and `displayItems()`. The implementation details of how items are stored and how the total is calculated are hidden.

### **Conclusion**

Encapsulation helps manage complexity by hiding the internal workings of a system and providing a clean interface for the user to interact with. Real-world systems, such as bank accounts, cars, ATM machines, and shopping carts, all implement encapsulation to keep sensitive data private and ensure controlled interaction through public methods. This allows developers to maintain and update the system’s internals without impacting the outside world.

---

---

## Q35: Abstraction in Java

### **Abstraction in Java**

Abstraction is one of the fundamental concepts in Object-Oriented Programming (OOP) that allows you to hide the complex implementation details and show only the essential features of an object. The idea behind abstraction is to represent only the relevant details to the user, leaving the unnecessary complexities hidden.

Abstraction can be achieved using **abstract classes** and **interfaces** in Java. It allows developers to create more modular and understandable code, making it easier to work with large applications.

### **Key Concepts of Abstraction:**

1. **Hiding Implementation Details**:
   Abstraction hides the internal workings (implementation details) and only exposes what is necessary. This helps to reduce complexity.

2. **Focus on What an Object Does, Not How It Does It**:
   Abstraction allows you to focus on _what_ an object represents and _what_ its behavior should be, without worrying about _how_ the behavior is implemented.

### **Types of Abstraction:**

1. **Abstraction through Abstract Classes**
2. **Abstraction through Interfaces**

### **Abstraction in Java:**

#### **1. Abstract Classes:**

An **abstract class** is a class that cannot be instantiated on its own and is meant to be subclassed by other classes. It can have both abstract methods (without implementation) and concrete methods (with implementation). Abstract classes are useful when you want to define a base class with some common functionality but leave the implementation of certain methods to the subclasses.

- **Abstract Method**: A method that is declared without an implementation. It must be implemented by any non-abstract subclass.

#### **Syntax**:

```java
abstract class Animal {
    abstract void sound(); // abstract method

    void sleep() {  // concrete method
        System.out.println("Animal is sleeping.");
    }
}

class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks.");
    }
}

class Main {
    public static void main(String[] args) {
        Animal animal = new Dog(); // You cannot instantiate Animal directly.
        animal.sound();  // Dog barks.
        animal.sleep();  // Animal is sleeping.
    }
}
```

#### **Explanation**:

- The `Animal` class is abstract, which means it cannot be instantiated directly.
- The `sound()` method is abstract, meaning the subclasses must implement it.
- The `sleep()` method is concrete, so it can be used by any subclass directly.
- The `Dog` class extends `Animal` and implements the abstract `sound()` method.

### **2. Interfaces:**

An **interface** in Java is a reference type, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types. Interfaces are used to define a contract that other classes must follow. A class that implements an interface must provide an implementation for all the methods declared in the interface.

#### **Syntax**:

```java
interface Animal {
    void sound();  // abstract method
}

class Dog implements Animal {
    public void sound() {
        System.out.println("Dog barks.");
    }
}

class Main {
    public static void main(String[] args) {
        Animal animal = new Dog();  // Interface reference pointing to Dog object
        animal.sound();  // Dog barks.
    }
}
```

#### **Explanation**:

- The `Animal` interface declares the `sound()` method.
- The `Dog` class implements the `Animal` interface, providing its own version of the `sound()` method.
- The `Main` class uses the interface `Animal` to refer to the `Dog` object, showing the abstraction of the object's actual type and behavior.

### **Advantages of Abstraction**:

1. **Hiding Complexity**:
   Abstraction hides unnecessary details, allowing you to focus on high-level concepts. For example, when you drive a car, you don’t need to understand how the engine works internally. You just need to know how to operate it.

2. **Modularity**:
   By breaking down a system into abstract components, you can work on different parts independently. For instance, defining abstract methods allows subclasses to implement their own versions.

3. **Flexibility**:
   You can change the implementation details without affecting the rest of the system, as long as the interface or abstract class remains the same. This makes it easier to maintain and update the code.

4. **Easier Maintenance**:
   When only essential details are exposed, the complexity is reduced. This also makes the system easier to modify without breaking existing code.

5. **Code Reusability**:
   With abstraction, you can define common methods in abstract classes or interfaces and reuse them across various concrete implementations, making your code more maintainable and reusable.

### **Real-World Example of Abstraction:**

#### **ATM System**

Consider an **ATM machine**. When you use an ATM, you don’t need to understand the internal working of the ATM such as how it communicates with the bank’s server or how it dispenses money. You interact with the ATM using a simple interface: inserting your card, entering your PIN, selecting a transaction, and receiving cash or a balance statement.

Here, the **ATM** system is abstracted, as the user only interacts with the system’s interface without knowing the complex underlying processes.

#### **Java Implementation of an ATM System:**

```java
// Abstract class
abstract class ATM {
    abstract void insertCard();
    abstract void enterPin();
    abstract void selectTransaction();
    abstract void dispenseCash();
}

// Concrete class implementing the abstract class
class RealATM extends ATM {
    void insertCard() {
        System.out.println("Card inserted.");
    }
    void enterPin() {
        System.out.println("PIN entered.");
    }
    void selectTransaction() {
        System.out.println("Transaction selected.");
    }
    void dispenseCash() {
        System.out.println("Cash dispensed.");
    }
}

class Main {
    public static void main(String[] args) {
        ATM atm = new RealATM();
        atm.insertCard();
        atm.enterPin();
        atm.selectTransaction();
        atm.dispenseCash();
    }
}
```

#### **Explanation**:

- The **ATM** class is abstract, hiding the specific details of ATM functionality.
- The `RealATM` class provides the actual implementation of each operation (e.g., inserting the card, entering the pin).
- The `Main` class uses the **ATM** interface to interact with the **RealATM** object, showing how abstraction hides the implementation details.

### **Summary of Abstraction in Java:**

- **Abstraction** allows you to focus on the essential features while hiding unnecessary implementation details.
- It can be achieved using **abstract classes** (providing partial implementation) or **interfaces** (defining a contract).
- **Abstract classes** are used when you want to provide common functionality to multiple classes, while **interfaces** are used to define behavior that can be implemented by any class, regardless of where it fits in the class hierarchy.
- The main goal of abstraction is to reduce complexity, improve code maintenance, and enhance reusability.

---

### **Who Is the "User" in Abstraction?**

In software, the "user" can mean two things:

1. **End-User**: The person interacting with the application (like using a mobile app or website).
2. **Developer/User of Your Code**: Other programmers who use the class or API you've created.

When we talk about abstraction in Java, **the "user" typically refers to the second type**—a programmer who uses your code.

### **What Does "Hiding Unnecessary Details" Mean?**

- It doesn’t mean literally hiding the code from visibility.
- It means providing a clean and simple interface (methods or functionalities) to interact with, while keeping the **implementation details and complexity** hidden inside the class.

In simpler terms:

- You only **expose what the user needs to know**.
- You **hide the internal working** so the user doesn't need to worry about it.

### **Why Do This?**

1. **Ease of Use**: The user (developer) doesn't need to understand the internal complexities.
2. **Flexibility**: You can change the internal implementation without breaking the code that uses it.
3. **Maintainability**: Simplifying what is exposed makes the system easier to maintain.

### **Normal Class vs. Abstract Class**

In a **normal class**, everything can be concrete and fully implemented.

- If the user sees all the details (every method and how they work), they might need to understand all of it to use the class effectively.
- This can make the class harder to use if it's complex.

In an **abstract class**, you can:

- Define only the **relevant methods** the user needs to know (abstract methods).
- Let subclasses handle the internal complexities by providing concrete implementations.

### **Example: Bank System**

Imagine you’re creating a **Banking System API** where developers use your classes to interact with bank accounts.

Without abstraction:

```java
class BankAccount {
    void transferMoney(String accountFrom, String accountTo, double amount) {
        // Steps to transfer money
        connectToBankServer();
        authenticateAccount(accountFrom);
        deductAmount(accountFrom, amount);
        creditAmount(accountTo, amount);
    }

    void connectToBankServer() {
        // Complex implementation
    }

    void authenticateAccount(String account) {
        // Complex implementation
    }

    void deductAmount(String account, double amount) {
        // Complex implementation
    }

    void creditAmount(String account, double amount) {
        // Complex implementation
    }
}
```

Here, the developer using your class needs to know **all these methods** and the sequence to use them correctly.

With abstraction:

```java
abstract class BankAccount {
    abstract void transferMoney(String accountFrom, String accountTo, double amount);

    // Internal methods are not exposed to the user
    protected void connectToBankServer() {
        // Complex implementation
    }

    protected void authenticateAccount(String account) {
        // Complex implementation
    }

    protected void deductAmount(String account, double amount) {
        // Complex implementation
    }

    protected void creditAmount(String account, double amount) {
        // Complex implementation
    }
}

class MyBankAccount extends BankAccount {
    @Override
    void transferMoney(String accountFrom, String accountTo, double amount) {
        connectToBankServer();
        authenticateAccount(accountFrom);
        deductAmount(accountFrom, amount);
        creditAmount(accountTo, amount);
        System.out.println("Transfer successful");
    }
}
```

Now, the user only needs to call **`transferMoney()`**. They don’t need to worry about how the server is connected, how authentication works, or how money is debited or credited. This complexity is hidden inside the class.

### **What Abstraction Really Does**

- **Normal Class**: Everything is visible, which can overwhelm the user of your code.
- **Abstract Class**: Exposes only what’s necessary and hides unnecessary details, simplifying usage and focusing on the "what" instead of the "how."

### **Key Takeaway**

Abstraction is not about hiding code from **physical visibility** but about separating **what the user needs to know** (interface) from **how it works internally** (implementation). This makes your code cleaner, easier to use, and more maintainable.

---

An **abstract class** in Java is a class that **cannot be instantiated** because it is meant to serve as a blueprint for other classes. It is not complete by itself; instead, it is designed to be extended by subclasses that provide the implementation of its abstract methods.

### 1. **Incomplete Implementation**

- An abstract class can have one or more **abstract methods** (methods without a body). These methods **must be implemented by subclasses**.
- Since the abstract class does not provide complete functionality, creating an object of it would result in an incomplete object, which makes no sense.

**Example:**

```java
abstract class Shape {
    abstract void draw(); // No implementation here
}

class Circle extends Shape {
    void draw() {
        System.out.println("Drawing a circle");
    }
}

// Shape s = new Shape(); // Error: Cannot instantiate the abstract class
Shape s = new Circle(); // Works because Circle provides the implementation
```

**Why can’t `Shape` be instantiated?**

- Because it doesn’t define how to `draw()`, and attempting to use `Shape` directly would lead to missing behavior.

### 2. **Encouraging Reusability**

- Abstract classes are intended to define **common behavior** and allow specific subclasses to provide their own versions of the missing functionality.
- This enforces the design principle of **code reuse** while maintaining flexibility.

**Example:**

```java
abstract class Animal {
    abstract void sound();

    void sleep() {
        System.out.println("Sleeping...");
    }
}

class Dog extends Animal {
    void sound() {
        System.out.println("Bark");
    }
}

class Cat extends Animal {
    void sound() {
        System.out.println("Meow");
    }
}

public class Main {
    public static void main(String[] args) {
        // Animal a = new Animal(); // Error: Cannot instantiate
        Animal dog = new Dog();
        dog.sound(); // Output: Bark
        dog.sleep(); // Output: Sleeping...
    }
}
```

Here, `Animal` defines the **common behavior** (`sleep()`), while `Dog` and `Cat` define the **specific behavior** (`sound()`).

### 3. **Enforcing Polymorphism**

- Abstract classes are often used to implement **polymorphism**, allowing a common reference type (the abstract class) to point to objects of different subclasses.
- If abstract classes were instantiable, this polymorphism would lose its purpose because the abstract class wouldn’t represent a meaningful entity on its own.

**Example:**

```java
abstract class Vehicle {
    abstract void start();
}

class Car extends Vehicle {
    void start() {
        System.out.println("Car is starting");
    }
}

class Bike extends Vehicle {
    void start() {
        System.out.println("Bike is starting");
    }
}

public class Main {
    public static void main(String[] args) {
        Vehicle v1 = new Car();
        Vehicle v2 = new Bike();
        v1.start(); // Output: Car is starting
        v2.start(); // Output: Bike is starting
    }
}
```

### 4. **Logical Design**

- Abstract classes represent **concepts** rather than concrete objects.
- For example:
  - A `Shape` class represents the idea of a shape (circle, rectangle, etc.), but it is meaningless to create a generic "shape" object without specifying what type of shape it is.

**Example:**

```java
abstract class Shape {
    abstract void draw();
}

class Circle extends Shape {
    void draw() {
        System.out.println("Drawing a Circle");
    }
}

class Rectangle extends Shape {
    void draw() {
        System.out.println("Drawing a Rectangle");
    }
}

// Shape s = new Shape(); // Doesn't make sense because Shape is not specific
Shape s = new Circle(); // Makes sense
```

### 5. **Prevent Misuse**

- By marking a class as abstract, Java enforces that it can only be **used through inheritance**. This ensures that the intended design of the class is followed.

### **Why Abstract Classes Cannot Be Instantiated:**

1. **They are incomplete**: They may have abstract methods with no implementation.
2. **They represent concepts**, not actual objects.
3. **They enforce inheritance**, allowing subclasses to provide specific implementations.
4. **Polymorphism**: Abstract classes allow dynamic behavior based on the subclass type, not the abstract class itself.

### Key Takeaway:

An abstract class cannot be instantiated because it serves as a **template** for subclasses, not as a fully functional class. Its purpose is to define a structure or a contract that subclasses must follow, while delegating the responsibility of implementing certain details to the subclasses.

---

---

## Q36: Real-World Examples of Abstraction

### **Real-World Examples of Abstraction**

Here are some relatable and easy-to-understand real-world examples of **Abstraction**:

### **1. TV Remote Control**

A **TV remote** is an excellent example of abstraction in real life. When you use a remote to control the TV, you don't need to know how the internal components of the TV or remote work. You simply press buttons to **change the channel**, **adjust the volume**, or **turn the TV on/off**.

#### **Abstraction Concept:**

- **Internal Implementation**: The workings of the remote's circuits and the internal functions of the TV (like signal processing and display technology) are hidden from the user.
- **Public Interface**: The user interacts with a simple interface (the remote buttons), and the remote communicates with the TV without revealing the complexities of how signals are sent and interpreted.

```java
class TV {
    public void turnOn() {
        System.out.println("The TV is now ON.");
    }

    public void turnOff() {
        System.out.println("The TV is now OFF.");
    }

    public void changeChannel(int channelNumber) {
        System.out.println("Changing to channel " + channelNumber);
    }

    public void adjustVolume(int volumeLevel) {
        System.out.println("Volume is now set to " + volumeLevel);
    }
}

class RemoteControl {
    private TV tv;

    public RemoteControl(TV tv) {
        this.tv = tv;
    }

    public void pressOnButton() {
        tv.turnOn();
    }

    public void pressOffButton() {
        tv.turnOff();
    }

    public void pressChannelButton(int channelNumber) {
        tv.changeChannel(channelNumber);
    }

    public void pressVolumeButton(int volumeLevel) {
        tv.adjustVolume(volumeLevel);
    }
}

public class Main {
    public static void main(String[] args) {
        TV myTV = new TV();
        RemoteControl remote = new RemoteControl(myTV);

        remote.pressOnButton();
        remote.pressChannelButton(5);
        remote.pressVolumeButton(15);
        remote.pressOffButton();
    }
}
```

### **Explanation**:

- You interact with the **TV** through the **RemoteControl** interface, hiding the complexity of how the TV and remote actually work internally.
- The actual operations (like turning the TV on or adjusting the volume) are abstracted away from the user, who only needs to know what button to press.

### **2. Car Dashboard**

When you drive a car, you don't need to understand how the engine works, how fuel is converted into motion, or how the exhaust system functions. You only need to interact with the dashboard through basic controls (accelerator, brake, gear lever, etc.), which provide the necessary abstraction.

#### **Abstraction Concept:**

- **Internal Implementation**: The car's engine, fuel system, transmission, and electronics are abstracted away from the driver.
- **Public Interface**: The driver interacts with simple controls, such as the steering wheel, pedals, and gear shift, to operate the car.

```java
class Car {
    public void startEngine() {
        System.out.println("The engine is started.");
    }

    public void drive() {
        System.out.println("The car is now driving.");
    }

    public void stop() {
        System.out.println("The car is stopped.");
    }

    public void turnOffEngine() {
        System.out.println("The engine is turned off.");
    }
}

class Driver {
    private Car car;

    public Driver(Car car) {
        this.car = car;
    }

    public void driveCar() {
        car.startEngine();
        car.drive();
        car.stop();
        car.turnOffEngine();
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();
        Driver driver = new Driver(myCar);

        driver.driveCar();
    }
}
```

### **Explanation**:

- The **Car** class abstracts away complex components such as the engine, transmission, and fuel system.
- The **Driver** interacts with a simple interface of **startEngine()**, **drive()**, **stop()**, and **turnOffEngine()**, which hide the inner workings of the car.

### **3. Online Payment System**

Consider an **online payment system** (e.g., PayPal, Credit/Debit Card Payment). When you make a payment online, you don’t need to know how the payment gateway processes transactions, connects to the bank, or validates your credentials. You simply enter your payment details and confirm the transaction.

#### **Abstraction Concept:**

- **Internal Implementation**: The entire payment processing system (communication with banks, security protocols, transaction handling) is abstracted from the user.
- **Public Interface**: The user only interacts with simple forms and buttons to make payments.

```java
interface PaymentGateway {
    void initiatePayment(double amount);
}

class PayPalPayment implements PaymentGateway {
    @Override
    public void initiatePayment(double amount) {
        System.out.println("Payment of $" + amount + " made via PayPal.");
    }
}

class CreditCardPayment implements PaymentGateway {
    @Override
    public void initiatePayment(double amount) {
        System.out.println("Payment of $" + amount + " made via Credit Card.");
    }
}

class OnlineShoppingCart {
    private PaymentGateway paymentGateway;

    public OnlineShoppingCart(PaymentGateway paymentGateway) {
        this.paymentGateway = paymentGateway;
    }

    public void checkout(double amount) {
        paymentGateway.initiatePayment(amount);
    }
}

public class Main {
    public static void main(String[] args) {
        PaymentGateway paypal = new PayPalPayment();
        OnlineShoppingCart cart1 = new OnlineShoppingCart(paypal);
        cart1.checkout(50.0);

        PaymentGateway creditCard = new CreditCardPayment();
        OnlineShoppingCart cart2 = new OnlineShoppingCart(creditCard);
        cart2.checkout(100.0);
    }
}
```

### **Explanation**:

- The **PaymentGateway** interface provides an abstraction for initiating payments without revealing the complex details of payment methods.
- Different payment methods like **PayPal** and **CreditCardPayment** implement this abstraction, but users don't need to understand how each method works internally. They only need to use the `checkout()` method.

### **4. Coffee Machine**

A **coffee machine** is a good example of abstraction. When you use a coffee machine, you don’t need to know the details of how it brews coffee. You just need to select a type of coffee, press a button, and the machine takes care of the rest.

#### **Abstraction Concept:**

- **Internal Implementation**: The brewing process, water heating, and coffee grinding are hidden from the user.
- **Public Interface**: The user only needs to choose the type of coffee and press a button.

```java
abstract class CoffeeMachine {
    public abstract void brewCoffee();

    public void serveCoffee() {
        System.out.println("Coffee is ready to be served!");
    }
}

class EspressoMachine extends CoffeeMachine {
    @Override
    public void brewCoffee() {
        System.out.println("Brewing Espresso...");
    }
}

class CappuccinoMachine extends CoffeeMachine {
    @Override
    public void brewCoffee() {
        System.out.println("Brewing Cappuccino...");
    }
}

public class Main {
    public static void main(String[] args) {
        CoffeeMachine espresso = new EspressoMachine();
        espresso.brewCoffee();
        espresso.serveCoffee();

        CoffeeMachine cappuccino = new CappuccinoMachine();
        cappuccino.brewCoffee();
        cappuccino.serveCoffee();
    }
}
```

### **Explanation**:

- The **CoffeeMachine** class abstracts the brewing process.
- The **EspressoMachine** and **CappuccinoMachine** classes provide specific implementations of the `brewCoffee()` method.
- The user interacts with a simple interface of `brewCoffee()` and `serveCoffee()`, without worrying about the internal workings.

### **5. Mobile Phone**

When you use a **mobile phone**, you don’t need to understand the internal operations like the CPU, RAM, storage management, or communication protocols. You simply use the phone’s interface (touch screen, buttons) to make calls, send messages, and use apps.

#### **Abstraction Concept:**

- **Internal Implementation**: The internal workings of the phone (hardware, operating system, and software) are abstracted.
- **Public Interface**: The user interacts with a simple touchscreen interface to perform tasks.

```java
class MobilePhone {
    public void makeCall(String phoneNumber) {
        System.out.println("Calling " + phoneNumber);
    }

    public void sendMessage(String message, String phoneNumber) {
        System.out.println("Sending message: " + message + " to " + phoneNumber);
    }

    public void openApp(String appName) {
        System.out.println("Opening " + appName + " app.");
    }
}

public class Main {
    public static void main(String[] args) {
        MobilePhone myPhone = new MobilePhone();
        myPhone.makeCall("123-456-7890");
        myPhone.sendMessage("Hello!", "123-456-7890");
        myPhone.openApp("Facebook");
    }
}
```

### **Explanation**:

- The **MobilePhone** class abstracts away the complex underlying components of the phone.
- The user interacts with the phone through simple methods such as `makeCall()`, `sendMessage()`, and `openApp()`, without understanding the hardware or OS layers.

### **Conclusion**

Abstraction helps simplify interactions with complex systems by providing a clean and simplified interface while hiding the internal complexities. In all these examples (TV remote, car, online payment system, coffee machine, and mobile phone), the user interacts with simple methods that abstract the underlying processes, making them easier to use and understand.

---

---

## Q37: Difference Between Encapsulation and Abstraction

Both **Encapsulation** and **Abstraction** are fundamental concepts in Object-Oriented Programming (OOP), but they serve different purposes and address different aspects of a program's design. Here's a detailed comparison:

### **1. Definition:**

- **Encapsulation**:

  - Encapsulation is the concept of **bundling** the data (variables) and the methods (functions) that operate on the data into a single unit, or class.
  - It is also about **restricting direct access** to some of the object's components, which can prevent the accidental modification of data. This is done using **access modifiers** such as `private`, `protected`, and `public`.

- **Abstraction**:
  - Abstraction is the concept of **hiding the complex implementation details** of a system and exposing only the necessary and relevant parts of it.
  - It focuses on **what** an object does, not **how** it does it.
  - Abstraction is achieved through **abstract classes** or **interfaces** in Java, allowing the implementation to be hidden from the user.

### **2. Focus:**

- **Encapsulation**:

  - Focuses on **data protection** and **modularizing** the code.
  - It’s about controlling access to the internal state of the object and ensuring that the object's data cannot be altered in unintended ways.

- **Abstraction**:
  - Focuses on **hiding unnecessary details** from the user.
  - It’s about showing only the essential features and providing a simple interface for interaction.

### **3. Access Control:**

- **Encapsulation**:

  - It uses **access modifiers** to protect the data and restrict the way the data is accessed or modified.
  - Commonly involves **getter** and **setter** methods to control access to private variables.

- **Abstraction**:
  - It hides the **implementation details** of methods or classes, exposing only what is necessary.
  - This can be achieved by using **abstract classes** or **interfaces**.

### **4. Implementation:**

- **Encapsulation**:

  - Implemented using **classes**, **access modifiers** (`private`, `protected`, `public`), and **getter/setter** methods.
  - Example: Hiding sensitive data (e.g., bank account balance) and providing methods to retrieve or modify it.

- **Abstraction**:
  - Implemented using **abstract classes**, **interfaces**, and **abstract methods**.
  - Example: A **Shape** class with abstract methods like `draw()` but no details of how the drawing is done. Concrete classes like **Circle** or **Rectangle** will implement how the drawing is done.

### **5. Purpose:**

- **Encapsulation**:

  - Protects the internal state of an object from unauthorized access and modification.
  - Ensures that an object’s data is consistent and valid through controlled access.

- **Abstraction**:
  - Hides the complex logic from the user and provides a simple interface for using an object.
  - Focuses on **reducing complexity** by only showing relevant features.

### **6. Example in Code:**

#### **Encapsulation Example**:

```java
class Account {
    private double balance;  // Private field

    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        }
    }

    public double getBalance() {
        return balance;
    }
}
```

- The **balance** is hidden using the `private` access modifier.
- Access to **balance** is controlled through **public methods** (`deposit()` and `getBalance()`), ensuring that the balance can only be changed in a controlled way.

#### **Abstraction Example**:

```java
abstract class Shape {
    public abstract void draw();  // Abstract method
}

class Circle extends Shape {
    @Override
    public void draw() {
        System.out.println("Drawing Circle");
    }
}

class Square extends Shape {
    @Override
    public void draw() {
        System.out.println("Drawing Square");
    }
}
```

- The **Shape** class is abstract and provides an abstract method `draw()` without specifying how it is done.
- **Circle** and **Square** provide the specific implementations of the `draw()` method.

### **7. Real-World Analogy:**

- **Encapsulation**:

  - Think of a **pill bottle**. The **pills (data)** are inside the bottle, and you have to use a **lid (method)** to access or modify the pills. You can only interact with the pills through the lid, which ensures they are not misused.

- **Abstraction**:
  - Think of a **TV remote**. You interact with the **buttons (interface)** to control the TV, but you don’t need to know how the TV internally works (e.g., signal processing, power control). You just know what the remote does when you press buttons.

### **8. Example in Real Life:**

- **Encapsulation**:

  - A **bank account** has private data such as the balance and account number. Only the methods provided by the bank (like `deposit()`, `withdraw()`, etc.) can manipulate these details. Direct access to the account's balance is restricted.

- **Abstraction**:
  - A **car** has complex systems under the hood (engine, transmission, electronics). As a driver, you don’t need to know how these systems work. You simply interact with the **steering wheel, pedals, and gearshift**, which provide a simple interface for driving the car.

### **9. Key Differences:**

| Aspect             | Encapsulation                                                        | Abstraction                                                         |
| ------------------ | -------------------------------------------------------------------- | ------------------------------------------------------------------- |
| **Purpose**        | Protects the data by restricting access.                             | Hides the implementation details.                                   |
| **Visibility**     | Controls access to the internal data of an object.                   | Hides unnecessary implementation details.                           |
| **Implementation** | Achieved through **classes**, **methods**, and **access modifiers**. | Achieved through **abstract classes** or **interfaces**.            |
| **Focus**          | **Data security** and **access control**.                            | **Simplified interaction** and **reduced complexity**.              |
| **Example**        | A class with **private** fields and **getter/setter** methods.       | A class with abstract methods, hiding the logic of implementations. |

### **Conclusion:**

- **Encapsulation** is about **data protection** and restricting access to the internal state, ensuring that data is manipulated safely.
- **Abstraction** is about **hiding complexity** by providing a simplified interface, focusing on **what** an object does rather than **how** it does it.

---

---

## Q38: Data Hiding in Object-Oriented Programming (OOP)

**Data Hiding** is one of the key principles of Object-Oriented Programming (OOP) that emphasizes restricting access to the internal data of an object to protect it from unauthorized access and modification. It allows the class to control how the data is accessed or changed. Data Hiding is closely related to **Encapsulation**, but the focus is specifically on controlling how data is exposed and accessed.

### **Key Points:**

1. **What is Data Hiding?**

   - Data Hiding is the practice of **restricting direct access** to an object's internal data and making it accessible only through well-defined methods (getter and setter methods).
   - It helps to protect the object’s integrity by preventing unwanted or harmful modifications and ensures that any change in the object’s data is done in a controlled and validated manner.
   - Data Hiding is achieved by making the fields (variables) of a class **private** or **protected** and providing **public getter and setter** methods to access or modify them.

2. **Why is Data Hiding Important?**

   - **Security**: By restricting direct access to data, it ensures that only authorized methods can manipulate the object's state. This prevents accidental or malicious changes.
   - **Control**: Data Hiding allows the class to enforce **validity checks** when the data is accessed or modified, maintaining the consistency and validity of the object’s state.
   - **Flexibility and Maintenance**: The implementation of the class can change without affecting the external code that uses it. For example, the way a value is calculated can be hidden, allowing for changes in logic without impacting users of the class.
   - **Reduced Complexity**: By hiding implementation details, it simplifies how the object interacts with other parts of the program. Users of the object don’t need to understand its internal workings to use it effectively.

3. **How is Data Hiding Implemented?**

   - Data Hiding is implemented using **access modifiers** in Java like:
     - **Private**: Makes fields and methods inaccessible from outside the class.
     - **Protected**: Restricts access to the class, its subclasses, and classes in the same package.
     - **Public**: Allows unrestricted access from anywhere.
   - Typically, **private** is used for data members (variables), and **public** methods (getters and setters) are used to access and modify them.

4. **How Data Hiding Works in Java?**
   - **Private Fields**: Variables are declared **private** so they cannot be directly accessed from outside the class.
   - **Public Methods**: Getter and setter methods are provided as **public** methods to get or set the values of private fields. The setter method can also include validation logic to ensure that only valid data is set.

### **Example of Data Hiding in Java:**

```java
class Person {
    // Private data members (Data Hiding)
    private String name;
    private int age;

    // Public getter method to access the name
    public String getName() {
        return name;
    }

    // Public setter method to modify the name with validation
    public void setName(String name) {
        if(name != null && !name.isEmpty()) {
            this.name = name;
        } else {
            System.out.println("Invalid name");
        }
    }

    // Public getter method to access the age
    public int getAge() {
        return age;
    }

    // Public setter method to modify the age with validation
    public void setAge(int age) {
        if(age >= 0 && age <= 150) {
            this.age = age;
        } else {
            System.out.println("Invalid age");
        }
    }
}

public class TestDataHiding {
    public static void main(String[] args) {
        Person person = new Person();

        // Accessing and modifying data via getter and setter methods
        person.setName("John");
        person.setAge(25);

        System.out.println("Name: " + person.getName());
        System.out.println("Age: " + person.getAge());

        // Attempt to access or modify private fields directly (This will give an error)
        // person.name = "Mike"; // Error: name has private access in Person
        // person.age = 200; // Error: age has private access in Person
    }
}
```

### **Explanation of Example:**

- **Private Fields**: The fields `name` and `age` are marked as **private**, meaning they cannot be accessed directly from outside the class.
- **Public Getter and Setter**: The `getName()`, `setName()`, `getAge()`, and `setAge()` methods are provided to allow access and modification of the private fields. In the setter methods, additional validation is added to ensure that only valid values are set for the `name` and `age`.

### **Key Points from Example:**

- **Name and Age** are hidden from direct access.
- The only way to modify or access these fields is through the **setter** and **getter** methods, which enforce validation.
- **Flexibility**: If we want to change the internal implementation of how `name` and `age` are stored, we can do so without affecting the users of the `Person` class.
- The **data is protected**, ensuring that only valid data gets through to the object's state.

### **Benefits of Data Hiding:**

1. **Improved Security**: Only authorized methods (like setter methods) can modify the object’s state. This reduces the chance of errors or malicious modifications.
2. **Encapsulation**: Data Hiding is a key aspect of **Encapsulation**, allowing the internal workings of an object to be protected while still providing controlled access to its data.
3. **Consistency**: By using setter methods to modify fields, we can ensure that changes to the object’s data follow specific rules (like range checks or formatting), ensuring consistency.
4. **Flexibility**: You can change the internal implementation of a class without affecting the external code that uses the class, as long as the public interface remains the same.
5. **Easy Maintenance**: Since data hiding controls how data is accessed or modified, the implementation can change without disturbing the classes or methods that depend on it.

### **Real-World Analogy:**

Imagine a **security safe**. The **combination lock** (setter method) is the only way to access or modify the contents of the safe (object’s data). You cannot just open the safe (access the data) directly. You must use the **lock (setter method)** to control who can access or modify the contents. This ensures that only authorized people can get to the valuable contents (protected data).

### **When to Use Data Hiding?**

1. **When you need to protect sensitive data**: For example, credit card information, passwords, etc., should not be directly accessible.
2. **When data should only be modified in a controlled way**: If an object’s data needs to be validated or processed before changing it (e.g., applying rules for a salary).
3. **When you want to reduce complexity**: Hiding unnecessary implementation details helps users of the class focus on what the object does, rather than how it does it.

### **Conclusion:**

Data Hiding is a vital concept in OOP that promotes security, integrity, and maintainability of the code. It restricts direct access to the object's data and ensures controlled, validated access through getter and setter methods. This principle enhances the design of an object by protecting its internal state and preventing unwanted or harmful changes.

---

---

## Q39: Access Modifiers in Java: A Deep Dive

Access modifiers in Java determine the visibility or accessibility of classes, methods, variables, and constructors. They control which parts of a program can interact with a particular member. Java provides four levels of access control:

1. **Public**
2. **Protected**
3. **Default (Package-Private)**
4. **Private**

Let's explore each modifier in depth.

### 1. **`public` Access Modifier**

- **Visibility**: Accessible from **anywhere** in the program, across all classes, packages, and modules.
- **Use Case**: Used when a member or class needs to be accessed globally.
- **Applicable To**: Classes, methods, fields, and constructors.
- **Examples**:

  ```java
  public class PublicClass {
      public String name = "Java";

      public void displayName() {
          System.out.println(name);
      }
  }

  class Main {
      public static void main(String[] args) {
          PublicClass obj = new PublicClass();
          obj.displayName(); // Accessible anywhere
      }
  }
  ```

### 2. **`protected` Access Modifier**

- **Visibility**: Accessible:
  - Within the **same package**.
  - By **subclasses** in other packages through **inheritance**.
- **Use Case**: Useful when you want to expose members to subclasses while restricting direct access from non-subclassed external code.
- **Applicable To**: Methods, fields, and constructors (not top-level classes).
- **Examples**:

  ```java
  package package1;

  public class Parent {
      protected String message = "Hello from Parent";

      protected void displayMessage() {
          System.out.println(message);
      }
  }

  package package2;

  import package1.Parent;

  public class Child extends Parent {
      public static void main(String[] args) {
          Child obj = new Child();
          obj.displayMessage(); // Accessible due to inheritance
      }
  }
  ```

### 3. **Default (Package-Private) Access Modifier**

- **Visibility**: Accessible only within the **same package**. This is the default modifier if no access modifier is specified.
- **Use Case**: Useful for members that should not be accessible outside the package, encouraging encapsulation within the same module.
- **Applicable To**: Classes, methods, fields, and constructors.
- **Examples**:

  ```java
  package package1;

  class DefaultClass {
      String message = "Default Access";

      void displayMessage() {
          System.out.println(message);
      }
  }

  class Main {
      public static void main(String[] args) {
          DefaultClass obj = new DefaultClass();
          obj.displayMessage(); // Accessible within the same package
      }
  }
  ```

### 4. **`private` Access Modifier**

- **Visibility**: Accessible only within the **same class**.
- **Use Case**: Used to enforce strict encapsulation and prevent external access.
- **Applicable To**: Methods, fields, and constructors (not top-level classes).
- **Examples**:

  ```java
  public class PrivateExample {
      private String message = "Private Access";

      private void displayMessage() {
          System.out.println(message);
      }

      public void accessPrivateMethod() {
          displayMessage(); // Accessible within the same class
      }

      public static void main(String[] args) {
          PrivateExample obj = new PrivateExample();
          obj.accessPrivateMethod(); // Indirect access to private method
      }
  }
  ```

### **Detailed Access Levels in Java**

| **Access Modifier**           | **Same Class** | **Same Package** | **Subclasses (Same/Different Package)** | **Anywhere** | **Short Tips**                                                                                    |
| ----------------------------- | -------------- | ---------------- | --------------------------------------- | ------------ | ------------------------------------------------------------------------------------------------- |
| **`public`**                  | ✅             | ✅               | ✅                                      | ✅           | Fully open access. Use for APIs or methods/classes meant to be accessible globally.               |
| **`protected`**               | ✅             | ✅               | ✅ (via inheritance, not objects)       | ❌           | Visible to subclasses and same package. Best for inheritance with limited external exposure.      |
| **Default (Package-Private)** | ✅             | ✅               | ❌                                      | ❌           | Accessible only within the same package. Good for internal logic and package-level encapsulation. |
| **`private`**                 | ✅             | ❌               | ❌                                      | ❌           | Strictly within the class. Ideal for securing sensitive data or implementation details.           |

### Additional Concepts

#### 1. **Access Modifiers for Top-Level Classes**

- A top-level class can only be `public` or default (package-private).
- `private` and `protected` are not allowed for top-level classes.

#### 2. **Encapsulation and Access Modifiers**

Access modifiers play a crucial role in encapsulation by restricting access to class members. By combining `private` with `public` or `protected` methods (getters/setters), you can control how data is accessed or modified.

#### 3. **Inheritance and `protected`**

The `protected` modifier allows a subclass to access its parent class's members even if they belong to a different package. However, a `protected` member is not accessible through an object instance unless it's in the same package.

#### 4. **Constructor Access Modifiers**

- **`public`**: Allows the class to be instantiated anywhere.
- **`protected`**: Restricts instantiation to the same package or subclasses.
- **`private`**: Restricts instantiation to the same class, often used in singleton patterns.

### Common Interview Questions

1. **Why can’t we use `private` or `protected` for top-level classes?**

   - Top-level classes must either be accessible everywhere (`public`) or restricted to their own package (default). Java's design prevents finer-grained restrictions for classes at the top level.

2. **What happens if we define a `protected` constructor?**

   - A `protected` constructor restricts object creation to the same package or subclasses.

3. **Can a private method be overridden?**
   - No, private methods are not visible to subclasses, so they cannot be overridden.

### **Access Modifiers Quick Tips**

| **Modifier**    | **Visibility Scope**                             | **Key Use Case**                                                                |
| --------------- | ------------------------------------------------ | ------------------------------------------------------------------------------- |
| **`public`**    | Accessible **everywhere**                        | Use for APIs, utility classes, and global methods/variables.                    |
| **`protected`** | Accessible within **package** and **subclasses** | Use when subclassing requires access but restrict access for unrelated classes. |
| **Default**     | Accessible within **package only**               | Use for internal package logic; restrict access outside the package.            |
| **`private`**   | Accessible **within the same class**             | Use to encapsulate sensitive data or helper methods within the class.           |

### **Key Notes**

- **`public`**: No restrictions; global access.
- **`protected`**: Visible to subclasses (even in other packages) but **only via inheritance**.
- **Default**: Accessible only within the same package (no keyword required).
- **`private`**: Strictly within the class; ensures encapsulation.

### **Quick Example**

- **Public**: Open to all.
- **Protected**: Family-only (subclasses).
- **Default**: Neighborhood-only (same package).
- **Private**: Me-only (same class).

---

---

## Q40: Commonly used built-in methods in Java

comprehensive list of commonly used built-in methods in Java, organized by data types or categories

### **String Methods**

| **Method**              | **Description**                                | **Example**                              |
| ----------------------- | ---------------------------------------------- | ---------------------------------------- |
| `length()`              | Returns the length of the string.              | `"Java".length()` → `4`                  |
| `charAt(index)`         | Returns the character at the specified index.  | `"Java".charAt(1)` → `'a'`               |
| `substring(start, end)` | Extracts a substring.                          | `"Java".substring(1, 3)` → `"av"`        |
| `contains(sequence)`    | Checks if the string contains the sequence.    | `"Java".contains("av")` → `true`         |
| `equals(object)`        | Compares two strings for equality.             | `"Java".equals("java")` → `false`        |
| `toUpperCase()`         | Converts all characters to uppercase.          | `"Java".toUpperCase()` → `"JAVA"`        |
| `toLowerCase()`         | Converts all characters to lowercase.          | `"Java".toLowerCase()` → `"java"`        |
| `replace(old, new)`     | Replaces occurrences of a substring.           | `"Java".replace('a', 'o')` → `"Jovo"`    |
| `split(delimiter)`      | Splits the string into an array of substrings. | `"A,B,C".split(",")` → `["A", "B", "C"]` |
| `trim()`                | Removes leading and trailing spaces.           | `" Java ".trim()` → `"Java"`             |

### **Math Methods**

| **Method**            | **Description**                                | **Example**                         |
| --------------------- | ---------------------------------------------- | ----------------------------------- |
| `abs(number)`         | Returns the absolute value.                    | `Math.abs(-10)` → `10`              |
| `sqrt(number)`        | Returns the square root.                       | `Math.sqrt(16)` → `4.0`             |
| `pow(base, exponent)` | Returns the value of base raised to the power. | `Math.pow(2, 3)` → `8.0`            |
| `max(a, b)`           | Returns the larger of two numbers.             | `Math.max(5, 10)` → `10`            |
| `min(a, b)`           | Returns the smaller of two numbers.            | `Math.min(5, 10)` → `5`             |
| `random()`            | Returns a random number between 0.0 and 1.0.   | `Math.random()` → `0.123` (example) |
| `ceil(number)`        | Rounds up to the nearest whole number.         | `Math.ceil(4.2)` → `5.0`            |
| `floor(number)`       | Rounds down to the nearest whole number.       | `Math.floor(4.8)` → `4.0`           |
| `round(number)`       | Rounds to the nearest whole number.            | `Math.round(4.5)` → `5`             |

### **Array Methods**

| **Method**                        | **Description**                             | **Example**                                   |
| --------------------------------- | ------------------------------------------- | --------------------------------------------- |
| `Arrays.toString(array)`          | Converts the array to a string.             | `Arrays.toString(new int[]{1, 2})` → `[1, 2]` |
| `Arrays.sort(array)`              | Sorts the array in ascending order.         | `Arrays.sort(arr)`                            |
| `Arrays.equals(arr1, arr2)`       | Checks if two arrays are equal.             | `Arrays.equals(arr1, arr2)` → `true/false`    |
| `Arrays.copyOf(array, len)`       | Copies elements into a new array.           | `Arrays.copyOf(arr, 3)`                       |
| `Arrays.binarySearch(array, key)` | Searches for a value and returns the index. | `Arrays.binarySearch(arr, 10)` → `2`          |

### **List Methods**

| **Method**          | **Description**                                    | **Example**                      |
| ------------------- | -------------------------------------------------- | -------------------------------- |
| `add(element)`      | Adds an element to the list.                       | `list.add("Java")`               |
| `remove(index)`     | Removes the element at the specified index.        | `list.remove(2)`                 |
| `get(index)`        | Retrieves the element at the specified index.      | `list.get(0)` → `"Java"`         |
| `size()`            | Returns the number of elements in the list.        | `list.size()` → `5`              |
| `clear()`           | Removes all elements from the list.                | `list.clear()`                   |
| `contains(element)` | Checks if the list contains the specified element. | `list.contains("Java")` → `true` |

### **Wrapper Class Methods**

| **Method**            | **Description**                        | **Example**                             |
| --------------------- | -------------------------------------- | --------------------------------------- |
| `parseInt(string)`    | Converts a string to an integer.       | `Integer.parseInt("10")` → `10`         |
| `parseDouble(string)` | Converts a string to a double.         | `Double.parseDouble("3.14")` → `3.14`   |
| `valueOf(string)`     | Converts a string to a wrapper object. | `Integer.valueOf("10")` → `Integer(10)` |
| `toString(value)`     | Converts a number to a string.         | `Integer.toString(10)` → `"10"`         |

### **Date and Time Methods (`java.time`)**

| **Method**            | **Description**                 | **Example**                                              |
| --------------------- | ------------------------------- | -------------------------------------------------------- |
| `LocalDate.now()`     | Gets the current date.          | `LocalDate.now()` → `2024-12-31`                         |
| `LocalTime.now()`     | Gets the current time.          | `LocalTime.now()` → `10:15:30`                           |
| `LocalDateTime.now()` | Gets the current date and time. | `LocalDateTime.now()`                                    |
| `plusDays(days)`      | Adds days to a date.            | `date.plusDays(5)`                                       |
| `format(formatter)`   | Formats the date/time.          | `date.format(DateTimeFormatter.ofPattern("dd-MM-yyyy"))` |

### **System Methods**

| **Method**                   | **Description**                           | **Example**                   |
| ---------------------------- | ----------------------------------------- | ----------------------------- |
| `System.out.println()`       | Prints to the console.                    | `System.out.println("Hello")` |
| `System.currentTimeMillis()` | Returns the current time in milliseconds. | `System.currentTimeMillis()`  |
| `System.gc()`                | Requests garbage collection.              | `System.gc()`                 |

### **Other Useful Methods**

| **Category** | **Method**            | **Description**                          | **Example**            |
| ------------ | --------------------- | ---------------------------------------- | ---------------------- |
| **File**     | `exists()`            | Checks if a file exists.                 | `file.exists()`        |
|              | `createNewFile()`     | Creates a new file.                      | `file.createNewFile()` |
| **Thread**   | `start()`             | Starts a thread.                         | `thread.start()`       |
|              | `sleep(milliseconds)` | Pauses execution for the specified time. | `Thread.sleep(1000)`   |
| **Scanner**  | `nextLine()`          | Reads the next line of input.            | `scanner.nextLine()`   |

---

### Object Methods

| **Method Name**                 | **Description**                                                            | **Example**                                                             |
| ------------------------------- | -------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `equals(Object obj)`            | Compares objects for equality.                                             | `System.out.println("abc".equals("abc")); // true`                      |
| `hashCode()`                    | Returns hash code for the object.                                          | `System.out.println("abc".hashCode()); // 96354`                        |
| `toString()`                    | Returns string representation of the object.                               | `System.out.println(new Object().toString()); // java.lang.Object@hash` |
| `getClass()`                    | Returns the runtime class of the object.                                   | `System.out.println("abc".getClass()); // class java.lang.String`       |
| `clone()`                       | Creates a copy of the object (requires `Cloneable`).                       | `MyClass obj = (MyClass) obj.clone();`                                  |
| `notify()`                      | Wakes up one waiting thread.                                               | `synchronized(obj) { obj.notify(); }`                                   |
| `notifyAll()`                   | Wakes up all waiting threads.                                              | `synchronized(obj) { obj.notifyAll(); }`                                |
| `wait()`                        | Makes the thread wait until notified.                                      | `synchronized(obj) { obj.wait(); }`                                     |
| `wait(long timeout)`            | Waits for a specified time or until notified.                              | `synchronized(obj) { obj.wait(1000); }`                                 |
| `wait(long timeout, int nanos)` | Waits for a specified time (milliseconds + nanoseconds) or until notified. | `synchronized(obj) { obj.wait(1000, 500); }`                            |

---

---

## Q41: `throw` and `throws`

In Java, `throw` and `throws` are used in exception handling but serve different purposes. Here's an explanation and their differences:

### **1. `throw`**

- **Purpose**: Used to explicitly throw an exception from a method or block of code.
- **Usage**: Follows the keyword with an exception object (either predefined or custom).
- **Example**:
  ```java
  public void checkAge(int age) {
      if (age < 18) {
          throw new IllegalArgumentException("Age must be 18 or above.");
      }
  }
  ```
- **Notes**:
  - The exception object must be created using the `new` keyword.
  - Can be used for both checked and unchecked exceptions.

### **2. `throws`**

- **Purpose**: Declares exceptions that a method might throw, alerting the calling method to handle them.
- **Usage**: Specified in the method signature, followed by the exception type(s).
- **Example**:
  ```java
  public void readFile(String filePath) throws IOException {
      // Code that might throw IOException
      FileReader reader = new FileReader(filePath);
  }
  ```
- **Notes**:
  - Used only for checked exceptions (those that must be handled or declared).
  - You can declare multiple exceptions, separated by commas.

### **Key Differences**

| Aspect         | `throw`                                     | `throws`                                       |
| -------------- | ------------------------------------------- | ---------------------------------------------- |
| **Definition** | Used to throw an exception.                 | Used to declare exceptions a method can throw. |
| **Location**   | Inside the method body.                     | In the method signature.                       |
| **Purpose**    | Actual action of throwing an exception.     | Alerts the caller about possible exceptions.   |
| **Used For**   | Both checked and unchecked exceptions.      | Mainly for checked exceptions.                 |
| **Syntax**     | `throw new Exception();`                    | `throws Exception`                             |
| **Number**     | Only one exception can be thrown at a time. | Multiple exceptions can be declared.           |

### **Example Combining Both**

```java
public class Example {
    // Declaring that this method throws an IOException
    public void readFile(String fileName) throws IOException {
        if (fileName == null) {
            // Throwing an exception
            throw new IOException("File name cannot be null.");
        }
        // Simulating file reading logic
        System.out.println("Reading file: " + fileName);
    }

    public static void main(String[] args) {
        Example example = new Example();
        try {
            example.readFile(null); // This will throw an exception
        } catch (IOException e) {
            System.out.println("Caught exception: " + e.getMessage());
        }
    }
}
```

---

---

## Q42: Exception Handling in Java

**Exception Handling** in Java is a mechanism to handle runtime errors, ensuring the program's normal flow is maintained. It is achieved using **try**, **catch**, **finally**, **throw**, and **throws** constructs.

### **What is an Exception?**

An **exception** is an event that disrupts the normal flow of a program during its execution. Exceptions can occur due to various reasons, such as:

- Invalid user input.
- Dividing a number by zero.
- Attempting to access an array element out of bounds.
- File not found or inaccessible.
- Network connection issues.

### **Types of Exceptions**

1. **Checked Exceptions**:

   - Known as compile-time exceptions.
   - The compiler requires the programmer to handle them explicitly using `try-catch` or by declaring them using `throws`.
   - Examples: `IOException`, `SQLException`.

2. **Unchecked Exceptions**:

   - Known as runtime exceptions.
   - Occur during program execution and are typically due to programming bugs.
   - Examples: `ArithmeticException`, `NullPointerException`, `ArrayIndexOutOfBoundsException`.

3. **Errors**:
   - Serious issues not meant to be caught or handled, often related to the JVM's environment.
   - Examples: `OutOfMemoryError`, `StackOverflowError`.

### **Key Exception Handling Constructs**

#### 1. **try-catch Block**

Used to handle exceptions by placing the risky code inside the `try` block and handling the exception in the `catch` block.

**Syntax**:

```java
try {
    // Risky code that may throw an exception
} catch (ExceptionType e) {
    // Code to handle the exception
}
```

**Example**:

```java
public class Example {
    public static void main(String[] args) {
        try {
            int result = 10 / 0; // This will throw ArithmeticException
        } catch (ArithmeticException e) {
            System.out.println("Cannot divide by zero!");
        }
    }
}
```

#### 2. **finally Block**

- Executed after the `try` and `catch` blocks, regardless of whether an exception occurred.
- Often used for cleanup activities (e.g., closing resources like files or database connections).

**Syntax**:

```java
try {
    // Risky code
} catch (ExceptionType e) {
    // Handle exception
} finally {
    // Code that will always execute
}
```

**Example**:

```java
try {
    int data = 50 / 0;
} catch (ArithmeticException e) {
    System.out.println("Exception caught!");
} finally {
    System.out.println("Finally block executed.");
}
```

#### 3. **throw**

Used to explicitly throw an exception.

**Syntax**:

```java
throw new ExceptionType("Error message");
```

**Example**:

```java
public void checkNumber(int num) {
    if (num < 0) {
        throw new IllegalArgumentException("Number cannot be negative");
    }
}
```

#### 4. **throws**

Used in the method signature to declare exceptions that a method might throw.

**Syntax**:

```java
public void methodName() throws ExceptionType {
    // Code that might throw the exception
}
```

**Example**:

```java
public void readFile(String fileName) throws IOException {
    FileReader reader = new FileReader(fileName);
}
```

### **Best Practices in Exception Handling**

1. **Use Specific Exceptions**:

   - Catch specific exceptions instead of generic ones like `Exception` or `Throwable`.

2. **Don't Swallow Exceptions**:

   - Avoid empty `catch` blocks; always provide meaningful handling or logging.

3. **Use `finally` for Cleanup**:

   - Ensure resources like files, streams, or connections are properly closed.

4. **Don't Overuse Exceptions**:

   - Exceptions should be used for exceptional scenarios, not for controlling normal program flow.

5. **Log Exceptions**:

   - Log exceptions for debugging and maintenance purposes.

6. **Custom Exceptions**:
   - Create custom exceptions for your application's domain-specific errors.

### **Complete Example**

```java
import java.io.*;

public class ExceptionHandlingExample {
    public static void main(String[] args) {
        try {
            FileReader reader = new FileReader("file.txt");
            BufferedReader br = new BufferedReader(reader);

            System.out.println(br.readLine());
            br.close();
        } catch (FileNotFoundException e) {
            System.out.println("File not found: " + e.getMessage());
        } catch (IOException e) {
            System.out.println("Error reading file: " + e.getMessage());
        } finally {
            System.out.println("Execution completed.");
        }
    }
}
```

---

---

## Q43: Exception and Error

In Java, both **Exception** and **Error** are types of **throwable objects** used to indicate abnormal conditions in a program. However, they serve different purposes and represent different kinds of problems. Here's a detailed comparison:

### **1. Exception**

- **Definition**:
  Exceptions represent conditions that a program **might want to catch and handle**. They are recoverable issues, such as invalid input, file not found, or network errors.

- **Subcategories**:

  - **Checked Exceptions**:
    - Must be declared in the `throws` clause or handled using `try-catch`.
    - Examples: `IOException`, `SQLException`.
  - **Unchecked Exceptions (Runtime Exceptions)**:
    - Do not need to be declared or explicitly handled.
    - Examples: `NullPointerException`, `ArithmeticException`.

- **When to Use**:

  - For problems that can be predicted and potentially recovered from, such as user input validation or file access errors.

- **Example**:
  ```java
  public void readFile(String fileName) throws IOException {
      FileReader reader = new FileReader(fileName);
      // Risky code
  }
  ```

### **2. Error**

- **Definition**:
  Errors represent serious conditions that are **beyond the control of the application** and cannot be reasonably handled. They are typically caused by the environment or system issues.

- **Examples**:

  - `OutOfMemoryError`: When the JVM runs out of memory.
  - `StackOverflowError`: When the call stack overflows due to deep recursion.
  - `LinkageError`: When a class cannot be linked during runtime.

- **When to Use**:

  - Errors are generally not meant to be caught or handled. They indicate critical issues that require fixing at the system or code level.

- **Example**:
  ```java
  public void causeStackOverflow() {
      causeStackOverflow(); // Recursive call leading to StackOverflowError
  }
  ```

### **Key Differences**

| **Aspect**        | **Exception**                                          | **Error**                                         |
| ----------------- | ------------------------------------------------------ | ------------------------------------------------- |
| **Nature**        | Represents recoverable problems.                       | Represents irrecoverable, serious issues.         |
| **Handling**      | Can be handled using `try-catch` or `throws`.          | Usually not handled; requires system-level fixes. |
| **Hierarchy**     | Subclass of `java.lang.Throwable`.                     | Subclass of `java.lang.Throwable`.                |
| **Recoverable**   | Yes, the program can continue after handling.          | No, usually the program terminates.               |
| **Examples**      | `IOException`, `NullPointerException`, `SQLException`. | `OutOfMemoryError`, `StackOverflowError`.         |
| **Usage in Code** | Used to handle predictable issues in the program.      | Represents critical system-level failures.        |
| **Focus Area**    | Application-level problems.                            | JVM or system-level problems.                     |

### **Class Hierarchy**

```plaintext
java.lang.Throwable
├── java.lang.Exception
│   ├── Checked Exceptions (e.g., IOException, SQLException)
│   └── Runtime Exceptions (e.g., NullPointerException, ArithmeticException)
└── java.lang.Error
    ├── VirtualMachineError (e.g., OutOfMemoryError, StackOverflowError)
    └── LinkageError (e.g., NoClassDefFoundError)
```

### **When to Catch or Handle**

- **Catch Exceptions**: Use `try-catch` for conditions you can anticipate and recover from, such as invalid user input or file not found.
- **Don't Catch Errors**: Errors like `OutOfMemoryError` or `StackOverflowError` typically indicate problems that require fixing in the code or environment.

### **Example Combining Both**

```java
public class ExceptionErrorDemo {
    public static void main(String[] args) {
        // Example of Exception
        try {
            int result = 10 / 0; // ArithmeticException
        } catch (ArithmeticException e) {
            System.out.println("Handled Exception: " + e.getMessage());
        }

        // Example of Error
        try {
            causeStackOverflow();
        } catch (StackOverflowError e) {
            System.out.println("Caught Error: " + e.getMessage());
        }
    }

    public static void causeStackOverflow() {
        causeStackOverflow(); // Recursive call causing StackOverflowError
    }
}
```

---

---

## Q44: list of commonly used Exceptions and Errors in Java

list of commonly used **Exceptions** and **Errors** in Java:

### **1. Exceptions**

| **Type**                                      | **Class Name**                              | **Description**                                                                  | **Example**                                                  |
| --------------------------------------------- | ------------------------------------------- | -------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| **Checked Exceptions**                        |                                             |                                                                                  |                                                              |
| IOException                                   | `java.io.IOException`                       | Thrown when an I/O operation fails or is interrupted.                            | Reading a non-existent file.                                 |
| FileNotFoundException                         | `java.io.FileNotFoundException`             | Thrown when a file specified by a pathname cannot be found.                      | Trying to read a file that doesn't exist.                    |
| SQLException                                  | `java.sql.SQLException`                     | Thrown when there is a database access or query error.                           | Running an invalid SQL query.                                |
| ClassNotFoundException                        | `java.lang.ClassNotFoundException`          | Thrown when the JVM cannot find a specified class during runtime.                | Using `Class.forName("SomeClass")` for a non-existent class. |
| InterruptedException                          | `java.lang.InterruptedException`            | Thrown when a thread is interrupted while waiting, sleeping, or paused.          | Interrupting a thread during `Thread.sleep()`.               |
| MalformedURLException                         | `java.net.MalformedURLException`            | Thrown when an invalid URL format is used.                                       | Using a malformed URL.                                       |
| **Unchecked Exceptions (Runtime Exceptions)** |                                             |                                                                                  |                                                              |
| NullPointerException                          | `java.lang.NullPointerException`            | Thrown when an application tries to access a method or field on a `null` object. | Accessing methods on a `null` reference.                     |
| ArithmeticException                           | `java.lang.ArithmeticException`             | Thrown when an illegal arithmetic operation occurs.                              | Dividing by zero.                                            |
| ArrayIndexOutOfBoundsException                | `java.lang.ArrayIndexOutOfBoundsException`  | Thrown when accessing an array with an illegal index.                            | Accessing `arr[5]` when the array has 4 elements.            |
| StringIndexOutOfBoundsException               | `java.lang.StringIndexOutOfBoundsException` | Thrown when accessing a string with an invalid index.                            | Accessing the 5th character in a 3-character string.         |
| IllegalArgumentException                      | `java.lang.IllegalArgumentException`        | Thrown when a method receives an invalid argument.                               | Passing a negative value where a positive one is expected.   |
| IllegalStateException                         | `java.lang.IllegalStateException`           | Thrown when a method is invoked in an inappropriate state.                       | Calling `Iterator.next()` when no elements remain.           |
| ClassCastException                            | `java.lang.ClassCastException`              | Thrown when an object is cast to a class it is not an instance of.               | Casting a `String` to `Integer`.                             |
| NumberFormatException                         | `java.lang.NumberFormatException`           | Thrown when attempting to convert a string to a number fails.                    | Parsing `"abc"` as an integer.                               |

### **2. Errors**

| **Type**                   | **Class Name**                   | **Description**                                                      | **Example**                                |
| -------------------------- | -------------------------------- | -------------------------------------------------------------------- | ------------------------------------------ |
| **Virtual Machine Errors** |                                  |                                                                      |                                            |
| OutOfMemoryError           | `java.lang.OutOfMemoryError`     | Thrown when the JVM runs out of memory.                              | Creating too many objects without cleanup. |
| StackOverflowError         | `java.lang.StackOverflowError`   | Thrown when the stack exceeds its size limit (e.g., deep recursion). | Recursive method calls with no base case.  |
| InternalError              | `java.lang.InternalError`        | Thrown when an internal JVM issue occurs.                            | Rare low-level JVM errors.                 |
| UnknownError               | `java.lang.UnknownError`         | Thrown when an unknown but serious JVM issue occurs.                 | Unknown JVM crash.                         |
| **Linkage Errors**         |                                  |                                                                      |                                            |
| NoClassDefFoundError       | `java.lang.NoClassDefFoundError` | Thrown when a required class cannot be found by the JVM.             | Missing a required class at runtime.       |
| ClassFormatError           | `java.lang.ClassFormatError`     | Thrown when a `.class` file does not conform to the expected format. | Using a corrupt `.class` file.             |
| UnsatisfiedLinkError       | `java.lang.UnsatisfiedLinkError` | Thrown when the JVM cannot load a required native library.           | Missing native dependencies for JNI.       |
| **Assertion Errors**       |                                  |                                                                      |                                            |
| AssertionError             | `java.lang.AssertionError`       | Thrown when an assertion fails during debugging/testing.             | `assert x > 0;` fails if `x` is negative.  |

---

---

## Q45: Generics in Java

### **Generics in Java**

Generics were introduced in **Java 5** to provide **type safety** and **reusability**. They allow you to write code that can handle **different data types** without compromising type safety.

### **Why Use Generics?**

1. **Type Safety**: Ensures that the compiler checks the data types, reducing runtime errors.
2. **Code Reusability**: Write a single class or method that works with different types.
3. **Avoid Casting**: Generics eliminate the need for explicit type casting, making the code cleaner.

### **Syntax of Generics**

Generics are denoted using angle brackets `<>` with a type parameter.

- **Type Parameter**: A placeholder for a specific type, such as `T`, `E`, `K`, `V`.
  - `T` - Type
  - `E` - Element
  - `K` - Key
  - `V` - Value

Example:

```java
class GenericClass<T> {
    private T data;

    public void setData(T data) {
        this.data = data;
    }

    public T getData() {
        return data;
    }
}
```

### **Basic Example Without Generics**

Before Generics, a class might look like this:

```java
import java.util.ArrayList;

public class WithoutGenerics {
    public static void main(String[] args) {
        ArrayList list = new ArrayList(); // No type specified
        list.add("Hello");
        list.add(123); // Mixed types allowed

        String value = (String) list.get(0); // Casting required
        System.out.println(value);

        // Causes a runtime error: ClassCastException
        String value2 = (String) list.get(1); // Runtime error!
    }
}
```

### **Basic Example With Generics**

```java
import java.util.ArrayList;

public class WithGenerics {
    public static void main(String[] args) {
        ArrayList<String> list = new ArrayList<>(); // Type specified
        list.add("Hello");
        // list.add(123); // Compile-time error

        String value = list.get(0); // No casting required
        System.out.println(value);
    }
}
```

### **Creating a Generic Class**

```java
class Box<T> {
    private T value;

    public void setValue(T value) {
        this.value = value;
    }

    public T getValue() {
        return value;
    }
}

public class GenericClassExample {
    public static void main(String[] args) {
        Box<Integer> intBox = new Box<>();
        intBox.setValue(10);
        System.out.println("Integer Value: " + intBox.getValue());

        Box<String> strBox = new Box<>();
        strBox.setValue("Hello Generics");
        System.out.println("String Value: " + strBox.getValue());
    }
}
```

### **Creating a Generic Method**

A generic method can accept type parameters independent of the class:

```java
class GenericMethodExample {
    public static <T> void printArray(T[] array) {
        for (T element : array) {
            System.out.print(element + " ");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        Integer[] intArray = {1, 2, 3, 4, 5};
        String[] strArray = {"A", "B", "C"};

        printArray(intArray); // Output: 1 2 3 4 5
        printArray(strArray); // Output: A B C
    }
}
```

### **Generic Interfaces**

A generic interface allows creating reusable contracts:

```java
interface GenericInterface<T> {
    void display(T data);
}

class GenericInterfaceImpl<T> implements GenericInterface<T> {
    @Override
    public void display(T data) {
        System.out.println("Data: " + data);
    }
}

public class GenericInterfaceExample {
    public static void main(String[] args) {
        GenericInterface<String> strImpl = new GenericInterfaceImpl<>();
        strImpl.display("Hello, Interface");

        GenericInterface<Integer> intImpl = new GenericInterfaceImpl<>();
        intImpl.display(100);
    }
}
```

### **Bounded Type Parameters**

Generics can restrict the type of objects it accepts using **bounds**.

#### **Upper Bound**

Restrict to a specific class or subclass:

```java
class BoundedClass<T extends Number> { // Only Number or its subclasses
    private T value;

    public void setValue(T value) {
        this.value = value;
    }

    public T getValue() {
        return value;
    }
}

public class BoundedTypeExample {
    public static void main(String[] args) {
        BoundedClass<Integer> intBox = new BoundedClass<>();
        intBox.setValue(10);

        BoundedClass<Double> doubleBox = new BoundedClass<>();
        doubleBox.setValue(15.5);

        // BoundedClass<String> strBox = new BoundedClass<>(); // Compile-time error
    }
}
```

#### **Lower Bound**

Use `super` keyword to restrict a type to a superclass.

### **Wildcards in Generics**

Wildcards (`?`) allow for flexibility in working with generics.

#### **Unbounded Wildcard**

Accepts any type:

```java
public void printList(List<?> list) {
    for (Object obj : list) {
        System.out.println(obj);
    }
}
```

#### **Upper-Bounded Wildcard**

Restrict to a specific class or subclass:

```java
public void printNumbers(List<? extends Number> list) {
    for (Number num : list) {
        System.out.println(num);
    }
}
```

#### **Lower-Bounded Wildcard**

Restrict to a specific class or superclass:

```java
public void addNumbers(List<? super Integer> list) {
    list.add(10); // Adding an Integer
}
```

---

### **1. Why Use Generics?**

Generics address several issues in Java programming, making code more robust and reusable. Here's why they are essential:

1. **Type Safety**  
   Without generics, you can store any object in a collection, which can lead to runtime errors. Generics ensure type consistency at compile time.

   Example (Without Generics):

   ```java
   List list = new ArrayList();
   list.add("Hello");
   list.add(123); // Allowed
   String str = (String) list.get(1); // Runtime error
   ```

   Example (With Generics):

   ```java
   List<String> list = new ArrayList<>();
   list.add("Hello");
   // list.add(123); // Compile-time error
   ```

2. **Code Reusability**  
   Generics allow you to create a single class or method that works with multiple data types.

3. **Avoid Casting**  
   Without generics, you must cast objects retrieved from collections to their original type. Generics eliminate the need for explicit casting.

### **2. What Are Generics?**

Generics allow classes, interfaces, and methods to operate on **types** specified as parameters. They enable **type abstraction**, making the code more flexible and robust.

- **Definition**: Generics are a way to write type-safe and reusable code. They are defined with **angle brackets `<T>`**, where `T` is a placeholder for a type.

Key Concepts:

- **T**: Type (can be any type like Integer, String, etc.)
- **E**: Element (used in collections)
- **K, V**: Key, Value (used in maps)

### **3. How to Use Generics?**

Generics can be applied to classes, methods, and interfaces.

#### **a. Generic Class**

A class that can handle any type:

```java
class Box<T> {
    private T value;

    public void setValue(T value) {
        this.value = value;
    }

    public T getValue() {
        return value;
    }
}

public class Main {
    public static void main(String[] args) {
        Box<Integer> intBox = new Box<>();
        intBox.setValue(10);
        System.out.println("Integer Value: " + intBox.getValue());

        Box<String> strBox = new Box<>();
        strBox.setValue("Hello Generics");
        System.out.println("String Value: " + strBox.getValue());
    }
}
```

#### **b. Generic Method**

A method that accepts type parameters:

```java
class GenericMethodExample {
    public static <T> void printArray(T[] array) {
        for (T element : array) {
            System.out.print(element + " ");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        Integer[] intArray = {1, 2, 3};
        String[] strArray = {"A", "B", "C"};

        printArray(intArray); // Prints: 1 2 3
        printArray(strArray); // Prints: A B C
    }
}
```

#### **c. Generic Interface**

Interfaces can also use generics:

```java
interface GenericInterface<T> {
    void display(T data);
}

class GenericClass<T> implements GenericInterface<T> {
    @Override
    public void display(T data) {
        System.out.println("Data: " + data);
    }
}

public class Main {
    public static void main(String[] args) {
        GenericInterface<String> obj = new GenericClass<>();
        obj.display("Hello Generics");
    }
}
```

#### **d. Wildcards in Generics**

Wildcards allow flexibility:

- `<?>`: Unbounded wildcard.
- `<? extends T>`: Upper-bounded wildcard (subtypes of T).
- `<? super T>`: Lower-bounded wildcard (supertypes of T).

Example:

```java
public void printList(List<?> list) {
    for (Object obj : list) {
        System.out.println(obj);
    }
}
```

### **4. When to Use Generics?**

Generics should be used when:

1. **You want type safety**: To prevent runtime type errors.
   - Use in collections like `List<T>`, `Set<T>`, or `Map<K, V>`.
2. **You want reusability**: When creating classes or methods that operate on various types.
   - Example: A class like `Box<T>` or a method like `<T> void swap(T a, T b)`.
3. **You want flexibility**: To make code adaptable to future changes.
   - Example: Writing methods or classes that support unknown or multiple types using wildcards.
4. **You want to avoid casting**: To make code cleaner and more maintainable.
   - Example: Avoid explicit casting while retrieving elements from collections.

### **Advantages of Generics**

1. **Compile-Time Checking**: Detects errors early.
2. **Code Reusability**: Avoids rewriting similar code for different types.
3. **Readability and Maintainability**: Cleaner and more expressive code.
4. **Performance**: Avoids the overhead of type casting.

### **Key Notes**

- Generics work only with reference types (e.g., `Integer`, `String`) and not with primitive types (`int`, `double`). Use wrapper classes instead (`Integer` for `int`).
- Generics are implemented using **type erasure** in Java, which means type parameters are replaced with their bounds or `Object` during compilation.

---

---

## Q46: Object Cloning in Java

### **Object Cloning in Java**

**Object Cloning** is a process of creating an exact copy of an existing object in Java. Java provides a mechanism for cloning objects through the **`Cloneable` interface** and the **`clone()`** method.

### **Why Use Object Cloning?**

- To duplicate an object without creating it from scratch.
- It’s faster than creating a new object and copying properties manually.
- Useful in scenarios like prototyping or creating backups of objects.

### **How to Perform Cloning in Java?**

#### **1. Implementing `Cloneable` Interface**

To enable cloning, a class must:

1. **Implement `Cloneable` interface**: This is a marker interface (no methods to implement) that signals the JVM that cloning is allowed.
2. **Override the `clone()` method**: This method in the `Object` class performs the cloning.

#### **Example of Cloning**

```java
class Person implements Cloneable {
    String name;
    int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    protected Object clone() throws CloneNotSupportedException {
        return super.clone(); // Creates a shallow copy
    }
}

public class Main {
    public static void main(String[] args) {
        try {
            Person person1 = new Person("John", 30);
            Person person2 = (Person) person1.clone(); // Cloning person1

            System.out.println("Original: " + person1.name + ", " + person1.age);
            System.out.println("Clone: " + person2.name + ", " + person2.age);
        } catch (CloneNotSupportedException e) {
            e.printStackTrace();
        }
    }
}
```

### **Shallow Copy vs. Deep Copy**

The type of cloning determines how object references within the object are handled.

#### **1. Shallow Copy**

- Copies **only the top-level object** and not the objects it references.
- References to other objects are shared between the original and cloned objects.
- Achieved by directly calling `super.clone()`.

**Example**:

```java
class Address {
    String city;

    public Address(String city) {
        this.city = city;
    }
}

class Person implements Cloneable {
    String name;
    Address address;

    public Person(String name, Address address) {
        this.name = name;
        this.address = address;
    }

    @Override
    protected Object clone() throws CloneNotSupportedException {
        return super.clone(); // Shallow copy
    }
}

public class Main {
    public static void main(String[] args) throws CloneNotSupportedException {
        Address address = new Address("New York");
        Person person1 = new Person("John", address);
        Person person2 = (Person) person1.clone();

        // Modifying the address of person2
        person2.address.city = "Los Angeles";

        System.out.println("Person1 Address: " + person1.address.city); // "Los Angeles"
        System.out.println("Person2 Address: " + person2.address.city); // "Los Angeles"
    }
}
```

In a **shallow copy**, changes to the referenced objects affect both the original and the clone.

#### **2. Deep Copy**

- Copies the top-level object and also **creates new copies of all referenced objects**.
- Requires manually cloning each referenced object.
- Ensures that changes in the cloned object do not affect the original object.

**Example**:

```java
class Address implements Cloneable {
    String city;

    public Address(String city) {
        this.city = city;
    }

    @Override
    protected Object clone() throws CloneNotSupportedException {
        return super.clone(); // Clone the Address object
    }
}

class Person implements Cloneable {
    String name;
    Address address;

    public Person(String name, Address address) {
        this.name = name;
        this.address = address;
    }

    @Override
    protected Object clone() throws CloneNotSupportedException {
        Person cloned = (Person) super.clone();
        cloned.address = (Address) address.clone(); // Clone the Address separately
        return cloned;
    }
}

public class Main {
    public static void main(String[] args) throws CloneNotSupportedException {
        Address address = new Address("New York");
        Person person1 = new Person("John", address);
        Person person2 = (Person) person1.clone();

        // Modifying the address of person2
        person2.address.city = "Los Angeles";

        System.out.println("Person1 Address: " + person1.address.city); // "New York"
        System.out.println("Person2 Address: " + person2.address.city); // "Los Angeles"
    }
}
```

In a **deep copy**, changes to the referenced objects in the clone do not affect the original object.

### **Key Differences Between Shallow Copy and Deep Copy**

| **Aspect**             | **Shallow Copy**                                          | **Deep Copy**                                       |
| ---------------------- | --------------------------------------------------------- | --------------------------------------------------- |
| **Definition**         | Copies only the top-level object.                         | Copies the top-level object and referenced objects. |
| **Reference Handling** | References are shared between the original and the clone. | Creates new copies of referenced objects.           |
| **Changes in Clone**   | Affect the original object.                               | Do not affect the original object.                  |
| **Performance**        | Faster (less memory usage).                               | Slower (more memory usage).                         |
| **Use Case**           | Suitable when referenced objects are immutable.           | Necessary when referenced objects are mutable.      |

### **Best Practices for Cloning**

1. **Prefer Deep Copy** when you need independent copies.
2. Use libraries like **Apache Commons Lang** or **serialization** for complex cloning needs.
3. Always handle the `CloneNotSupportedException`.
4. Avoid excessive use of cloning if it complicates your design—consider alternative approaches like constructors or factory methods.

---

---

## Q47: Collection Framework in Java

The **Collection Framework** in Java is a set of classes and interfaces that implement commonly used collection data structures, such as lists, sets, and maps. It provides a unified architecture for storing and manipulating groups of objects. The framework is part of the `java.util` package and includes several key interfaces, classes, and algorithms.

### Key Interfaces

1. **Collection**: The root interface in the collection hierarchy. It defines basic operations for all collections.

   - Methods: `add()`, `remove()`, `size()`, `clear()`, etc.

2. **List**: Extends `Collection` and represents an ordered collection that may contain duplicate elements.

   - Implementing classes: `ArrayList`, `LinkedList`, `Vector`, `Stack`.
   - Common methods: `get()`, `set()`, `add()`, `remove()`, `size()`, `contains()`.

3. **Set**: Extends `Collection` and represents an unordered collection that does not allow duplicate elements.

   - Implementing classes: `HashSet`, `LinkedHashSet`, `TreeSet`.
   - Common methods: `add()`, `remove()`, `size()`, `contains()`.

4. **Queue**: Extends `Collection` and represents a collection designed for holding elements before processing. It follows the FIFO (First In, First Out) principle.

   - Implementing classes: `LinkedList`, `PriorityQueue`, `ArrayDeque`.
   - Common methods: `offer()`, `poll()`, `peek()`.

5. **Deque**: Extends `Queue` and represents a double-ended queue. It allows adding and removing elements from both ends.

   - Implementing classes: `ArrayDeque`, `LinkedList`.
   - Common methods: `addFirst()`, `addLast()`, `removeFirst()`, `removeLast()`.

6. **Map**: Represents a collection of key-value pairs. It is not a true subclass of `Collection` but is part of the collection framework.
   - Implementing classes: `HashMap`, `LinkedHashMap`, `TreeMap`, `Hashtable`, `ConcurrentHashMap`.
   - Common methods: `put()`, `get()`, `remove()`, `containsKey()`, `keySet()`.

### Implementing Classes

- **ArrayList**: A resizable array implementation of the `List` interface. It allows fast random access but slow insertion/removal from the middle of the list.
- **LinkedList**: A doubly linked list implementation of the `List` and `Deque` interfaces. It allows fast insertions and deletions but slower access by index.
- **HashSet**: A collection that implements the `Set` interface and stores elements in a hash table. It does not allow duplicates and does not guarantee any specific order.
- **TreeSet**: A collection that implements the `Set` interface and stores elements in a sorted order, based on their natural ordering or a provided comparator.
- **HashMap**: A collection that implements the `Map` interface and stores key-value pairs. It uses a hash table for fast lookups.

### Algorithms

The **Collection Framework** also provides useful algorithms that can be applied to collections:

- **Sorting**: The `Collections` class provides static methods like `sort()`, `reverse()`, `shuffle()`.
- **Searching**: Methods such as `binarySearch()` are available in the `Collections` class.

### Advantages of the Collection Framework

- **Unified architecture**: All collections implement common interfaces like `Collection`, `Set`, `List`, etc.
- **Reusability**: You can use pre-built classes like `ArrayList`, `HashSet`, and `HashMap` for common tasks.
- **Flexibility**: You can choose the appropriate collection class depending on the performance needs (e.g., fast access, fast insertion, ordering, etc.).
- **Improved performance**: Collections like `HashMap` and `HashSet` use hashing for fast access.

### Example

```java
import java.util.*;

public class CollectionExample {
    public static void main(String[] args) {
        // List example
        List<String> list = new ArrayList<>();
        list.add("Apple");
        list.add("Banana");
        list.add("Cherry");
        System.out.println("List: " + list);

        // Set example
        Set<String> set = new HashSet<>();
        set.add("Apple");
        set.add("Banana");
        set.add("Apple"); // Duplicate will not be added
        System.out.println("Set: " + set);

        // Map example
        Map<Integer, String> map = new HashMap<>();
        map.put(1, "Apple");
        map.put(2, "Banana");
        map.put(3, "Cherry");
        System.out.println("Map: " + map);
    }
}
```

### Output:

```
List: [Apple, Banana, Cherry]
Set: [Apple, Banana]
Map: {1=Apple, 2=Banana, 3=Cherry}
```

---

Here's a more detailed textual representation of the Java Collection Framework:

```
                            Collection
                               |
       +-----------------------+------------------------+
       |                                              |
     Set (unordered)                                  List (ordered)
       |                                              |
  +------------+                              +-----------------+
  |            |                              |                 |
HashSet   LinkedHashSet                  ArrayList        LinkedList
  |            |                              |                 |
  |      +------------+                +-------------+        +-----------+
  |      |            |                |             |        |           |
TreeSet  EnumSet   CopyOnWriteArraySet Vector        Stack   ConcurrentLinkedQueue
                                                       |
                                                   PriorityQueue

                     Queue (FIFO)                         Map (key-value pairs)
                         |                                 |
               +------------------+               +---------------------------+
               |                  |               |                           |
        LinkedList             PriorityQueue  HashMap                 TreeMap
               |                  |               |                           |
           ArrayDeque      LinkedBlockingQueue  LinkedHashMap           ConcurrentHashMap
               |                                         |
    Deque (Double-ended Queue)                         WeakHashMap
```

### Detailed Breakdown:

1. **Collection Interface**:
   - The root interface in the collection hierarchy.
2. **Set Interface** (Ordered: No):

   - A collection that doesn't allow duplicate elements.
   - **HashSet**: Does not maintain the order of elements.
   - **LinkedHashSet**: Maintains the order of elements as they were inserted.
   - **TreeSet**: A set that maintains elements in a sorted order (based on natural ordering or a custom comparator).
   - **EnumSet**: A specialized set for use with enum types.
   - **CopyOnWriteArraySet**: A thread-safe implementation of a set.

3. **List Interface** (Ordered: Yes):

   - A collection that allows duplicate elements and preserves order.
   - **ArrayList**: A resizable array-based implementation of the List interface.
   - **LinkedList**: A doubly-linked list implementation of the List interface.
   - **Vector**: A thread-safe, growable array that is synchronized.
   - **Stack**: A subclass of Vector that implements a last-in, first-out (LIFO) stack.
   - **Vector** and **Stack** are legacy classes but are still in use.

4. **Queue Interface** (FIFO: First-In, First-Out):

   - A collection designed for holding elements prior to processing.
   - **LinkedList**: A doubly-linked list implementation that also implements Queue.
   - **PriorityQueue**: A queue where the elements are ordered based on their natural ordering or by a comparator.
   - **ArrayDeque**: A resizable array implementation of a deque (double-ended queue).
   - **LinkedBlockingQueue**: A thread-safe blocking queue implementation.
   - **ConcurrentLinkedQueue**: A non-blocking, thread-safe queue.

5. **Deque Interface** (Double-ended Queue):
   - A collection that supports insertion, removal, and access at both ends.
   - **ArrayDeque**: Provides fast, random access to the elements at both ends.
6. **Map Interface** (Key-Value Pairs):
   - A collection of key-value pairs, where each key is associated with exactly one value.
   - **HashMap**: A map that does not maintain any order.
   - **TreeMap**: A map that maintains the order of keys based on their natural ordering or a comparator.
   - **LinkedHashMap**: A map that maintains insertion order.
   - **WeakHashMap**: A map where the keys are weakly referenced (garbage collection can remove them).
   - **ConcurrentHashMap**: A thread-safe map designed for concurrent access.

### Additional Notes:

- **Thread-Safety**: Some of the classes like `CopyOnWriteArraySet`, `ConcurrentLinkedQueue`, `LinkedBlockingQueue`, and `ConcurrentHashMap` are designed for thread-safe operations.
- **Legacy Collections**: `Vector` and `Stack` are part of the original Java collections framework, but newer alternatives such as `ArrayList` and `Deque` are preferred in most cases.

---

---

## Q48: Enums in Java

### **Enums in Java - Deep Dive**

In Java, **enums** (short for enumerations) are a special data type used to define collections of constants. They were introduced in **Java 5** and provide a type-safe way to represent a fixed set of constants (like days of the week, months of the year, or states in a process). Enums are more powerful than simple constants (like `static final` variables) because they can have fields, methods, and constructors.

Let’s explore enums in depth:

### 1. **Basic Enum Declaration**

An enum is declared using the `enum` keyword. The constants of the enum are defined in a comma-separated list inside curly braces.

```java
public enum Day {
    SUNDAY, MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY;
}
```

- `Day` is the enum type.
- `SUNDAY`, `MONDAY`, etc., are the enum constants.

#### **Usage:**

```java
public class TestEnum {
    public static void main(String[] args) {
        Day today = Day.MONDAY;
        System.out.println(today);  // Output: MONDAY
    }
}
```

### 2. **Enum with Fields, Constructors, and Methods**

Enums in Java can have fields, constructors, and methods. This makes enums more powerful, as they allow us to associate additional data and behavior with the constants.

#### **Example: Enum with Fields and Methods**

```java
public enum Day {
    SUNDAY("Relax", 1),
    MONDAY("Work", 2),
    TUESDAY("Work", 3),
    WEDNESDAY("Work", 4),
    THURSDAY("Work", 5),
    FRIDAY("Work", 6),
    SATURDAY("Relax", 7);

    private final String activity; // field
    private final int dayNumber;   // field

    // Constructor
    private Day(String activity, int dayNumber) {
        this.activity = activity;
        this.dayNumber = dayNumber;
    }

    // Method to get the activity
    public String getActivity() {
        return activity;
    }

    // Method to get the day number
    public int getDayNumber() {
        return dayNumber;
    }
}
```

#### **Usage:**

```java
public class EnumExample {
    public static void main(String[] args) {
        for (Day day : Day.values()) {
            System.out.println(day + " -> " + day.getActivity() + " (" + day.getDayNumber() + ")");
        }
    }
}
```

**Output:**

```
SUNDAY -> Relax (1)
MONDAY -> Work (2)
TUESDAY -> Work (3)
WEDNESDAY -> Work (4)
THURSDAY -> Work (5)
FRIDAY -> Work (6)
SATURDAY -> Relax (7)
```

### 3. **Enum Methods**

Java automatically provides several methods for enums. Some of the most commonly used methods are:

- **`values()`**: Returns an array of all the enum constants in the order they are declared.
- **`valueOf(String name)`**: Returns the enum constant with the specified name.
- **`ordinal()`**: Returns the ordinal value (index) of the enum constant (its position in the enum declaration).
- **`name()`**: Returns the name of the enum constant.

#### Example Usage:

```java
public class EnumMethods {
    public static void main(String[] args) {
        // Using valueOf() to get an enum constant
        Day day = Day.valueOf("MONDAY");
        System.out.println(day);  // Output: MONDAY

        // Using ordinal() to get the position of an enum constant
        System.out.println(Day.MONDAY.ordinal());  // Output: 1

        // Using name() to get the name of the enum constant
        System.out.println(Day.MONDAY.name());  // Output: MONDAY
    }
}
```

### 4. **Enum with Abstract Methods**

Enums can also have abstract methods. Every enum constant can provide its own implementation of the abstract method. This is useful when different constants need different behavior.

#### Example:

```java
public enum Day {
    SUNDAY {
        public String getActivity() {
            return "Relax";
        }
    },
    MONDAY {
        public String getActivity() {
            return "Work";
        }
    },
    SATURDAY {
        public String getActivity() {
            return "Play";
        }
    };

    // Abstract method
    public abstract String getActivity();
}
```

### 5. **Enum with `switch` Statement**

Enums are often used with the `switch` statement. Since enums are constants, they provide a clean, readable way to handle different cases.

```java
public class SwitchEnum {
    public static void main(String[] args) {
        Day day = Day.MONDAY;

        switch (day) {
            case MONDAY:
                System.out.println("Start of the week");
                break;
            case SUNDAY:
                System.out.println("Relaxing day");
                break;
            default:
                System.out.println("Midweek");
        }
    }
}
```

### 6. **Enum Singleton Pattern**

An enum is often used to implement the Singleton design pattern because of its thread-safe and serialization properties.

#### Example:

```java
public enum Singleton {
    INSTANCE;

    public void showMessage() {
        System.out.println("Hello from Singleton!");
    }
}
```

You can access the singleton instance using `Singleton.INSTANCE`.

```java
public class SingletonExample {
    public static void main(String[] args) {
        Singleton.INSTANCE.showMessage();
    }
}
```

### 7. **Enum and Interfaces**

Enums can also implement interfaces. Each enum constant must provide its own implementation of the methods defined in the interface.

#### Example:

```java
interface Action {
    void performAction();
}

public enum Day implements Action {
    SUNDAY {
        public void performAction() {
            System.out.println("Relax");
        }
    },
    MONDAY {
        public void performAction() {
            System.out.println("Start work");
        }
    };

    // Optional: Enum methods can also have additional logic
    public abstract void performAction();
}
```

### 8. **Comparing Enums**

You can compare enums using `==` or `equals()` method.

```java
public class EnumComparison {
    public static void main(String[] args) {
        Day day1 = Day.MONDAY;
        Day day2 = Day.MONDAY;
        Day day3 = Day.SUNDAY;

        System.out.println(day1 == day2); // true
        System.out.println(day1.equals(day3)); // false
    }
}
```

### 9. **Enum in Collections**

Since enums are objects, they can be stored in collections like lists, sets, or maps.

```java
import java.util.EnumSet;

public class EnumSetExample {
    public static void main(String[] args) {
        EnumSet<Day> weekend = EnumSet.of(Day.SUNDAY, Day.SATURDAY);
        System.out.println(weekend);
    }
}
```

### Key Points About Enums in Java:

1. **Type Safety**: Enums provide type safety by ensuring that you can only use predefined constants.
2. **Singleton Nature**: Each enum constant is a singleton, meaning there’s only one instance of each constant.
3. **Serialization**: Enums are inherently serializable, so they can be safely used in serialized contexts (like saving and loading objects).
4. **Inheritance**: Enums cannot extend other classes, but they can implement interfaces.
5. **Built-in Methods**: Enums come with a set of built-in methods like `valueOf()`, `ordinal()`, `values()`, `name()`, and more.

### Conclusion

Enums in Java offer a powerful way to define a fixed set of constants. They are much more flexible and powerful than traditional constants, as they can have fields, methods, and constructors. Enums are also useful in implementing design patterns like Singleton and when you need to represent a finite set of values, such as days of the week, states, or commands.
