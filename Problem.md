# Pseudocode
## 1. Display student information using different data types.
```
START
    DECLARE name : STRING
    DECLARE rollNo. : INTEGER
    DECLARE gpa : FLOAT
    DECLARE grade : CHAR
    DECLARE isEnrolled : BOOLEAN

    OUTPUT "Enter your name: "
    INPUT name
    OUTPUT "Enter your roll number: "
    INPUT rollNo.
    OUTPUT "Enter your GPA: "
    INPUT gpa
    OUTPUT "ENTER your grade: "
    INPUT grade
    
    OUTPUT "Student Name: " + name
    OUTPUT "Roll Number: " + rollNo.
    OUTPUT "GPA: " + gpa
    OUTPUT "Grade: " grade
END
```

## 2. Read and display a character using getchar() and putchar().
```
START
    DECLARE ch AS CHARACTER

    OUTPUT "Enter a character: "
    ch = getchar()

    OUTPUT "You entered: "
    putchar(ch)
END
```

## 3. Display a floating-point value using different precision settings.
```
START
    DECLARE value AS FLOAT

    OUTPUT "Enter a floating-point number: "
    INPUT value

    DISPLAY "Default precision: " + value
    DISPLAY "1 decimal place: " + FORMAT(value, 1)
    DISPLAY "2 decimal places: " + FORMAT(value, 2)
    DISPLAY "4 decimal places: " + FORMAT(value, 4)
END
```
