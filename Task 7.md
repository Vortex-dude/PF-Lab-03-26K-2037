#include <stdio.h>
 
int main() {
   char ch1, ch2, ch3;
 
   printf("Enter first character: ");
   ch1 = getchar();
   getchar();
 
   printf("Enter second character: ");
   ch2 = getchar();
   getchar();
 
   printf("Enter third character: ");
   ch3 = getchar();
   getchar();
 
   printf("--------------------------------\n");
   printf("Characters Entered:\n");
 
   printf("Character 1 : ");
   putchar(ch1);
   printf("\n");
 
   printf("Character 2 : ");
   putchar(ch2);
   printf("\n");
 
   printf("Character 3 : ");
   putchar(ch3);
   printf("\n");
 
   printf("--------------------------------\n");
 
   return 0;
}
