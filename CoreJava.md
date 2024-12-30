## **Core Java**

- [Features of Java?](#q1-features-of-java)
- [What is a Compiler?](#q2-what-is-a-compiler)
- [Classes and Objects in Java?](#q3-classes-and-objects-in-java)
- [wrapper classes classes Java?](#q4-wrapper-classes-classes-java)

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

### **Static Keyword in Java**

The `static` keyword in Java is used to define members (variables, methods, blocks, and nested classes) that belong to the class rather than any specific object. These members are shared across all instances of the class.

## Q6: What is `static` in Java?

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
