# EX 59 C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use character data in Queue).
## DATE:08/05/2025
## AIM: To write a C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a functions to perform enqueue, dequeue,peek,display, in Queue using linked 
list. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End
   
## Program:
```
struct Node 
{ 
char data; 
struct Node *next; 
}*front=NULL,*rear=NULL; 
void enqueue(char data) 
{ 
struct Node *n=(struct Node*)malloc(sizeof(struct Node)); 
n->data=data; 
n->next=NULL; 
if(front==NULL) 
{ 
front=rear=n; 
} 
else 
{ 
rear->next=n; 
rear=n; 
} 
} 
Void display() 
{ 
struct Node *temp; 
temp=front; 
if(temp==NULL) 
{ 
printf("queue elements:\n"); 
} 
else 
{ 
printf("queue elements:\n"); 
while(temp!=NULL) 
{ 
printf("%c\n",temp->data); 
temp=temp->next; 
} 
} 
} 
void dequeue() 
{ 
struct Node *temp; 
temp=front; 
if(temp==NULL) 
{ 
printf("queue is empty\n"); 
} 
else 
{ 
front=temp->next; 
free(temp); 
} 
} 
void peek(){ 
printf("peek:"); 
printf("%c\n",front>data);
}
/*
functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use character data in Queue).

Developed by: 
RegisterNumber:  
*/
```

## Output:

SAMPLE INPUT:

front=NULL;

rear=NULL;

enqueue('R');

enqueue('A');

enqueue('V'); 

enqueue('I');

display();

peek();

dequeue();

dequeue();

display();

peek();


SAMPLE OUTPUT:

queue elements:

R

A

V

I

peek: R

queue elements:

V

I

peek:V


## Result:
Thus the program was executed and the output was verified successfully.
