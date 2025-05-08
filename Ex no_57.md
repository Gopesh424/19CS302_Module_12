# EX 57 C function to perfom push,pop and peek functions in Stack using Linked List.( store float data in stack)
## DATE:08/05/2025
## AIM: To write a C function to perfom push,pop and peek functions in Stack using Linked List.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a program to push an element in stack using linked list. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End 

## Program:
```
struct Node 
{ 
float data; 
struct Node *next; 
}*head; 
void push(float data) 
{ 
struct Node *temp; 
temp=(struct Node*)malloc(sizeof(struct Node)); 
if(temp==NULL) 
{ 
temp->data=data; 
temp->next=NULL; 
head=temp; 
} 
else 
{ 
temp->data=data; 
temp->next=head; 
head=temp; 
}  
} 
/*
function to perfom push,pop and peek functions in Stack using Linked List.( store float data in stack)

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


## Result:
Thus the program was executed and the output was verified successfully.
