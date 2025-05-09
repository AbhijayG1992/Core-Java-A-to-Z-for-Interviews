
# Java Programming Basics

This README provides a detailed overview of foundational Java programming concepts including methods, computation, input/output, data types, operators, conditionals, and loops.

---

## 📌 Introduction to Java

Java is a high-level, object-oriented programming language. At its core, Java programs consist of **methods**, which perform tasks using input, processing logic, and producing output.

---

## 🧱 Method of a Java Program

### What is a Method?
A **method** in Java is a block of code that performs a specific task. It's the fundamental building block of any Java program.

### Method Components
- **Input**: Data provided to the method.
- **Processing**: Operations performed on the input.
- **Output**: The result after processing.

### Example of Built-in Methods:
```java
public class MyJavaApp {
    public static void main(String[] args) {
        System.out.println(Math.round(3.14159));  // Output: 3
        System.out.println(Math.pow(2, 3));       // Output: 8.0
    }
}
```

---

## 🖥️ Java Program Structure

### Basic Java Program:
```java
public class MyJavaApp {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```

- `public class MyJavaApp`: Declares a class.
- `public static void main(String[] args)`: Entry point of the program.
- Statements end with `;`.

---

## 🔣 Compute and Output

Use `System.out.println()` to output data.

```java
String message = "Java is fun!";
int year = 2025;

System.out.println(message);               // Java is fun!
System.out.println("Year: " + year);       // Year: 2025
```

---

## ⌨️ Input and Assign to Variable

Use the `Scanner` class to read user input.

```java
import java.util.Scanner;

public class ReadInput {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter name: ");
        String name = scanner.nextLine();

        System.out.print("Enter age: ");
        int age = scanner.nextInt();

        System.out.println("Hello " + name + ", age " + age);
        scanner.close();
    }
}
```

---

## 🧮 Java Data Types

| Type     | Description                  | Example              |
|----------|------------------------------|----------------------|
| `byte`   | 8-bit integer                 | `byte b = 100;`      |
| `short`  | 16-bit integer                | `short s = 30000;`   |
| `int`    | 32-bit integer                | `int i = 100000;`    |
| `long`   | 64-bit integer                | `long l = 100000L;`  |
| `float`  | 32-bit decimal                | `float f = 5.75f;`   |
| `double` | 64-bit decimal                | `double d = 19.99;`  |
| `char`   | Single character              | `char c = 'A';`      |
| `boolean`| True or false                 | `boolean b = true;`  |

---

## ➗ Operators

- **Arithmetic**: `+`, `-`, `*`, `/`, `%`
- **Assignment**: `=`
- **Comparison**: `==`, `!=`, `<`, `>`, `<=`, `>=`
- **Logical**: `&&`, `||`, `!`

```java
int a = 10, b = 3;
System.out.println(a + b);      // 13
System.out.println(a > b);      // true
System.out.println(a % b == 1); // true
```

---

## 🔀 Conditional Statements

### `if` Statement
```java
int score = 75;
if (score >= 60) {
    System.out.println("Passed!");
}
```

### `if-else` Statement
```java
int temp = 15;
if (temp > 25) {
    System.out.println("Hot");
} else {
    System.out.println("Not hot");
}
```

---

## 🔁 Loops

### `while` Loop
```java
int count = 0;
while (count < 3) {
    System.out.println("Count: " + count);
    count++;
}
```

### `for` Loop
```java
for (int i = 0; i < 3; i++) {
    System.out.println("Iteration: " + i);
}
```

---

Happy Coding! 🎉
