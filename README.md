# EX-11-FUNCTIONS

## AIM

write a Program to convert a given decimal value to binary using function with arguments with return type.


## ALGORITHM

```
1.Start
2.Input a decimal number (decimal) from the user.
3.Initialize an array binary[32] to store binary digits.
4.Store the original decimal number in another variable for later display
(original = decimal).
5.Set index i = 0 to track the position in the binary array.
6.Repeat while decimal > 0:
a. Compute remainder = decimal % 2.
b. Store the remainder in binary[i].
c. Update decimal = decimal / 2 (integer division).
d. Increment i by 1.
7.Print the original decimal number.
8.Print binary digits stored in the array in reverse order (from i-1 to 0).
9.End
```

## PROGRAM

```
#include <stdio.h>
void decimalToBinary(int n)
{
    int binary[32],decimal;
    int i=0;
    decimal=n;
    
    while(n>0)
    {
        binary[i]=n%2;
        n=n/2;
        i++;
    }
    printf("%d in decimal = ",decimal);
    for(int j=i-1;j>=0;j--)
    {
        printf("%d",binary[j]);
    }
    printf(" in binary\n");
}
int main()
{
    int decimal;
    scanf("%d",&decimal);
    decimalToBinary(decimal);
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/44f5f2cf-ac0e-4d5d-8df7-8a8d94c7286f)


## RESULT

Thus the Program to convert a given decimal value to binary using function with arguments with return type has been executed successfully.



# EX-12-FIBONACCI-SERIES

## AIM

Create a C program to generate the Fibonacci series for the value 13

## ALGORITHM

```
1. Start the program.
2. Read number of terms to display.
3. Add the previous two terms and store it in new term.
4. Assign 2nd term to 1st term and 3rd term to 2nd term.
5. Repeat steps 3 and 4 n number of times.
6. Display the result.
7. Stop the program.
```

## PROGRAM

```
#include <stdio.h>

void generateFibonacci(int n) {
    int a = 0, b = 1, next;
    printf("%d %d ", a, b);
    for (int i = 2; i < n; i++) {
        next = a + b;
        printf("%d ", next);
        a = b;
        b = next;
    }
    printf("\n");
}

int main() {
    int n = 13;
    generateFibonacci(n);
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/495e3229-a21c-4ce3-9b3a-027c4996a969)


## RESULT

Thus the program to generate the Fibonacci series for the value 13 has been executed successfully.


# EX-13-ARRAY

## AIM

Write a program in C to read n number of values in an array and display it in reverse
order

## ALGORITHM

```
1. Start
2.Input the size of the array n.
3.Declare an integer array a[n].
4.Repeat for i from 0 to n-1:
a. Input a[i] (i.e., read each element into the array).
5.Repeat for i from n-1 down to 0:
a. Print a[i] (i.e., print the array elements in reverse order).
6.End
```

## PROGRAM

```
#include <stdio.h>

int main()
{
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d ",&a[i]);
    }
    for(int i=n-1;i>=0;i--)
    {
      printf("%d ",a[i]);
    }
    
    return 0;
}
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/370ad50a-eec7-4d5a-86b7-8ee7fe437cb9)


## RESULT

Thus the program in C to read n number of values in an array and display it in reverse order has been executed successfully


# EX-14-ARRAY

## AIM

Write a C program to delete last element in an array.

## ALGORITHM

```
1.Start
2.Input an integer n (size of the array).
3.Declare an integer array arr[n].
4.Repeat for i from 0 to n-1:
a. Input arr[i] (read array elements).
5.Repeat for i from 0 to n-2:
a. Print arr[i] followed by a space.
6.Print a newline.
7.End

```

## PROGRAM

```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    for (int i = 0; i < n - 1; i++)
        printf("%d ", arr[i]);
    printf("\n");
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/532f2044-87cb-4fe5-87bb-3acc00edf6f9)


## RESULT

Thus the program to delete last element in an array has been executed successfully.


# EX -15 - Array

## Aim:

Write a C program to read the elements of the n x n matrix and check whether the first element is divisible by 5.

## Algorithm:

```
1.Start
2.Input the size of the matrix n.
3.Declare a 2D array a[10][10].
4.Repeat for i from 0 to n-1:
a. Repeat for j from 0 to n-1:
i. Input a[i][j].
5.Check if a[0][0] is divisible by 5:
a. If a[0][0] % 5 == 0, then:
6.Print: "a[0][0] = <value> is divisible by 5"
b. Else:
7.Print: "a[0][0] = <value> is not divisible by 5"
8.End
```

## Program:

```
#include<stdio.h>
int main()
{
    int i,j,n,a[10][10];
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
    if(a[0][0]%5==0)
    printf("a[0][0] =%d is divisible by 5",a[0][0]);
    else
    printf("a[0][0] =%d is not divisible by 5",a[0][0]);
    return 0;
}
```

## Output:
 ![image](https://github.com/user-attachments/assets/00892b63-0813-4f7d-920b-554baff73080)

 
## Result:

Thus, the program to read the elements of the n x n matrix and check whether the first element is divisible by 5 was verified successfully.



