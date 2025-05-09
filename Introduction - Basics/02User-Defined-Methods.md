# User-Defined Methods in Java

## Introduction

Learn how to make your own methods.

Built-in methods are like ready-to-cook recipes, but Java also allows us to create customized methods for our specific needs. For example, there's no built-in method like `buildYouTubeForMe("please")`, so we must define our own.

## Why Make User-Defined Methods?

User-defined methods help create **modular** and **reusable** code. They can be used to perform tasks such as displaying a message, generating random numbers, or executing other predefined routines.

## What are User-Defined Methods?

Here’s the basic structure of a user-defined method:

```java
public static ReturnType methodName(ParameterList) {
    // method body
}
```

This structure is similar to the main method, but the name, parameters, and return type are defined by the programmer.

### Important Notes:
- The Java Virtual Machine always starts execution from the `main` method.
- User-defined methods must be **called** from the main method to be executed.

## Conceptual Understanding

### Example: Order a Pizza

```java
public static String orderPizza(String pizzaType, String extraTopping) {
    return pizzaType + " Pizza with " + extraTopping;
}

public static void main(String[] args) {
    String pizza1 = orderPizza("Margherita", "Olives");
    String pizza2 = orderPizza("Pepperoni", "Extra Cheese");
    System.out.println(pizza1);
    System.out.println(pizza2);
}
```

- **Line 2–4:** Defines the method `orderPizza`.
- **Line 8 & 11:** Calls the method with different arguments to get different outputs.

### Example: Add Two Numbers

```java
public static int addNumbers(int num1, int num2) {
    return num1 + num2;
}

public static void main(String[] args) {
    int result = addNumbers(5, 10);
    System.out.println(result);
}
```

> If you don’t print the result, you won’t see the output. Always remember to call and print if needed!

## Improving Readability with Methods

### Without Methods

```java
System.out.println("What is 2 + 3?");
System.out.println("Expected: 5");
System.out.println("Actual: " + (2 + 3));
```

- This kind of code is repetitive and prone to errors.

### With Methods

```java
public static void askQuestion(String question, int expected, int actual) {
    System.out.println(question);
    System.out.println("Expected: " + expected);
    System.out.println("Actual: " + actual);
}

public static void main(String[] args) {
    askQuestion("What is 2 + 3?", 5, 2 + 3);
    askQuestion("What is 7 - 4?", 3, 7 - 4);
}
```

- Cleaner, modular, and easier to debug.

## Review

- **User-defined methods** promote **modularity**, **reusability**, and **clarity**.
- Always define methods with the correct format and call them from `main()`.
- Use methods to avoid code repetition and enhance maintainability.
