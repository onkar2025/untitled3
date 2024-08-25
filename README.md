# untitled3
Mini Project for guessing numbers
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        //Mini Project
        Scanner sc = new Scanner(System.in);
        int myNumber = (int)(Math.random()*100);
        int userNumber = 0;
        do {
            System.out.println("Guess my Number(1-50): ");
            userNumber = sc.nextInt();

            if(userNumber == myNumber) {
                System.out.println("Wohoo ...Correct number");
                break;
            }
            else if (userNumber > myNumber) {
                System.out.println("Your number is too large");

            }
            else {
                System.out.println("Your number is too small");
            }
        } while(userNumber >= 0);

        System.out.println("My number was ");
        System.out.println(myNumber);
    }
}

