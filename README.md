# Calculator
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Inserisci il primo numero: ");
        double num1 = scanner.nextDouble();
        System.out.println("Inserisci il secondo numero: ");
        double num2 = scanner.nextDouble();

        System.out.println("Scegli un'operazione (+, -, *, /): ");
        char operator = scanner.next().charAt(0);

        double result;
        switch (operator) {
            case '+':
                result = num1 + num2;
                break;
            case '-':
                result = num1 - num2;
                break;
            case '*':
                result = num1 * num2;
                break;
            case '/':
                result = num1 / num2;
                break;
            default:
                System.out.println("Operazione non valida");
                return;
        }

        System.out.println("Risultato: " + result);
    }
}
