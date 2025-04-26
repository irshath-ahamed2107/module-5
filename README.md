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
![Screenshot 2025-04-26 105449](https://github.com/user-attachments/assets/5dbeaa84-a4c0-492d-890d-1ec78e7c3675)

## OUTPUT
![Screenshot 2025-04-26 105500](https://github.com/user-attachments/assets/0184d91d-f8db-4645-8af5-1754bd1be031)
		       	


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
![Screenshot 2025-04-26 110032](https://github.com/user-attachments/assets/e0ab2cb8-736a-4d3a-9614-c150ef7c47c8)


## OUTPUT
![Screenshot 2025-04-26 110040](https://github.com/user-attachments/assets/8ec16b69-1983-4cf1-9bc5-a6b4911452f7)



## RESULT
Thus the program to print 'WELCOME' using malloc() and free() has been executed successfully
 
.



# EX-28-STUDENT-INFORMATION-USING-STRUCTURE

## AIM

To write a C Program to store the student information and display it using structure.

## ALGORITHM

1.	Start the program.
2.	Create a student structure with name, roll number and marks as members.
3.	Using structure variable read the structure members and print them.
4.	Stop the program.

## PROGRAM
![Screenshot 2025-04-26 110659](https://github.com/user-attachments/assets/6004e83a-2507-4c7f-abb1-3c169f0248fe)


## OUTPUT
![Screenshot 2025-04-26 110706](https://github.com/user-attachments/assets/d52661bb-68a8-40e5-a327-f7bdef0daebf)


## RESULT

Thus the program to store the student information and display it using structure has been executed successfully
 
 


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
![Screenshot 2025-04-26 112958](https://github.com/user-attachments/assets/91f7b7f1-d896-4a90-b620-45c64c39d007)


 ## OUTPUT
![Screenshot 2025-04-26 113017](https://github.com/user-attachments/assets/6b0058d9-26a4-44d6-aa42-af6ca1dfca85)

![Screenshot 2025-04-26 113023](https://github.com/user-attachments/assets/c656b9ad-f430-485c-a313-9589d4c391c1)


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
![Screenshot 2025-04-26 113655](https://github.com/user-attachments/assets/a1514c7d-ab76-4b98-b845-b8d42eadd5f7)


## OUTPUT

![image](https://github.com/user-attachments/assets/bcc3d330-5d49-47d5-a91a-70803f8e0a1b)
![Screenshot 2025-04-26 113714](https://github.com/user-attachments/assets/fa7a48d7-1d8b-4b15-9a5c-e21e1eb7dd1b)
![Screenshot 2025-04-26 113722](https://github.com/user-attachments/assets/02d899ee-e98d-4d84-8126-2366a96e9f9b)


## RESULT

Thus the C program to calculate the total and average of student using structure has been executed successfully.
	


