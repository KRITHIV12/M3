# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
#include <stdio.h>
#include <math.h>
void calculate_emi(float principal, float rate_of_interest, int months) {
float r = rate_of_interest / (12 * 100);
int t = months;
float emi = (principal * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
printf("The EMI for the loan is: %.2f\n", emi);
}
int main() 
{
    float principal, rate_of_interest;
    int months;

    printf("Enter the principal amount: ");
    scanf("%f", &principal);
    
    printf("Enter the annual rate of interest (in %%): ");
    scanf("%f", &rate_of_interest);
    
    printf("Enter the number of months: ");
    scanf("%d", &months);

    calculate_emi(principal, rate_of_interest, months);

    return 0;
}


## OUTPUT
![Screenshot 2025-05-06 161737](https://github.com/user-attachments/assets/79330c11-bb79-4e93-b011-cf866b5a4354)


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
#include <stdio.h>

void generateFibonacci(int n) {
int first = 0, second = 1, next, i;
for(i = 1; i <= n; i++) {
printf("%d ", first);
next = first + second;
first = second;
second = next;
}
}
int main() {
int terms = 6;
generateFibonacci(terms);
return 0;
}

## OUTPUT
![Screenshot 2025-05-06 161847](https://github.com/user-attachments/assets/9a5f2959-ad19-4581-9284-a5d934a7ef53)

## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
#include <stdio.h>

int main() {
int n, i;
scanf("%d", &n);
int arr[n]; 
for(i = 0; i < n; i++) {
scanf("%d", &arr[i]);
}
printf("Last element = %d\n", arr[n-1]);
return 0;
}

## OUTPUT
n : 5
i:10 20 30 40 50
Last element = 50

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
#include <stdio.h>

int main() {
int n, i, count = 0;
scanf("%d", &n);
int arr[n];
for(i = 0; i < n; i++) {
scanf("%d", &arr[i]);
}
for(i = 0; i < n; i++) {
if(arr[i] > 0) {
count++;
}
}
printf("Total number of positive elements = %d\n", count);
return 0;
}

## OUTPUT
n: 1 -2 3 0 4
Total number of positive elements = 3


## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
#include <stdio.h>

int main() {
int n, i;
scanf("%d", &n);
int arr[n];
char updated[n]; 
for(i = 0; i < n; i++) {
scanf("%d", &arr[i]);
if(arr[i] % 2 == 0) {
updated[i] = 'E';
} else {
updated[i] = arr[i] + '0';
}
}
for(i = 0; i < n; i++) {
printf("%c ", updated[i]);
}
printf("\n");
return 0;
}

## Output:
n:1 2 3 4 5
Updated array:
1 E 3 E 5

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



