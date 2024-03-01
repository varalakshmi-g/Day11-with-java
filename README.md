# Day11-with-java

Today's  task is to Write a program that counts the occurrences of an element in an array.

Here comes the program :

import java.util.Scanner;

public class Main {
 public static void main(String[] args) {
 Scanner sc = new Scanner(System.in);
 int n;
 System.out.println("Enter the total number of elements: ");
 n = sc.nextInt(); 

 int arr[] = new int[n];
 System.out.println("Enter the elements of the array: ");
 for (int i = 0; i < n; i++) {
 arr[i] = sc.nextInt(); 
 }

 System.out.println("Enter the element whose frequency you want to know: ");
 int element = sc.nextInt();
 int occ = 0; 

 
 for (int i = 0; i < n; i++) {
 if (element == arr[i]) {
 occ++;
 }
 }

 System.out.println(element + " occurred " + occ + " times.");
 }
}

