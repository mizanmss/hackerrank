
Grade Syatem option :1
implement JAVA

public class Solution {
   public static void main(String[] args) {
       Scanner in = new Scanner(System.in);
       int n = in.nextInt();
       for(int i=0; i < n; i++){
           int grade = in.nextInt();
           System.out.println(grade < 38 || grade % 5 < 3 ? grade : grade + (5 - (grade % 5)));
       }
   }
}





Grade Syatem option :2 
implement JAVA

import java.util.Scanner;

public class GradingStudents {
   
   public static void main(String[] args) {
       Scanner scan = new Scanner(System.in);
       int n = scan.nextInt();
       while (n-- > 0) {
           int grade = scan.nextInt();
           System.out.println(calculateGrade(grade));
       }
   }
   
   private static int calculateGrade(int grade) {
       if (grade >= 38) {
           int newgrade = grade % 5;
           if (newgrade > 2) {
               grade =grade + 5 - newgrade;
           }
       }
       return grade;
   }
}
