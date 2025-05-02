# EX-11-FUNCTIONS

## AIM

To write a Program to convert a given decimal value to binary using function with arguments without return type.

## ALGORITHM

1.	Start
2.	Define a function decimalToBinary(int number):
   .	Initialize an array to store binary digits.
   .	If the number is 0, print 0 and return.
   .	Use a loop to:
   .	Divide the number by 2.
   . Store the remainder in an array.
	  . Update the number as the quotient.
	  . After the loop ends, print the array in reverse to show the binary number.
   	In main():
3.	Prompt the user to input a decimal number.
   .	Call the function decimalToBinary() with the input number.
4.	End



## PROGRAM

```
#include <stdio.h>
void convert(int n);
int main()
{
    int n;
    scanf("%d",&n);
    convert(n);
    return 0;
}
void convert(int n)
{
    int a=0,f=1;
    int n1=n;
    while(n!=0)
    {
        a+=(n%2)*f;
        f=f*10;
        n=n/2;
    }
    printf("%d in decimal = %d in binary",n1,a);
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/b367a06a-58df-4430-a816-72cc0f316d68)




## RESULT

Thus the  Program to convert a given decimal value to binary using function with arguments without return types has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start
2.	Initialize three integers:
   . first = 0
  	. second = 1
  	. next (to hold the sum)
3.  Loop from 1 to 11:

Print the current value of first
   . Compute next = first + second
   . Update first = second
   . Update second = next

4. End the loop after 11 iterations
5. End

## PROGRAM
```
#include <stdio.h>

int main() {
    int n = 11; 
    int first = 0, second = 1, next;

 

    for (int i = 0; i < n; i++) {
        if (i <= 1)
            next = i; 
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }

    printf("\n");
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/c602c4e3-d018-433d-90ea-3a8e3454d824)







## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-MATRIX-IN-REVERSE-ORDER

## AIM
To Write  a C program to read the elements of the n x n matrix and print the elements of the matrix in the reverse order

## ALGORITHM
1.	Start
2.	Input value n for the size of the matrix.
3.	Declare a 2D array matrix[n][n].
4.	Use nested loops to read n x n elements:
   .	For i from 0 to n-1
  	. For j from 0 to n-1
   . Read matrix[i][j]
5. Use nested loops to print matrix in reverse order:
   . For i from n-1 down to 0
   . For j from n-1 down to 0
   . Print matrix[i][j]
6. End

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);

    int a[n][n];
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            scanf("%d", &a[i][j]);
        }
    }
    for (int i = n - 1; i >= 0; i--) {
        for (int j = n - 1; j >= 0; j--) {
            printf("a[%d][%d] is %d\n", i, j, a[i][j]);
        }
    }

    return 0;
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/d849cf2f-c9e2-44f8-9d52-fbaf13bdeaed)







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


## OUTPUT





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

## Output:
 


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



