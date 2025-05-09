# Recovering from Errors in Java

## Introduction
In this lesson, we explore common types of programming errors (bugs) and how to handle or prevent them effectively.

## 🐞 Bugs: What Are They?
Bugs are unintended flaws in code and its functionality. They typically fall into two categories:

### Syntax Errors
- Occur when the code violates Java's syntax rules.
- Prevent the program from compiling or running.
- **Example:** Misplaced quotation marks or missing parentheses.

### Logical Errors
- Do not prevent the code from compiling or running.
- Result in incorrect output or behavior.
- **Example:** Using the wrong formula for a calculation.

## 🔍 Common Error Scenarios

### 1. Syntax Mistake Example
Incorrect use of syntax like missing or misplaced punctuation causes compilation errors.

**Bug Example:**  
```java
System.out.println("Hello World); // Missing closing quote
```

### 2. Logical Error Example
Code compiles and runs, but output is wrong due to logic mistake.

**Bug Example:**  
```java
int area = length + width; // Should be length * width
```

### 3. Scope-Related Errors
Incorrect placement of `{}` can cause issues.

**Bug Example:**  
```java
public static int calculateRectangleArea(int l, int w)
{
}
return area; // Error: Return placed outside method block
```

### 4. Incorrect Execution Order
Code should follow logical execution steps.

**Bug Example:**  
```java
System.out.println(fullName); // Displayed before being updated
fullName = "John Doe";
```

### 5. Parameter Order Mismatch
Parameters and arguments must align in number and order.

**Bug Example:**  
```java
printQuestion(10, 2, "*"); // Correct: (int x, int y, String op)
printQuestion(10, "*", 2); // Error: Mismatched types
```

### 6. Wrong Number of Parameters
Providing too few or too many arguments causes errors.

**Bug Example:**  
```java
calculateSum(2, 3, 4); // Correct
calculateSum(2, 3);    // Error: Too few arguments
```

## ✅ Summary
- Always validate syntax to prevent compiler errors.
- Carefully review logic to ensure correct output.
- Respect method signatures: order and number of parameters matter.
- Fixing and learning from bugs is a vital part of the development process.

> "To err is human, to debug is divine."

---
