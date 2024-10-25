# Fibonacci-Sequence
//Program to print Fibonacci Sequence of n terms where n is a input by user


//code in java..........

import java.util.*;

public class Main
{
    public static void main(String[] args){
    
        Scanner sc=new Scanner(System.in);
        
        System.out.println("Enter the number of terms of fibonacci sequence:");
        
        int n=sc.nextInt();//taking input from user
        
        if (n<0){
            System.out.println("Enter the positive integer number.");
        }
        else {
            System.out.println("fibonacci series."+" ");

            
            int first=0;           //initial number fixed  
            int second=1;           //second number fixed
            
            for(int i=1;i<=n;i++){
                System.out.print(first+" ");
                int next=first+second;
                first=second;
                second=next;
            }
        }
        sc.close();
    }
}
