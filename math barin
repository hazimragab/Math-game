// import static org.junit.jupiter.api.Assertions.assertEquals;
import java.util.Scanner;
// import org.junit.jupiter.api.Test;

public class Main {
  public static void main(String[] args) {
    System.out.println("Hello, welcome to the Math Game! Answer the questions asked and you will be rewarded with points. Good luck!");
    Scanner scanner = new Scanner(System.in);
    int num1;
    int num2;
    int points = 0;
    while(true) {
     num1 = (int) (Math.random() * 100 +1);
     num2 = (int) (Math.random() * 100 +1);
    System.out.println("Total points: " + points);
    System.out.println("What is " + num1 + " + " + num2 + "?");
    int answer = scanner.nextInt();
    if(answer == num1 + num2) {
      System.out.println("Correct! Good job!");
      points += 5;
    }
    else
      System.out.println("Incorrect. The correct answer is " + (num1 + num2));
       num1 = (int) (Math.random() * 100 +1);
       num2 = (int) (Math.random() * 100 +1);
      System.out.println("What is " + num1 + " - " + num2 + "?");
       answer = scanner.nextInt();
      if(answer == num1 - num2) {
        System.out.println("Correct! Good job!"  + "\n"); 
        points += 5;
      }
      else
        System.out.println("Incorrect. The correct answer is " + (num1 + num2) + "\n");
    }
  }
}
