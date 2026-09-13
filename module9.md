EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:

<img width="717" height="602" alt="image" src="https://github.com/user-attachments/assets/8bff5f8a-e87d-436f-8cc4-4d642f98a80d" />


Output:

<img width="734" height="428" alt="image" src="https://github.com/user-attachments/assets/311dd296-b3bf-4885-aaa0-90de9b3ed72e" />



Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:

<img width="633" height="601" alt="image" src="https://github.com/user-attachments/assets/0b36d05f-d8b2-46c7-82aa-47da1932c34d" />


Output:

<img width="781" height="285" alt="image" src="https://github.com/user-attachments/assets/6f507963-18eb-4f9e-8c47-5e7dd9c512d5" />




Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:

<img width="708" height="645" alt="image" src="https://github.com/user-attachments/assets/3e79724c-56c7-4401-9d66-f2b8afd02653" />

Output:

<img width="956" height="322" alt="image" src="https://github.com/user-attachments/assets/8fbb150a-f735-490b-8176-fb03679f6195" />



Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:

#include <stdio.h>

int main()
{
    int queue[10];
    int front = 0, rear = -1;
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    if(n > 10)
    {
        printf("Queue Overflow");
        return 0;
    }

    printf("Enter elements:\n");

    for(i = 0; i < n; i++)
    {
        rear++;
        scanf("%d", &queue[rear]);
    }

    printf("Queue elements are:\n");

    for(i = front; i <= rear; i++)
    {
        printf("%d ", queue[i]);
    }

    return 0;
}
Output:

<img width="1654" height="766" alt="image" src="https://github.com/user-attachments/assets/c6042c1d-04a5-413b-9dd2-52b78e16d63d" />


Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:

#include <stdio.h>

int queue[10];
int front = 0, rear = -1;

void deleteElement()
{
    if(front > rear)
    {
        printf("Queue Underflow\n");
    }
    else
    {
        printf("Deleted element: %d\n", queue[front]);
        front++;
    }
}

int main()
{
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter queue elements:\n");

    for(i = 0; i < n; i++)
    {
        rear++;
        scanf("%d", &queue[rear]);
    }

    deleteElement();

    printf("Queue after deletion:\n");

    for(i = front; i <= rear; i++)
    {
        printf("%d ", queue[i]);
    }

    return 0;
}

Output:

<img width="1658" height="777" alt="image" src="https://github.com/user-attachments/assets/b8d4753a-a3a1-4eb6-989e-e162d8ebf24f" />



Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
