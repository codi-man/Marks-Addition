package com.company;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner kb = new Scanner(System.in);
        System.out.print("How many Subject do you have?: ");
        int subjects_range;
        subjects_range = kb.nextInt();

        int i = 0;
        int sum = 0;
        while (i<=subjects_range) {

            for (i=1;i<=subjects_range;i++) {
                System.out.print("Enter Marks of Subject #" + i + ": ");
                int subject_marks;
                subject_marks = kb.nextInt();
                sum+=subject_marks;
            }
        }
        System.out.println("Sum of your result is: "+sum);
    }
}