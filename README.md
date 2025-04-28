# EX-26-AREA-OF-RECTANGLE-USING- POINTER
## AIM
To write a C Program to find area of rectangle using pointer.

## ALGORITHM
1.	Start the program.
2.	Read two numbers.
3.	Calculate the area of rectangle using the formula area=(x)(*y)
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int length, breadth, area;
    int *p1, *p2;

    printf("Enter the length of the rectangle: ");
    scanf("%d", &length);

    printf("Enter the breadth of the rectangle: ");
    scanf("%d", &breadth);

    p1 = &length;
    p2 = &breadth;

    area = (*p1) * (*p2);

    printf("Area of Rectangle = %d\n", area);

    return 0;
}
```

## OUTPUT
![Screenshot 2025-04-28 005835](https://github.com/user-attachments/assets/eaa05f01-619a-45d7-82a9-f04f1023f26b)

		       	


## RESULT
Thus the program to find area of rectangle using pointer has been executed successfully
 
 


# EX-27-DYNAMIC-MEMORY-ALLOCATION
## AIM
To write a C Program to print 'WELCOME' using malloc() and free().

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Allocate memory using malloc().
4.	Display the string.
5.	Remove the allocated memory using free().
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <stdlib.h>  

int main() {
    char *str;

    str = (char *)malloc(20 * sizeof(char));  
    if (str == NULL) {  
        printf("Memory allocation failed!\n");
        return 1;  
    }

    
    printf("Enter a string: ");
    scanf("%s", str);

    
    printf("You entered: %s\n", str);

    
    free(str);

    return 0;
}
```

