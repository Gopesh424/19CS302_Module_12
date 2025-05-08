# EX 58 C Function to display queue elements using Linked List.(use integer data in the queue)
## DATE:08/05/2025
## AIM: To write a C Function to display queue elements using Linked List.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a program to display queue elements using linked list. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End

## Program:
```
struct Node 
{ 
int data; 
struct Node *next; 
}*front=NULL,*rear=NULL; 
void display() 
{ 
struct Node *temp=front; 
if(temp==NULL) 
{ 
printf("queue is empty\n"); 
} 
else 
{ 
while(temp!=NULL) 
{ 
printf("%d\n",temp->data); 
temp=temp->next; 
} 
 
}
/*
C Function to display queue elements using Linked List.(use integer data in the queue)

Developed by: 
RegisterNumber:  
*/
```

## Output:
head=NULL;

push(10.01);

push(20.01);

push(30.01);

display();

30.01

20.01

10.01



## Result:
Thus the program was executed and the output was verified successfully.
