#include <stdio.h>
#include <string.h>
void copy(char input[], char output[]);
int palindrome(char input[]);
void reverse(char input[]);
void substring(char input[]);
int stringlength(char input[]);
int main()
{
char str[10], output[10];
int ch, c;
printf("\nEnter the string: ");
scanf("%s", str);
do
{
printf("\n\n1) copy\n2) palindrome\n3) reverse\n4) substring\n5) Exit");
printf("\nEnter your choice: ");
scanf("%d", &ch);
switch(ch)
{
case 1:
copy(str, output);
break;
case 2:
c = palindrome(str);
if (c == 1)
printf("\nThe given string is a Palindrome.");
else
printf("\nThe given string is not a Palindrome.");
break;

case 3:
reverse(str);
break;
case 4:
substring(str);
break;
case 5:
printf("\nExiting program.");
break;
default:
printf("\nInvalid choice! Please select 1-5.");
}
} while (ch != 5);
return 0;
}
int palindrome(char name[])
{
int i = 0, j = 0;
while (name[j] != '\0')
j++;
j--;
while (i < j)
{
if (name[i] != name[j])
return 0;
i++;
j--;
}
return 1;
}
void copy(char input[], char output[])
{
int i;
for (i = 0; input[i] != '\0'; i++)
{
output[i] = input[i];
}
output[i] = '\0';

printf("\nThe output (copied) string is: %s", output);
}
void substring(char input[])
{
int i, n, position;
char output[10];
printf("\nEnter the starting position of substring (0-indexed): ");
scanf("%d", &position);
n = stringlength(input);
if (position >= 0 && position < n)
{
for (i = 0; i < n - position; i++)
{
output[i] = input[position + i];
}
output[i] = '\0';
printf("\nInput string: %s\nOutput substring: %s", input, output);
}
else
{
printf("\nPosition entered is out of range.");
}
}
int stringlength(char input[])
{
int i = 0;
while (input[i] != '\0')
{
i++;
}
return i;
}
void reverse(char input[])
{
int n, i;
char output[10];
n = stringlength(input);
for (i = 0; i < n; i++)
{
output[n - 1 - i] = input[i];
}
output[n] = '\0';
printf("\nInputstring: %s\nOutput(reversed)string: %s", input, output);
}
