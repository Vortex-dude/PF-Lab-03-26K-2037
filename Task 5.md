#include <stdio.h>
 
int main() {
   int a;
   unsigned int b;
   float f;
   double d;
   char c;
   long int l;
 
   printf("Enter an integer: ");
   scanf("%d", &a);
   printf("Enter an unsigned integer: ");
   scanf("%u", &b);
   printf("Enter a float value: ");
   scanf("%f", &f);
   printf("Enter a double value: ");
   scanf("%lf", &d);
   printf("Enter a character: ");
   scanf(" %c", &c);
   printf("Enter a long int value: ");
   scanf("%ld", &l);
 
   printf("   DATA TYPE & FORMAT SPECIFIER DEMO    \n");
 
   printf("\nInteger value in different bases:\n");
   printf("Decimal            : %d\n", a);
   printf("Octal              : %o\n", a);
   printf("Hexadecimal (lower): %x\n", a);
   printf("Hexadecimal (upper): %X\n", a);
 
   printf("\nOther values:\n");
   printf("Unsigned int       : %u\n", b);
   printf("Character          : %c\n", c);
   printf("Long int           : %ld\n", l);
 
   printf("\nFloating-point value using different specifiers:\n");
   printf("%%f (decimal)      : %f\n", f);
   printf("%%e (scientific)   : %e\n", f);
   printf("%%g (general)      : %g\n", f);
 
   printf("\nDouble value using different specifiers:\n");
   printf("%%f (decimal)      : %f\n", d);
   printf("%%e (scientific)   : %e\n", d);
   printf("%%g (general)      : %g\n", d);
 
   return 0;
}
