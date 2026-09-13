EXP NO:6 C PROGRAM PRINT THE LOWERCASE ENGLISH WORD CORRESPONDING TO THE NUMBER
Aim:
To write a C program print the lowercase English word corresponding to the number
Algorithm:
1.	Start
- Initialize an integer variable n.
2.	Input Validation
3.	Switch Statement cases.
-	Case 5: Print "seventy one"
-	Case 6: Print "seventy two"
-	Case 13: Print "seventy three"
-	...
-	Case 13: Print "seventy nine"
-	Default: Print "Greater than 13"
4.	Exit the program.
 
Program:

<img width="607" height="672" alt="image" src="https://github.com/user-attachments/assets/013adf32-d0ac-4258-8095-e0d3e2ab730e" />





Output:


<img width="712" height="216" alt="image" src="https://github.com/user-attachments/assets/b7ca353f-46e7-4f87-8bb1-6f14a3011ee3" />






Result:
Thus, the program is verified successfully
 
EXP NO:7 C PROGRAM TO PRINT TEN SPACE-SEPARATED INTEGERS     IN A SINGLE  LINE DENOTING THE FREQUENCY OF EACH DIGIT FROM 0 TO 3 .
Aim:
To write a C program to print ten space-separated integers in a single line denoting the frequency of each digit from 0 to 3.
Algorithm:
1.	Start
2.	Declare char array a[50] outer loop for each digit from 0 to 3
3.	Initialize counter c to 0
4.	For each character in the string print count c for current digit, followed by a space
5.	Increment h to move to the next digit
6.	End
 
Program:

<img width="732" height="561" alt="image" src="https://github.com/user-attachments/assets/101db30f-525c-480b-8c22-a6dda36d0e9e" />




Output:


<img width="787" height="364" alt="image" src="https://github.com/user-attachments/assets/5715b8aa-fada-4f1f-bb47-6cb8201c9c87" />





Result:
Thus, the program is verified successfully

EXP NO:8 C PROGRAM TO PRINT ALL OF ITS PERMUTATIONS IN STRICT LEXICOGRAPHICAL ORDER.
Aim:
To write a C program to print all of its permutations in strict lexicographical order.

Algorithm:
1.	Start
2.	Declare variables s (pointer to an array of strings) and n (number of strings)

3.	Memory Allocation
Dynamically allocate memory for s to store an array of strings
4.	Input
Read the number of strings n from the user Dynamically allocate memory for each string in s
5.	Permutation Generation Loop
6.	Memory Deallocation
Free the memory allocated for each string in s Free the memory allocated for s
7.	End
 
Program:

#include <stdio.h>
#include <string.h>

void sort(char str[])
{
    int i, j;
    char temp;

    for(i = 0; str[i] != '\0'; i++)
    {
        for(j = i + 1; str[j] != '\0'; j++)
        {
            if(str[i] > str[j])
            {
                temp = str[i];
                str[i] = str[j];
                str[j] = temp;
            }
        }
    }
}

int nextPermutation(char str[], int n)
{
    int i, j;
    char temp;

    i = n - 2;

    while(i >= 0 && str[i] >= str[i + 1])
        i--;

    if(i < 0)
        return 0;

    j = n - 1;

    while(str[j] <= str[i])
        j--;

    temp = str[i];
    str[i] = str[j];
    str[j] = temp;

    j = n - 1;

    while(i + 1 < j)
    {
        temp = str[i + 1];
        str[i + 1] = str[j];
        str[j] = temp;
        i++;
        j--;
    }

    return 1;
}

int main()
{
    char str[20];
    int n;

    printf("Enter a string: ");
    scanf("%s", str);

    n = strlen(str);

    sort(str);

    printf("Permutations in lexicographical order:\n");

    do
    {
        printf("%s\n", str);
    } while(nextPermutation(str, n));

    return 0;
}



Output:


<img width="814" height="324" alt="image" src="https://github.com/user-attachments/assets/acbaf2f4-32f8-453b-a361-1700d59a51e1" />






Result:
Thus, the program is verified successfully
 
EXP NO:9 C PROGRAM PRINT A PATTERN OF NUMBERS FROM 1 TO N AS
SHOWN BELOW.
Aim:
To write a C program to print a pattern of numbers from 1 to n as shown below.
Algorithm:
1.	Start
2.	Declare integer variables n, i, j, min
3.	Read the value of n from the user
4.	Calculate the length of the side of the square matrix: len = n * 2 - 1
5.	Matrix Generation Loop
6.	Calculate min as the minimum distance to the borders
7.	End
 
Program:

<img width="810" height="506" alt="image" src="https://github.com/user-attachments/assets/754d757f-e73c-4351-ae5a-d841218f7abf" />




Output:


<img width="705" height="321" alt="image" src="https://github.com/user-attachments/assets/a8b949fa-fca7-4f0b-ba58-8f80933762a8" />





Result:
Thus, the program is verified successfully

EXP NO:10 C PROGRAM TO FIND A SQUARE  OF NUMBER USING FUNCTION WITHOUT ARGUMENTS WITH RETURN TYPE

Aim:

To write a C program that calculates the square of a number using a function that does not take any arguments, but returns the square of the number.

Algorithm:

1.	Start.
2.	Define a function square() with no parameters. This function will return an integer value.
3.	Inside the function:
o	Declare an integer variable to store the number.
o	Ask the user to input a number.
o	Calculate the square of the number (multiply the number by itself).
o	Return the squared value.
4.	In the main function:
o	Call the square() function and display the result.
5.	End.

Program:

<img width="708" height="567" alt="image" src="https://github.com/user-attachments/assets/6e7f09a5-81b5-404d-8d3d-95d9dbcb4aa5" />





Output:


<img width="1665" height="634" alt="image" src="https://github.com/user-attachments/assets/d3134458-1ac8-48b1-bd95-25fe76cbf649" />





Result:
Thus, the program is verified successfully



























