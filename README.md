import java.util.Scanner;

// code to promt student to enter marks for five units 

public class Averagemarks{
public static void public static void main(String[] args) {
	Scanner scanner = new Scanner(System.in);

	// variable initialization
	double totalMarks = 0.0;
	int numUnits = 5;

	 // get marks for each unit
	for (int i = 1;i <= numUnits; i++ ) {
		System.out.print("input marks for units"+ i +":");

		double marks = scanner.nextDouble();
		totalMarks += marks;

	}
	 // get the calculation of average
	double average = totalMarks / numUnits;

	 	// output average 
	System.out.printf("Average marks: %.2f%n", average);

Scanner.close();
}

}

import java.util.Scanner;

// divisibility check
public class Checkingfordivisiblenumbers{
	public static void main(String[]args){
		Scanner scanner = new Scanner(System.in);

		// input integer
		System.out.print("enter an integer:");
			int number = scanner.nextInt();

		// divisibility check for 0 to 9
			for (int divisor = 1; divisor <= 9; divisor ++){
				if (number % 10 == 0){

					System.out.printIn("Number is divisible by " + divisor +" cause it ends with 0.");
}else if (number% divisor == 0){
	System.out.printIn("number is divisible by"+ divisor + " because it ends with a " + (number % 10) + ".");
}

			}
			scanner.close();	
	}
}


// CODE TO DISPLAY MULTIPLES
 
 public class FindMultiples {
 	public static void main(String[]args){

 		int start = 71;
 		int end = 150;

 		//output multiples
 		System.out.println("Multiples of 2, 3 and 7 within the range"+ start + "to " + end +":");
 	for (int i = start; i <= end; i++){
 		if (i% 2 == 0 || i % 3 == 0 || i % 7 == 0){
 			System.out.print(i =" ");
 		}
 	}

 	}

 }


 // creating a calculator

import java.util.Scanner;
public static void main(String[]args){
	Scanner scanner = new	Scanner(System.in);

	// input first value
	System.out.print(" Input first number: ");
	double num1 = scanner.nextDouble();

	// input operation (+,-,*,/)
		System.out.print("input operation (+,-,*,/):");
			char operation = scanner.next().charAt(0);

			// input second value
        System.out.print("Input second number: ");
        double num2 = scanner.nextDouble();
        	 double result;

    // Perform the following operation
        switch (operation) {
            case '+':
                result = num1 + num2;
                break;
            case '-':
                result = num1 - num2;
                break;
            case '*':
                result = num1 * num2;
                break;
            case '/':
                if (num2 != 0) {
                    result = num1 / num2;
                } else {
                    System.out.println("Error: Division by zero!");

                    return;
                }
          break;
            default:
                System.out.println("Invalid operation. Please choose +, -, *, or /.");
                return;
        }

        System.out.println("Result: " + result);

        scanner.close();
    }

}
