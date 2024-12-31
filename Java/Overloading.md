# Overloading Methods in Java

In Java, it is possible to define two or more methods within the same class that share the same name, as long as their parameter declarations are different. While overloaded methods may have different return types, the return type alone is insufficient to distinguish two versions of a method.

When Java encounters a call to an overloaded method, it executes the version of the method whose parameters match the arguments used in the call. In some cases, Java’s automatic type conversions can play a role in overload resolution.

### Example: Overloading

```java
class OverloadDemo {
    void test(double a) {
        System.out.println("Inside test(double) a: " + a);
    }
}

class Overload {
    public static void main(String args[]) {
        OverloadDemo ob = new OverloadDemo();
        int i = 88;
        ob.test(i);        // this will invoke test(double)
        ob.test(123.2);    // this will invoke test(double)
    }
}
```

### Explanation:

In the above example:

- The `OverloadDemo` class defines a `test(double)` method.
- When `test()` is called with an integer argument, no matching `test(int)` method is found.
- Java automatically converts the integer to a double (using automatic type conversion) and invokes `test(double)`.

If `test(int)` had been defined, it would have been called instead. Java employs its automatic type conversions only if no exact match is found.

---

### Returning Objects in Java

Java methods can return objects. When a method creates and returns an object, it provides a reference to the calling code. Objects created within a method continue to exist as long as there is a reference to them.

### Example: Returning an Object

```java
// Returning an object
class Test {
    int a;

    Test(int i) {
        a = i;
    }

    Test incrByTen() {
        Test temp = new Test(a + 10);
        return temp;
    }
}

class RetOb {
    public static void main(String args[]) {
        Test ob1 = new Test(2);
        Test ob2;

        ob2 = ob1.incrByTen();
        System.out.println("ob1.a: " + ob1.a);
        System.out.println("ob2.a: " + ob2.a);
    }
}
```

### Output:

```
ob1.a: 2
ob2.a: 12
```

### Explanation:

- Each time the `incrByTen()` method is invoked, a new `Test` object is created and returned.
- In the `main()` method:
  - `ob1` refers to the original object with `a = 2`.
  - `ob2` refers to the new object with `a = 12`.

Objects in Java are dynamically allocated using `new`, so they persist as long as there is a reference to them. When no references to an object exist, it becomes eligible for garbage collection.
