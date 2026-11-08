Grading_system readme.file
Group 12
students name : Cephas Syamupa, student_id : 202601059 
                Stacey Chitundu, student_id : 202612681  
                Emmanuel Siame, student_id : 202605604   
                Tumelo Chizoka, student_id: 202612988
                Emmanuel Mwila, student_id : 202605299 
                Harrison Shawa, student_id: 202602128 
                Mwaka Nankololwe, student_id : 202607766 
                Faith Mutofwe, student_id : 202612512  
                Abigail Chibeka Chikumbi, student_id : 202602898 
                Bumi Lukomona, student_id : 202402328 
                Natasha Nachalwe, student_id : 202500090   

What is this Project:
This is a simple program that runs the program in python,adds a student and their mark,outputs  all the students and their results and outputs  the class summary. This uses lists and dictionaries to store records, if/elif/else to classify marks,for and while loops to process records and repeat them in the menu and functions to keep the code organised .

Planning:
Input
- user types a menu option fron 1 to 4
-when adding a student, the user types the students name,student number, and mark.
Process
-The system formats the name , checks that the mark is between 0 to100
- uses if/elif/else to decide te remark,stores the details in a dictionary
- adds the dictionary to the students list
Output
- The menu of the four options
- a report of all students 
- a class summary
- clear message such as student database is empty when there are no records
Grading scale
This is the Grading system provided
Mark.                        Grade.               Decision.
80-100.                      A.                   Excellent
70-79.                       B.                   Very Good
60-69.                       C.                   Good
50-59.                       D.                   Pass
0-49.                        F.                   Fail

Why a list of dictionaries is suitable:
Each dictionary stores one student,each detail is a key such as name, student_id, mark and decision so it makes student['mark'] is easy to read and hard to mix-up and avoid confusion. The list stores the whole , new students can be added appen(),and so the list can easily grow. Loops also work well with them, as the first loop,can easily loop through each student to print out a report.

How the program works
Menu
These are options that continue to appear until the user enters option 4 to exit the loop .
option1: adds the student; asks the student name, id number,mark and records this input and gives a decision 
option2: Display all; uses the for loop to print each students name, id, mark and remark
option3: Class summary; Prints the name and student id of every student 
option 4: Exit; stops the loop and closes the program

Code structure:
students - This is a list of dictionaries that stores every student record,it starts with 11 sample students.
add_student(student_list) - This collects a new students details, checks the marks and adds the new record from the user entry
display_all(student_list) - This prints the full, details of every student, or a message that the lit is empty
c_summary(student_list) - prints the class summary. ary of names and student ids
Mainprogram loop - shows the menu and calls the correct function for the associated chosen option

How to run the program 
1.Install Python 3 if not already installed
2.Download or lonely the project;grading_system.py is in a folder
3. Open the terminal inside tht folder 
4. Run the python grading_system.py
5. Enter your desired number according to the options

Why does the order of if/elif matter at grade boundaries?
This matters python checks conditions from top to bottom and runs only first that is true .If mark>=50 was written before mark >=80,a mark of 86 would be given "Pass" instead ad of "Excellent",because it already satisfies the first condition. By checking th highest mark first and moving downwards,every boundary mrk such as 49,50,79 and 80misnplaced in the correct grade.

what error could arise when calculating the average of an empty list
A ZeroDivisionError. The average is the total of the marks divided by the number of students. If there are no students,the program would,d divide zero and crash. To prevent this, the program should first check that the lit is not empty and ho an informative message instead.

How to adapt the program to handle two courses per student
Each student dictionary could have a courses key that holds a list of course records,for example{'course':'ICT111','mark':80}. The program would then ask which course a mrk belongs to, and loops would go through each students courses to grade them and calculate statstistics.



