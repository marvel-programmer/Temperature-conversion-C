//C program to convert temperature from Fahrenheit to Celsius and vice versa.
#include<stdio.h>

int main()
{
  int choice;
  float f, c;

  printf("1 - Convert from Fahrenheit to celsius\n2 - Convert from Celsius to Fahrenheit\nEnter Your Choice(1/2): ");
  scanf("%d", &choice);
  
  switch(choice)
  {
    case 1:
    printf("Enter the value in Fahrenheit: ");
    scanf("%f", &f);
    c = (f-32)*5/9;
    printf("Temperature in Celsius is %f", c);
    break;
    case 2:
    printf("Enter the value in Celsius: ");
    scanf("%f", &c);
    f = (c*9)/5+32;
    printf("Temperature in Fahrenheit is %f", f);
    break;
    default:
    printf("Please choose the correct option");
    break;
  }
  
  return 0;
}
