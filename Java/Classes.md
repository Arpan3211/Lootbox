# Java Concepts: Classes and Objects

## Classes and Objects

- **A class** is a template for an object, and an object is an instance of a class.
- A class creates a new data type that can be used to create objects.
- When you declare an object of a class, you are creating an instance of that class.
  - A class is a logical construct.
  - An object has physical reality (i.e., it occupies space in memory).

### Object Characteristics

Objects are characterized by three essential properties:

1. **State**: The value from its data type.
2. **Identity**: Distinguishes one object from another. The identity can be thought of as the location where the object’s value is stored in memory.
3. **Behavior**: The effect of data-type operations.

## The Dot Operator (`.`)

- Links the name of the object with the name of an instance variable.
- Formally categorized in Java as a separator.

## The `new` Keyword

- Dynamically allocates memory for an object at runtime and returns a reference to it.
- The reference (essentially the address in memory) is stored in a variable.
- All class objects in Java must be dynamically allocated.

Example:

```java
Box mybox; // declare reference to object
mybox = new Box(); // allocate a Box object
```

- The first line declares `mybox` as a reference to an object of type `Box`.
- The second line allocates an object and assigns its reference to `mybox`.

### Important Notes on Object References

- In Java, you cannot manipulate references like pointers.
- References cannot point to arbitrary memory locations or be manipulated like integers.

## A Closer Look at `new`

General Syntax:

```java
classname class-var = new classname();
```

- `class-var`: A variable of the class type being created.
- `classname()`: Specifies the constructor for the class, which defines what occurs when an object is created.

### Why `new` is Not Used for Primitives

- Java’s primitive types (e.g., integers, characters) are implemented as “normal” variables, not objects, for efficiency.

### Example of Shared Object References

```java
Box b1 = new Box();
Box b2 = b1;
```

- Both `b1` and `b2` refer to the same object.
- Assigning `b1` to `b2` does not allocate memory or copy the object.
- Changes made through `b2` will reflect in `b1` since they reference the same object.

### Method Parameters and Arguments

- A **parameter** is a variable defined by a method that receives a value when the method is called.
  - Example: In `square(int i)`, `i` is a parameter.
- An **argument** is the value passed to a method when invoked.
  - Example: `square(100)` passes `100` as an argument.

Example:

```java
int square(int i) {
    return i * i;
}
```

## Important Notes

- **Compilation and Execution**:
  - The **left-hand side (lhs)** (reference, e.g., `bus`) is checked by the compiler.
  - The **right-hand side (rhs)** (object, e.g., `new Bus()`) is processed by the JVM.

Example:

```java
Bus bus = new Bus();
```
