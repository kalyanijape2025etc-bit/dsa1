//QUEUE using array
#include <stdio.h>
#include <stdlib.h>
#define SIZE 5
struct Queue {
int arr[SIZE];
int front, rear;
} q;
int isfull() {
if (q.rear >= SIZE - 1)
return 1;
else
return 0;
}
void insert(int item) {
if (isfull()) {
printf("\n Queue is full");
} else {
q.rear = q.rear + 1;
q.arr[q.rear] = item;
}
}
int isempty() {
if (q.front > q.rear)
return 1;
else
return 0;
}
int delete() {
int item;
if (isempty()) {
printf("\n Queue is Empty");
return -1;
} else {
item = q.arr[q.front];

q.front = q.front + 1;
return item;
}
}
void display() {
int i;
if (isempty()) {
printf("\n Queue is Empty");
} else {
for (i = q.front; i <= q.rear; i++) {
printf("%d\t", q.arr[i]);
}
}
}
void main() {
int choice, item;
q.front = 0;
q.rear = -1;
while (1) {
printf("\n Implementation of queue");
printf("\n 1. Insert");
printf("\n 2. Delete");
printf("\n 3. Display");
printf("\n 4. Exit");
printf("\n Enter Choice: ");
scanf("%d", &choice);
switch (choice) {
case 1:
printf("\n Enter item to insert: ");
scanf("%d", &item);
insert(item);
break;
case 2:
if (isempty()) {
printf("\n Queue is Empty");

} else {
item = delete();
}
break;
case 3:
display();
break;
case 4:
printf("\n Exiting the program...");
exit(0);
default:
printf("\n Invalid Choice !!");
}
}
}
