// Stack using array
#include <stdio.h>
#include <stdlib.h>
#define SIZE 5
struct stack
{
int s[SIZE];
int top;
} st;
int isFull()
{
if (st.top >= SIZE - 1)
return 1;
else
return 0;
}
int isEmpty()
{
if (st.top == -1)
return 1;
else
return 0;
}
int pop()
{
int item;
item = st.s[st.top];
st.top--;
return item;
}
void push(int item)
{
st.top++;
st.s[st.top] = item;
}
void display()
{
int i;

if (isEmpty())
printf("\nStack is empty!!!");
else
{
for (i = st.top; i >= 0; i--)
printf("\n%d", st.s[i]);
}
}
int main(void)
{
int item, choice;
char ans;
st.top = -1;
printf("\nImplementation of Stack");
do
{
printf("\nMain menu");
printf("\n1. Push\n2. Pop\n3. Display\n4. Exit");
printf("\nEnter your choice: ");
scanf("%d", &choice);
switch (choice)
{
case 1:
printf("\nEnter the item to be pushed: ");
scanf("%d", &item);
if (isFull())
printf("\nStack is full");
else
push(item);
break;
case 2:
if (isEmpty())
printf("\nEmpty stack (Underflow)");
else
{
item = pop();
printf("\nThe popped element is: %d", item);
}
break;

case 3:
display();
break;
case 4:
exit(0);
}
printf("\nDo you want to continue? (Y/N): ");
scanf(" %c", &ans);
} while (ans == 'Y' || ans == 'y');
return 0;
}
