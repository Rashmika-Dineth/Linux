#include <stdio.h>

int main() {
  // Create an integer variable that will store the number we get from the user
  float a;
  float b;
  float c;

  // Ask the user to type a number 1
  printf("Type a number 1 and press enter: \n"); 
  // Get and save the number 1 the user types
  scanf("%f", &a);
   // Ask the user to type a number 2
  printf("Type a number 1 and press enter: \n"); 
  // Get and save the number 2 the user types
  scanf("%f", &b);
  
  c = a+b;

  // Print the number the user typed
  printf("Sum of the value is: %f", c);

  return 0;
}