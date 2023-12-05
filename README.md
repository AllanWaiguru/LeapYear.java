# LeapYear.java
import java.util.Scanner;

public class LeapYearChecker {
    public static void main(String[] args) {
        checkLeapYear();
    }

    public static void checkLeapYear() {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter the year: ");
        int year = input.nextInt();

        if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0) {
            System.out.println("The year you entered is a leap year");
        } else {
            System.out.println("The year you entered is not a leap year");
        }
    }
}
