#include <stdio.h>
 
int main() {
   char name[50];
   int rollNo;
   char section;
   char sampleChar;
   float value;
 
   printf("Enter student name: ");
   scanf(" %[^\n]", name);
   printf("Enter roll number: ");
   scanf("%d", &rollNo);
   printf("Enter section: ");
   scanf(" %c", &section);
   getchar();
   printf("Enter a sample character: ");
   sampleChar = getchar();
   getchar();
 
   printf("Enter a floating-point value: ");
   scanf("%f", &value);
 
   printf("\n=============================================\n");
   printf("          PROGRAMMING FUNDAMENTALS\n");
   printf("=============================================\n");
   printf("Name        : %s\n", name);
   printf("Roll No     : %d\n", rollNo);
   printf("Section     : %c\n", section);
 
   printf("\nC Topics:\n");
   printf("\t1. Variables\n");
   printf("\t2. Data Types\n");
   printf("\t3. Input/Output\n");
   printf("\t4. Format Specifiers\n");
   printf("\t5. Escape Sequences\n");
 
   printf("\nSample Character: '");
   putchar(sampleChar);
   printf("'\n");
 
   puts("Sample Question: \"What is C?\"");
 
   printf("\nFloating Value:\n");
   printf("Default : %f\n", value);
   printf("2-digit : %.2f\n", value);
   printf("4-digit : %.4f\n", value);
   printf("=============================================\n");
 
   return 0;
}
