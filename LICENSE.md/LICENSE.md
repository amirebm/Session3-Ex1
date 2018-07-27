//برنامه ایی بنویسید که عددی از ورودی گرفنه و بررسی نماید اول است یا خیر؟

package com.personal.Ex1;

import java.util.Scanner;

public class Ex1 {

	public static void main(String[] args) {
		
		Scanner sc= new Scanner(System.in);
		System.out.println("Enter a Number");
		int prime= sc.nextInt();
		if(PrimeFinder(prime))
			{System.out.println(prime + " is a prime number");}
		else
			System.out.println(prime + " is not a prime number");
			}
		
	
	
	static boolean PrimeFinder(int prime) {
		
		double root= Math.sqrt(prime);
		for (int i = 2; i <= root; i++) {
			
			if(prime %i==0) {
				return false;}
			
			}
		return true;
		
	}

}
