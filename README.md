# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:

```
#include <stdio.h>

int main() {
    int M, N;

    
    printf("Enter the value of M: ");
    scanf("%d", &M);

    printf("Enter the value of N: ");
    scanf("%d", &N);

    printf("Even numbers from %d to %d are:\n", M, N);

    
    if (M % 2 != 0) {
        M++; 
    }

  
    for (int i = M; i <= N; i += 2) {
        printf("%d ", i);
    }

    printf("\n");

    return 0;

}
```

## OUTPUT:

![WhatsApp Image 2025-04-30 at 19 59 24_152c927c](https://github.com/user-attachments/assets/b555aacf-b33f-4574-bf12-d4dd5c97c2f1)










## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int i, j, rows;

   
    printf("Enter the number of rows: ");
    scanf("%d", &rows);

   
    for (i = 1; i <= rows; i++) {
        
        for (j = 1; j <= i; j++) {
            printf("*");
        }
        
        printf("\n");
    }

    return 0;
}
```


## OUTPUT:
![WhatsApp Image 2025-04-30 at 19 59 23_48a0f73c](https://github.com/user-attachments/assets/4e449a47-428d-48bd-89fb-911d06b32825)






## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>


void add(int a, int b);
void subtract(int a, int b);

int main() {
    int num1, num2;

    
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);

    
    add(num1, num2);
    subtract(num1, num2);

    return 0;
}


void add(int a, int b) {
    int result = a + b;
    printf("Addition = %d\n", result);
}


void subtract(int a, int b) {
    int result = a - b;
    printf("Subtraction = %d\n", result);
}
```


## OUTPUT:
![WhatsApp Image 2025-04-30 at 20 02 52_2a7015ff](https://github.com/user-attachments/assets/6cc2d36e-fcfa-42f3-95c1-67a45311e183)







## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int number, digit, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &number);

    
    for (int temp = number; temp > 0; temp /= 10) {
        digit = temp % 10;
        if (digit % 2 != 0) { 
            sum += digit;
        }
    }

    printf("Sum of odd digits = %d\n", sum);

    return 0;
}
```


## OUTPUT:
![WhatsApp Image 2025-04-30 at 20 06 24_e181639e](https://github.com/user-attachments/assets/526a2a3d-fe6f-47d8-93fa-2180dbac6577)





## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.

## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>


void factorial(int n);

int main() {
    int num;

   
    printf("Enter a positive integer: ");
    scanf("%d", &num);

    
    if (num < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        factorial(num);
    }

    return 0;
}


void factorial(int n) {
    int i;
    unsigned long long fact = 1;

    for (i = 1; i <= n; i++) {
        fact *= i;
    }

    printf("Factorial of %d is %llu\n", n, fact);
}
```


## OUTPUT:
![WhatsApp Image 2025-04-30 at 20 10 57_6ccc63e0](https://github.com/user-attachments/assets/d0141889-d717-4803-b704-db89fca0b6cb)






## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
