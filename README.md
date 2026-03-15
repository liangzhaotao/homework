import java.util.Scanner;
public class homework {
    public static void MassIndex(double weight, double height) {
        double bmi = weight / (height * height);
        if (bmi < 18.5) {
            System.out.println("Underweight: less than 18.5");
        } else if (bmi >= 18.5 && bmi <= 24.9) {
            System.out.println("Normal: between 18.5 and 24.9");
        } else if (bmi >= 25 && bmi <= 29.9) {
            System.out.println("Overweight: between 25 and 29.9");
        } else {
            System.out.println("Obesity: 30 or greater");
        }
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("请输入体重 (kg): ");
        double weight = scanner.nextDouble();
        System.out.print("请输入身高 (m): ");
        double height = scanner.nextDouble();
        homework.MassIndex(weight, height);
        scanner.close();
    }
}
