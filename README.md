
// import static org.junit.jupiter.api.Assertions.assertEquals;
import java.util.Scanner;
// import org.junit.jupiter.api.Test;

public class Main {
  public static void main(String[] args) {
    System.out.println(
        "Hello, welcome to the Math Game! Answer the questions asked and you will be rewarded with points. Good luck!");
    Scanner scanner = new Scanner(System.in);
    int num1;
    int num2;
    int points = 0;
    int numCorrect = 0;
    int numDone = 0;
    int level = 2;
    String achieve = "Achievements Unlocked: None";
    while (true) {

      if(level == 2) 
        achieve = "Achievements Unlocked: I've begun";
      if(level == 3) 
        achieve = "Achievements Unlocked: I've begun, I'm getting there";
      if(level == 100)
        achieve = "Achievements Unlocked: I've begun, I'm getting there, I'm da pro";
      if(level == 1000)
        achieve = "Achievements Unlocked: I've begun, I'm getting there, I'm da pro, NASA Computer Detected";
      
      int num = 0;
      num1 = (int) (Math.random() * 100 + 1);
      num2 = (int) (Math.random() * 100 + 1);
      System.out.println("You are on level " + level);
      System.out.println(achieve);
      System.out.println("Total points: " + points);
      System.out.println("Number of correct answers: " + numCorrect+ "/" + numDone);
      numDone++;
      System.out.println("What is " + num1 + " + " + num2 + "?");
      double answer = scanner.nextInt();
      if (answer == num1 + num2) {
        System.out.println("Correct! Good job!" + "\n");
        points += 5;
        numCorrect++;
        num++;
      } else
        System.out.println("Incorrect. The correct answer is " + (num1 + num2) + "\n");

      num1 = (int) (Math.random() * 100 + 1);
      num2 = (int) (Math.random() * 100 + 1);
      numDone++;
      System.out.println("What is " + num1 + " - " + num2 + "?");
      answer = scanner.nextInt();
      if (answer == num1 - num2) {
        System.out.println("Correct! Good job!" + "\n");
        points += 5;
        numCorrect++;
        num++;
      } else
        System.out.println("Incorrect. The correct answer is " + (num1 - num2) + "\n");

      num1 = (int) (Math.random() * 100 + 1);
      num2 = (int) (Math.random() * 100 + 1);
      numDone++;
      System.out.println("What is " + num1 + " * " + num2 + "?");
      answer = scanner.nextInt();
      if (answer == num1 * num2) {
        System.out.println("Correct! Good job!" + "\n");
        points += 5;
        numCorrect++;
        num++;
      } else
        System.out.println("Incorrect. The correct answer is " + (num1 * num2) + "\n");

      num1 = (int) (Math.random() * 100 + 1);
      num2 = (int) (Math.random() * 100 + 1);
      numDone++;
      System.out.println("What is " + num1 + " / " + num2 + " rounded to the whole number?");
      answer = scanner.nextInt();
      if (answer == num1 / num2) {
        System.out.println("Correct! Good job!" + "\n");
        points += 5;
        numCorrect++;
        num++;
      } else
        System.out.println("Incorrect. The correct answer is " + (num1 / num2) + "\n");

      if(num == 4)
        level++;
      
     
    }
  }
}
