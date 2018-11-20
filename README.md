# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: USERPASS

package userinput;

import java.util.*;

public class UserPass {

    public static void main (String [] args) {
       
        Scanner sc = new Scanner(System.in);
        System.out.println ("Enter your username: ");
        String username = sc.nextLine();
        
        System.out.println ("Enter your password: ");
        String a = sc.nextLine();
     
        System.out.println ("Confirm you password: ");
        String b = sc.nextLine();
        
        if (a.equals(b)){
            System.out.println ("Correct Password");
        } else { 
            System.out.println ("Invalid Password");
        }
     
    }
}

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: CALCULATOR

public class Calculator {

    public static void main (String [] args) {
     
        Scanner sc = new Scanner(System.in);
        System.out.println ("Enter the first number: ");
        int a = sc.nextInt();
        System.out.println ("Enter the second number: ");
        int b = sc.nextInt();
        
        System.out.println ("What arithmetic operation to be used(add, subtract, multiply, divide, modulo): ");
        String c = sc.next();                
        
        int sum, diff, prod, quo, mod;
        sum = a + b;
        diff = a - b;
        prod = a * b;
        quo = a / b;
        mod = a % b;
        
        if (c.equals("add")){
            System.out.println ( "Sum is: "+ sum);
        } else if (c.equals("subtract")){
            System.out.println ( "Difference is: "+ diff);
        }else if (c.equals("multiply")){
            System.out.println ( "Product is: "+ prod);
        } else if (c.equals("divide")){
             System.out.println ( "Quotient is: "+ quo);
        } else if (c.equals("modulo")){
             System.out.println ( "Modulo is: "+ mod);
        }
    }
}

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: COURSE

import java.util.*;

public class NestedIf {

    public static void main (String [] args){

        Scanner sc = new Scanner (System.in);
        System.out.println("What is your course?");
        String course = sc.nextLine();
        
        if (course.equalsIgnoreCase("BSIT")){
            System.out.println("What is your major?(NetSec, WebTech, ERP)");
            String major = sc.nextLine();
            if (major.equalsIgnoreCase("NetSec")){
                System.out.println("Your course is BSIT-NetSec");
            }
            else if (major.equalsIgnoreCase("WebTech")){
                System.out.println("Your course is BSIT-WebTech");
            }
            else if (major.equalsIgnoreCase("ERP")){
                System.out.println("Your course is BSIT-ERP");
            }
        }
        else if (course.equalsIgnoreCase("BSCS")){
            System.out.println("What is your major?(WebDev, Digital Arts, Animation)");
            String major = sc.nextLine();
            if (major.equalsIgnoreCase("WebDev")){
                System.out.println("Your course is BSCS-WebDev");
            }
            else if (major.equalsIgnoreCase("Digital Arts")){
                System.out.println("Your course is BSCS-Digital Arts");
            }
            else if (major.equalsIgnoreCase("Animation")){
                System.out.println("Your course is BSCS-Animation");
            }
        }
        else if (course.equalsIgnoreCase("BSDA")){
            System.out.println("Your course is BSDA");
        }
        else{
            System.out.println("Invalid");
        }
    }   
}

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: GUESSING GAME

package repetitivestructures;

import java.util.*;

public class GuessingNumber {

    public static void main (String [] args){
    
        Scanner sc = new Scanner (System.in);
        
        System.out.println("Enter a number from 0 - 1000:");
        int a = sc.nextInt(); 
        
        if (a>1000){
            System.out.println("Invalid.");
        }else if (a<0){
            System.out.println("Invalid");
        }else{
        
        
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();                                                                              
        System.out.println();
        System.out.println();  
        System.out.println();                                                                              
        System.out.println();
        System.out.println(); 
        System.out.println();
        System.out.println();    
        
        System.out.println("Guess a number from 0 - 1000:");
        int guess = sc.nextInt();
        
        if (guess>1000){
            System.out.println("Invalid.");
        }else if (guess<0){
            System.out.println("Invalid");
        }else{
            do{
                if (a%2==0){
                System.out.println("Hint:The number is an even number.");
                guess = sc.nextInt();
                }else{
                System.out.println("Hint:The number is an odd number.");
                guess = sc.nextInt();
                }if (guess < a){
                    System.out.println("Hint:The number is higher.");
                    guess = sc.nextInt();
                }else if (guess > a){
                    System.out.println("Hint:The number is lower");
                    guess = sc.nextInt();
                }
            }while (guess!=a);
                System.out.println("You have guessed the correct number.");
               System.out.println("Congratulations!");
            }
        }
    }
}

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: ODD AND EVEN

package userinput;

import java.util.*;


package array;

import java.util.ArrayList;

public class Array {

    public static void main(String[] args) {

        int[] elements  = {3,9,15,20,65,23,18,4,2,14,21};

        System.out.print("Array={");
        for (int i : elements){
        System.out.print( i + " ");
        }
        System.out.println("}");
        
        ArrayList odd  = new ArrayList ();
        ArrayList even  = new ArrayList ();       
        System.out.println("Even\tOdd");
        
        
        for (int i = 0; i<elements.length; i++){
            if (elements [i]%2==0){
                even.add(elements[i]);
            }
            else{
                odd.add(elements[i]);
            }
        }
        
        for (int i = 0; i<elements.length; i++){
            if (i>= even.size() && i < odd.size()){
                System.out.println("\t" + odd.get(i));
            }else if (i>= odd.size() && i < even.size()){
                System.out.println("\t" + even.get(i));
            }else if (i< even.size() && i < odd.size()){
                System.out.println(even.get(i)+ "\t"+odd.get(i));
            }
        }
    } 
}

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: MULTIDIMENTIONAL ARRAY

package array;

import java.util.*;

