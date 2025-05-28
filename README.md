# Simple Calculator 🧮

This is an easy Java console-based application. In this, we can perform different operations on two numbers such as:

- ➕ Addition
- ➖ Subtraction
- ✖ Multiplication
- ➗ Division

---

## 🖥 Language
- Java (.java)

---

## 📁 Files
- Calculator.java

---

## 🚀 How to Use
1. Run javac Calculator.java
2. Make sure Java is already installed.
3. Enter two numbers.
4. Select the operation.
5. Your answer will be shown on the screen.

---

## 👨‍💻 Developer
*Rohit Patil*

The main purpose of this Java project is to learn Java and upload the project on GitHub.

---

## 💡 Sample Code

```java
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter First number: ");
        double num1 = sc.nextDouble();

        System.out.print("Enter Second number: ");
        double num2 = sc.nextDouble();

        System.out.println("1: Addition (+)");
        System.out.println("2: Subtraction (-)");
        System.out.println("3: Multiplication (*)");
        System.out.println("4: Division (/)");
        System.out.print("Choose Your operation: ");
        int choice = sc.nextInt();

        double result = 0;

        switch (choice) {
            case 1:
                result = num1 + num2;
                break;
            case 2:
                result = num1 - num2;
                break;
            case 3:
                result = num1 * num2;
                break;
            case 4:
                if (num2 != 0)
                    result = num1 / num2;
                else {
                    System.out.println("Cannot divide by zero!");
                    return;
                }
                break;
            default:
                System.out.println("Invalid choice!");
                return;
        }

        System.out.println("Result: " + result);
    }
}
