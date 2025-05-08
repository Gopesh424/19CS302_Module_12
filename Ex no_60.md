# EX 60 C function to find the peek element of the queue using linked list.
## DATE:08/05/2025
## AIM:To write a C function to find the peek element of the queue using linked list.

## Algorithm
1. Start
2. Define Node Structure: Each node will store data and a pointer to the next node.
3. Initialize Front and Rear pointers to manage the queue.
4. Enqueue: Create a new node.
5. If the queue is empty, set both front and rear to the new node.
6. Peek: If the queue is not empty, return the front node's data.
7. Display: For sample output, print the whole queue  
8. End
   
## Program:
```
#include <stdio.h>
#include <stdlib.h>

// Define node structure
struct Node {
    int data;
    struct Node* next;
};

// Define front and rear pointers
struct Node* front = NULL;
struct Node* rear = NULL;

// Enqueue function
void enqueue(int value) {
    struct Node* newNode = (struct Node*)malloc(sizeof(struct Node));
    newNode->data = value;
    newNode->next = NULL;

    if (rear == NULL) {
        front = rear = newNode;
    } else {
        rear->next = newNode;
        rear = newNode;
    }
}

// Peek function - returns the front element
int peek() {
    if (front == NULL) {
        printf("Queue is empty.\n");
        return -1;  // Sentinel value
    } else {
        return front->data;
    }
}

// Display the queue (for demonstration)
void display() {
    struct Node* temp = front;
    if (front == NULL) {
        printf("Queue is empty.\n");
        return;
    }
    printf("Queue elements: ");
    while (temp != NULL) {
        printf("%d ", temp->data);
        temp = temp->next;
    }
    printf("\n");
}

// Main function
int main() {
    enqueue(10);
    enqueue(20);
    enqueue(30);

    display();

    int frontElement = peek();
    if (frontElement != -1)
        printf("Peek element (front of queue): %d\n", frontElement);

    return 0;
}

/*
C function to find the peek element of the queue using linked list.

Developed by: 
RegisterNumber:  
*/
```

## Output:
Queue elements: 10 20 30

Peek element (front of queue): 10


## Result:
Thus the program was executed and the output was verified successfully.