public class TwoDArrayUserInput {

    public static void main (String [] args ){
    
        Scanner sc = new Scanner (System.in);
        
        System.out.println("Enter number of rows:");
        int row = sc.nextInt();
        
        System.out.println("Enter number of columns:");
        int column = sc.nextInt();
        
        int [][] matrix = new int [row] [column];              
        
        for (int i = 0; i<row; i++){
            for (int j = 0; j<column; j++){
                System.out.println("Enter value for row: " + i + " and column: " + j);
                matrix [i] [j] = sc.nextInt();
            }
        }
        System.out.println("\n"+"Table");
        for (int i = 0; i<row; i++){
               System.out.println("\n" + "Row"+ i +"\t"+ "Column" + i);
            for (int j = 0; j<column; j++){
                System.out.print(matrix [i] [j] + "\t");
            }
        }System.out.println("");
    }
}

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: FIBONACCI

package fibonacci;

import java.util.*;

public class Fibonacci {

    static long num;
    
    public static void main(String[] args) {
        
        input();
        fib (num);
        display();
        //display2();
    }//end of main method
    
    static void input(){
        Scanner hi = new Scanner (System.in);
        System.out.println("Enter a number for fibonacci:");
        num = hi.nextLong();
    }//end of input
    
    static long fib (long num){
        if (num<=1){
            return num;           
        }else{
            return fib(num-1)+fib(num-2);
        }
    }//end of fib
    
    static void display(){
        for (int x = 0; x<= num; x++){
            System.out.print("f("+ x + ")" + "\t" );   
        }System.out.println("");
        
        for (int a = 0; a <= num; a++){
            for (int b = 0; b<=a; b++ ){
            System.out.print(fib(b)+ "\t");
            }
            System.out.println("");
        }
    }//end of display

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: SORTING ALGORITHM

package mergesort;

import java.util.*;

public class MergeSort {

    public static void main(String[] args) {
       

        //Unsorted array
        Integer[] a = { 2, 6, 3, 5, 1 };
         
        //Call merge sort
        mergeSort(a);
         
        //Check the output which is sorted array
        System.out.println(Arrays.toString(a));
    }
 
    @SuppressWarnings("rawtypes")
    public static Comparable[] mergeSort(Comparable[] list)
    {
        //If list is empty; no need to do anything
        if (list.length <= 1) {
            return list;
        }
         
        //Split the array in half in two parts
        Comparable[] first = new Comparable[list.length / 2];
        Comparable[] second = new Comparable[list.length - first.length];
        System.arraycopy(list, 0, first, 0, first.length);
        System.arraycopy(list, first.length, second, 0, second.length);
         
        //Sort each half recursively
        mergeSort(first);
        mergeSort(second);
         
        //Merge both halves together, overwriting to original array
        merge(first, second, list);
        return list;
    }
     
    @SuppressWarnings({ "rawtypes", "unchecked" })
    private static void merge(Comparable[] first, Comparable[] second, Comparable[] result)
    {
        //Index Position in first array - starting with first element
        int iFirst = 0;
         
        //Index Position in second array - starting with first element
        int iSecond = 0;
         
        //Index Position in merged array - starting with first position
        int iMerged = 0;
         
        //Compare elements at iFirst and iSecond,
        //and move smaller element at iMerged
        while (iFirst < first.length && iSecond < second.length)
        {
            if (first[iFirst].compareTo(second[iSecond]) < 0)
            {
                result[iMerged] = first[iFirst];
                iFirst++;
            }
            else
            {
                result[iMerged] = second[iSecond];
                iSecond++;
            }
            iMerged++;
        }
        //copy remaining elements from both halves - each half will have already sorted elements
        System.arraycopy(first, iFirst, result, iMerged, first.length - iFirst);
        System.arraycopy(second, iSecond, result, iMerged, second.length - iSecond);
    }
}

# CC2-projects

1-H, Tamayo, Dynah M.

TITLE: FACTORIAL OR FIBONACCI ARRAY

package factorialfibonacci;

import java.util.*;

public class FactFib {
        
        static int i;
        static int x[];
        public static void main(String[] args) {
        
        Scanner hi = new Scanner (System.in);
        System.out.println("What do you want to get? Factorial or Fibonacci?");
        String a = hi.nextLine();
        
        System.out.println("Enter the size of array:");
        int b = hi.nextInt();
        
        int [] x = new int [b];
                
        System.out.println("Enter elements:");
        for (int i=0; i<b; i++){
            System.out.print("index " + i + ": ");
            x [i] = hi.nextInt();    
        }System.out.println("  ");
        

        if (a.equalsIgnoreCase("factorial")){
           display1 (x);

        }else if (a.equalsIgnoreCase("fibonacci")){
            display2 (x);
        }
        }//end of main class
        
        static void display1 (int [] x){
            for (int i = 0; i<x.length; i++){
                System.out.print ("f (" + x[i] + ")" + "\t");  
            }System.out.println("");
            for (int i = 0; i<x.length; i++){
                System.out.print(fact(x[i]) + "\t");
            }System.out.println("");
        }//end of 1
        
        static void display2 (int [] x){
             for (int i = 0; i<x.length; i++){
                System.out.print ("f (" + x[i] + ")" + "\t");  
              
            }System.out.println("");
            for (int i = 0; i<x.length; i++){
                System.out.print(fib(x[i]) + "\t");
            }System.out.println("");
        }//end of 2
        
        static int fact(int i) {
        if (i<=1){
            return 1;
        }else{
            return i*fact(i-1);
        }
        }//end of fact
    
        static int fib (int i){
        if (i<=1){
            return i;           
        }else{
            return fib(i-1)+fib(i-2);
        }
        }//end of fib
        
}
