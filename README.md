import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter First Number: ");
        double num1 = sc.nextDouble();

        System.out.print("Enter Second Number: ");
        double num2 = sc.nextDouble();

        System.out.println("1: Addition (+)");
        System.out.println("2: Substraction (-)");
        System.out.println("3: Multiplication (*)");
        System.out.println("4: Division (/)");
        System.out.print("Choose Your Type : ");
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
                result = num1 / num2;
                break;
            default:
                System.out.println("Wrong Type Choosen!");
                return;
        }

        System.out.println("Answer: " + result);
    }
}
