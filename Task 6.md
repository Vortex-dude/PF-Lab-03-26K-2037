#include <stdio.h>
 
int main() {
   float fVal;
   double dVal;
 
   printf("Enter a float value: ");
   scanf("%f", &fVal);
 
   printf("Enter a double value: ");
   scanf("%lf", &dVal);
 
   printf("\n========================================\n");
   printf("          PRECISION COMPARISON\n");
   printf("========================================\n");
 
   printf("Float value:\n");
   printf("Default : %f\n", fVal);
   printf("2 digits: %.2f\n", fVal);
   printf("4 digits: %.4f\n", fVal);
   printf("6 digits: %.6f\n", fVal);
 
   printf("\nDouble value:\n");
   printf("Default : %f\n", dVal);
   printf("2 digits: %.2f\n", dVal);
   printf("4 digits: %.4f\n", dVal);
   printf("6 digits: %.6f\n", dVal);
 
   return 0;
}
