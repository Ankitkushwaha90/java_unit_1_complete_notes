# it's running code in java 22 version

# Java Environment
The Java environment consists of the JVM, JRE, and JDK, which provide the necessary tools to develop and run Java applications.

### Java Source File Structure and Compilation
A typical Java source file contains:

Package Declaration: package com.example;
Import Statements: import java.util.*;
Class Declaration: public class MyClass { ... }
Compilation:

```bash
javac MyClass.java
java MyClass
```
Fundamental Programming Structures in Java
Defining Classes in Java
```java
public class MyClass {
    // Class body
}
```
### Constructors
```java
public class MyClass {
    int x;

    // Constructor
    public MyClass(int y) {
        x = y;
    }
}
```
### Methods
```java
public class MyClass {
    int x;

    public MyClass(int y) {
        x = y;
    }

    public void display() {
        System.out.println("Value of x: " + x);
    }
}
```
### Access Specifiers
```java
public class MyClass {
    public int publicVar;
    private int privateVar;
    protected int protectedVar;
    int defaultVar; // default access
}
```
### Static Members
```java
public class MyClass {
    public static int staticVar;

    public static void staticMethod() {
        System.out.println("Static method called.");
    }
}
```
### Final Members
```java
public class MyClass {
    public final int finalVar = 10;

    public final void finalMethod() {
        System.out.println("Final method called.");
    }
}
```
### Comments
```java
public class MyClass {
    // This is a single-line comment

    /*
     * This is a multi-line comment
     */

    /**
     * This is a Javadoc comment
     */
}
```
### Data Types and Variables
```java
public class MyClass {
    int integerVar = 5;
    double doubleVar = 5.99;
    char charVar = 'D';
    boolean boolVar = true;
    String stringVar = "Hello";
}
```
### Operators
```java
public class MyClass {
    int sum = 5 + 3;
    int diff = 5 - 3;
    int product = 5 * 3;
    int quotient = 5 / 3;
    int remainder = 5 % 3;

    boolean isEqual = (5 == 3);
    boolean isNotEqual = (5 != 3);
    boolean isGreater = (5 > 3);
    boolean isLess = (5 < 3);
    boolean isGreaterOrEqual = (5 >= 3);
    boolean isLessOrEqual = (5 <= 3);
}
```
### Control Flow
```java
public class MyClass {
    public static void main(String[] args) {
        // if-else
        int x = 10;
        if (x > 5) {
            System.out.println("x is greater than 5");
        } else {
            System.out.println("x is less than or equal to 5");
        }

        // switch
        int day = 2;
        switch (day) {
            case 1:
                System.out.println("Monday");
                break;
            case 2:
                System.out.println("Tuesday");
                break;
            default:
                System.out.println("Other day");
                break;
        }

        // while loop
        int i = 0;
        while (i < 5) {
            System.out.println(i);
            i++;
        }

        // for loop
        for (int j = 0; j < 5; j++) {
            System.out.println(j);
        }
    }
}
```
### Arrays and Strings
```java
public class MyClass {
    public static void main(String[] args) {
        // Arrays
        int[] numbers = {1, 2, 3, 4, 5};
        for (int number : numbers) {
            System.out.println(number);
        }

        // Strings
        String greeting = "Hello, World!";
        System.out.println(greeting);
    }
}
```
### Object-Oriented Programming
Class and Object
```java
public class MyClass {
    int x;

    public MyClass(int y) {
        x = y;
    }

    public static void main(String[] args) {
        MyClass obj = new MyClass(5);
        System.out.println(obj.x);
    }
}
```
### Inheritance
```java
class Animal {
    public void eat() {
        System.out.println("This animal eats food.");
    }
}

class Dog extends Animal {
    public void bark() {
        System.out.println("The dog barks.");
    }
}

public class MyClass {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.eat();
        dog.bark();
    }
}
```
### Overriding
```java
class Animal {
    public void sound() {
        System.out.println("This animal makes a sound.");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("The dog barks.");
    }
}

public class MyClass {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.sound();
    }
}
```
### Overloading
```java
public class MyClass {
    public void display(int a) {
        System.out.println("Argument: " + a);
    }

    public void display(int a, int b) {
        System.out.println("Arguments: " + a + ", " + b);
    }

    public static void main(String[] args) {
        MyClass obj = new MyClass();
        obj.display(1);
        obj.display(1, 2);
    }
}
```
### Encapsulation
```java
public class MyClass {
    private int age;

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

    public static void main(String[] args) {
        MyClass obj = new MyClass();
        obj.setAge(25);
        System.out.println(obj.getAge());
    }
}
```
### Polymorphism
```java
class Animal {
    public void sound() {
        System.out.println("This animal makes a sound.");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("The dog barks.");
    }
}

class Cat extends Animal {
    @Override
    public void sound() {
        System.out.println("The cat meows.");
    }
}

public class MyClass {
    public static void main(String[] args) {
        Animal myDog = new Dog();
        Animal myCat = new Cat();
        myDog.sound();
        myCat.sound();
    }
}
```
### Abstraction
```java
abstract class Animal {
    public abstract void sound();
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("The dog barks.");
    }
}

public class MyClass {
    public static void main(String[] args) {
        Animal myDog = new Dog();
        myDog.sound();
    }
}
```
### Interfaces
```java
interface Animal {
    void sound();
}

class Dog implements Animal {
    @Override
    public void sound() {
        System.out.println("The dog barks.");
    }
}

public class MyClass {
    public static void main(String[] args) {
        Animal myDog = new Dog();
        myDog.sound();
    }
}
```
### Packages
Defining Package
```java
package com.example;

public class MyClass {
    public static void main(String[] args) {
        System.out.println("Package Example");
    }
}
```
### CLASSPATH Setting for Packages
You can set the CLASSPATH environment variable to include the directories of your packages.

```bash
export CLASSPATH=/path/to/your/classes:/path/to/your/jars
```
###Making JAR Files for Library Packages
```bash
jar cf mylibrary
```