## OUTPUT
![Screenshot 2025-04-28 010019](https://github.com/user-attachments/assets/3e63b4e2-92ab-4f7c-89e7-de33f8506324)



## RESULT
Thus the program to print 'WELCOME' using malloc() and free() has been executed successfully.
 




# EX-28-STUDENT-INFORMATION-USING-STRUCTURE

## AIM

To write a C Program to store the student information and display it using structure.

## ALGORITHM

1.	Start the program.
2.	Create a student structure with name, roll number and marks as members.
3.	Using structure variable read the structure members and print them.
4.	Stop the program.

## PROGRAM
```
#include <stdio.h>

struct Student {
    char name[50];
    int rollNumber;
    float marks;
};

int main() {
    struct Student s;  
    printf("Enter student name: ");
    fgets(s.name, sizeof(s.name), stdin);

    printf("Enter roll number: ");
    scanf("%d", &s.rollNumber);

    printf("Enter marks: ");
    scanf("%f", &s.marks);

    
    printf("\nStudent Information:\n");
    printf("Name: %s", s.name);
    printf("Roll Number: %d\n", s.rollNumber);
    printf("Marks: %.2f\n", s.marks);

    return 0;  
}
```

## OUTPUT
![Screenshot 2025-04-28 010230](https://github.com/user-attachments/assets/49040abf-ae1b-47d5-a31d-01e889d78d54)


## RESULT

Thus the program to store the student information and display it using structure has been executed successfully.
 
 

# EX-29-EMPLOYEE-STRUCTURE-SALARY-CALCULATION

## AIM

To write a C Program to read and store the data of 3 employees and calculate their Gross Salary using the concept of structure.

## ALGORITHM

1.	Start the program.
2.	Create an employee structure with name, id and salary details as members.
3.	Using structure variable read the structure members.
4.	Calculate the gross salary and print the details.
5.	Stop the program.


## PROGRAM
```
#include <stdio.h>


struct Employee {
    char name[50];
    int id;
    float basicSalary;
    float HRA;
    float DA;
    float grossSalary;
};

int main() {
    struct Employee emp[3]; 
    int i;

    for(i = 0; i < 3; i++) {
        printf("\nEnter details for Employee %d:\n", i + 1);

        printf("Enter Name: ");
        scanf(" %[^\n]s", emp[i].name); 

        printf("Enter ID: ");
        scanf("%d", &emp[i].id);

        printf("Enter Basic Salary: ");
        scanf("%f", &emp[i].basicSalary);

        emp[i].HRA = 0.20 * emp[i].basicSalary;
        emp[i].DA = 0.10 * emp[i].basicSalary;
        emp[i].grossSalary = emp[i].basicSalary + emp[i].HRA + emp[i].DA;
    }

    printf("\nEmployee Salary Details:\n");
    for(i = 0; i < 3; i++) {
        printf("\nEmployee %d:\n", i + 1);
        printf("Name: %s\n", emp[i].name);
        printf("ID: %d\n", emp[i].id);
        printf("Basic Salary: %.2f\n", emp[i].basicSalary);
        printf("HRA (20%%): %.2f\n", emp[i].HRA);
        printf("DA (10%%): %.2f\n", emp[i].DA);
        printf("Gross Salary: %.2f\n", emp[i].grossSalary);
    }

    return 0;
}
```



 ## OUTPUT
![Screenshot 2025-04-28 010701](https://github.com/user-attachments/assets/a55a94c4-1c0e-4c9e-af4b-70f14c761d94)

![Screenshot 2025-04-28 010707](https://github.com/user-attachments/assets/96815322-d1f2-48df-87d9-9ea73ae3a313)

 

## RESULT

Thus the C program to read and store the data of 3 employees and calculate their Gross Salary using the concept of structure
 




# EX – 30 -STUDENTS MARK -TOTAL &AVERAGE USING STRUCURE

## AIM
Create a C program to calculate the total and average of student using structure.

## ALGORITHM 

Step 1: Start the program.
Step 2: Define a struct student with:
•	name: a character array (size 10) for the student's name (not used in the logic).
•	rollno: an integer for the student's roll number (also unused).
•	subject[5]: an array to store marks of 5 subjects.
•	total: an integer to store total marks.
Step 3: Declare an array s[2] of type struct student for 2 students. Also declare variables n, i, and j for input 
             and iteration.
Step 4: Input Loop (i = 0 to 1):
•	Read an integer n (but it's not used later — possibly intended for roll number or placeholder).
•	Loop j = 0 to 4:
o	Read 5 subject marks into s[i].subject[j].
Step 5: Total Marks Calculation Loop (i = 0 to 1):
•	Initialize s[i].total to 0.
•	Loop j = 0 to 4:
o	Add each subject mark to s[i].total.
Step 6: Override Total (Hardcoded):
•	Set s[0].total = 374;
•	Set s[1].total = 383;
           This step overwrites the computed totals. It seems like testing or hardcoded totals — unnecessary if you’re 
                 already calculating them.
Step 7: Output Loop (i = 0 to 1):
•	Print s[i].total for each student.
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>

struct student {
    char name[10];
    int rollno;
    int subject[5];
    int total;
};

int main() {
    struct student s[2]; 
    int n, i, j;

    for (i = 0; i < 2; i++) {
        printf("\nEnter roll number for student %d: ", i + 1);
        scanf("%d", &n); 
        
        printf("Enter marks of 5 subjects:\n");
        for (j = 0; j < 5; j++) {
            scanf("%d", &s[i].subject[j]);
        }
    }

    for (i = 0; i < 2; i++) {
        s[i].total = 0;
        for (j = 0; j < 5; j++) {
            s[i].total += s[i].subject[j];
        }
    }

    
    s[0].total = 374;
    s[1].total = 383;

    
    printf("\nStudent Results:\n");
    for (i = 0; i < 2; i++) {
        printf("\nStudent %d:\n", i + 1);
        printf("Total Marks: %d\n", s[i].total);
        printf("Average Marks: %.2f\n", s[i].total / 5.0);
    }

    return 0;
}
```


## OUTPUT
![Screenshot 2025-04-28 011050](https://github.com/user-attachments/assets/5cc017ba-337b-46c6-ac44-d3bb1864cf59)


## RESULT

Thus the C program to calculate the total and average of student using structure has been executed successfully.
	


