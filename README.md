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





1.	Explain the differences between primitive and reference data types. 
•	Primitive 
These are basic types of data built into a language, such as int and chr
•	Reference 
These are creatable classes as well as arrays, the show an object and store the address of the object stored in the memory.
2.	Define the scope of a variable (hint: local and global variable)
•	The scope is a part of the program where the variable is available.
•	Local variable is a method inside that is declared and can only be used within the method
•	Global variable it declared outside any method and is accessed by all parts of the class

3.	Why is initialization of variables required. 
Initialization is required because it assigns an initial value to a variable without it, it can lead to unpredictable behavior.

4.	Differentiate between static, instance and local variables. 
•	Static is shared among all instance of a class and belong to the class itself.
•	Instance is non static and each instance of class has its own copy of the variables
•	Local is declared within a method and are not accessible outside

5.	Differentiate between widening and narrowing casting in java. 
Widening is converting a smaller type to a large type size while narrowing requires explicating conversion and it’s converting a larger type to small type size.

6.	The following table shows data type, its size, default value and the range. Filling in the missing values.

Type	Size	Default 	Range
Boolean	1 bit	False	True/false
Char	2 	‘\u0000	‘\0000` to \ffff
Byte	1	0	-128 to 127
Short	2	0	-215  to +215 -1
Int	4 	0	-2^31 to 2^31-1
Long	8 	0l	-2^63 to 2^63-1
Float	4	00.bf	~1.4E-45 to ~3.4E+38
Double	8	0.0D	-1.8E +308 to +1.8E +308


7.	Define class as used in OOP
In oop a class is a blueprint for creating objects it defines a data type by bundling data into a single unit. The class also specifies the data attribute and behaviors that the object created from the class have.

8.	Explain the importance of classes in Java programming.
•	Reusability: when a class is written it can be used to create multiple objects saving on time
•	Modularity: classes allow the programmers to breakdown complex problems into smaller pieces. Making the code more organized.
•	Inheritance: this mechanism helps new classes to inherit properties and methods from an existing class. Aids in code reusability 
•	Polymorphism: through classes java can allow methods to perform differently based on the object that invoke it.


