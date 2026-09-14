#include <stdio.h>
 
int main() {
   char name[50];
   int rollNo;
   char section;
   int age;
   double cgpa;
   float height;
 
   printf("Enter student name: ");
   scanf(" %[^\n]", name);
 
   printf("Enter roll number: ");
   scanf("%d", &rollNo);
 
   printf("Enter section: ");
   scanf(" %c", &section);
 
   printf("Enter age: ");
   scanf("%d", &age);
 
   printf("Enter CGPA: ");
   scanf("%lf", &cgpa);
 
   printf("Enter height: ");
   scanf("%f", &height);
 
   printf("\n========================================\n");
   printf("             STUDENT REPORT\n");
   printf("========================================\n");
   printf("Field\t\t Value\n");
   printf("----------------------------------------\n");
   printf("Name\t\t %s\n", name);
   printf("Roll Number\t %d\n", rollNo);
   printf("Section\t\t %c\n", section);
   printf("Age\t\t %d\n", age);
   printf("CGPA\t\t %.2f\n", cgpa);
   printf("Height\t\t %.2f\n", height);
   printf("----------------------------------------\n");
 
   return 0;
}
