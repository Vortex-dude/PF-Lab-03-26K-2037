#include <stdio.h>
 
int main() {
   char name[50];
   int rollNo;
   int age;
   float height;
   double gpa;
   char section;
 
   printf("Enter student name: ");
   scanf(" %[^\n]", name);
 
   printf("Enter roll number: ");
   scanf("%d", &rollNo);
 
   printf("Enter age: ");
   scanf("%d", &age);
 
   printf("Enter height (in feet): ");
   scanf("%f", &height);
 
   printf("Enter GPA: ");
   scanf("%lf", &gpa);
 
   printf("Enter section: ");
   scanf(" %c", &section);
 
   printf("\n========================================\n");
   printf("           STUDENT INFORMATION\n");
   printf("========================================\n");
   printf("Name       : %s\n", name);
   printf("Roll No    : %d\n", rollNo);
   printf("Age        : %d\n", age);
   printf("Height     : %.1f\n", height);
   printf("GPA        : %.2f\n", gpa);
   printf("Section    : %c\n", section);
   printf("========================================\n");
 
   return 0;
}
