
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




Diagonal Defference 
Implement in C

int main(){
    int n;
    int i=0,sum=0,j,sum2=0;
    scanf("%d",&n);
    int a[n][n];
    for(int a_i = 0; a_i < n; a_i++){
       for(int a_j = 0; a_j < n; a_j++){
         
          scanf("%d",&a[a_i][a_j]);
       }
    }
 while(i<n)
 {
  sum=sum+a[i][i];
  i++;
 }
    j=n-1,i=0;
 while(i<n)
 {
  sum2=sum2+a[i][j];
  i++;
        j--;
 }
    printf("%d",abs(sum-sum2));
    return 0;
}


Simple Array Sum 
Implement in C

#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a[1000],n,i,sum=0;
    scanf("%d",&n);
    for(i=0;i<n;i++)
        {
        scanf("%d",&a[i]);
        sum+=a[i];
    }
    printf("%d",sum);
    return 0;
}
