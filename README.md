🎓 Student Grade Tracker System

A comprehensive Java application for managing and tracking student grades efficiently. This system allows educators and administrators to add students, record grades, calculate statistics, and generate detailed performance reports.

✨ Features


✅ Add Students - Register new students with unique IDs
✅ Grade Management - Add multiple grades per student
✅ Statistics Calculation - Automatic average, highest, and lowest score tracking
✅ Individual Reports - View detailed performance for each student
✅ Class Summary Reports - Generate comprehensive class-wide statistics
✅ Letter Grades - Automatic conversion to letter grades (A-F)
✅ Input Validation - Prevents invalid data entry
✅ User-Friendly Interface - Menu-driven console application


📋 System Requirements


Java Version: Java 8 or higher
Operating System: Windows, macOS, or Linux
RAM: Minimum 512 MB
Storage: Less than 1 MB


🚀 How to Run

1. Compile the Program

bashjavac StudentGradeTracker.java

2. Run the Program

bashjava StudentGradeTracker

3. Follow the Menu

The program will display an interactive menu with the following options:

1. Add a New Student
2. Add Grade to Existing Student
3. View All Students
4. View Individual Student Details
5. Generate Summary Report
6. Exit Program

📖 Usage Examples

Example 1: Add a Student

--- Add New Student ---
Enter Student Name: John Doe
Enter Student ID: S001
✅ Student John Doe added successfully!

Example 2: Add a Grade

--- Add Grade to Student ---
Enter Student ID: S001
Enter Grade (0-100): 85
✅ Grade added successfully!

Example 3: View Summary Report

📊 CLASS STATISTICS:
   • Total Students: 3
   • Total Grades Recorded: 9
   • Class Average: 82.33
   • Class Highest Score: 95.00
   • Class Lowest Score: 75.00

StudentID | Name          | Average | Highest | Lowest | Letter
S001      | John Doe      | 85.00   | 90.00   | 80.00  | B
S002      | Jane Smith    | 92.00   | 95.00   | 88.00  | A
S003      | Mike Johnson  | 78.00   | 85.00   | 75.00  | C

🏗️ Program Structure

Classes

1. Student Class

Represents individual student data and calculations.

Key Methods:


addGrade(double grade) - Add a grade for the student
getAverage() - Calculate average score
getHighest() - Get highest score
getLowest() - Get lowest score
getGradeLetters() - Convert grades to letters


2. GradeTracker Class

Manages all students and generates reports.

Key Methods:


addStudent(String name, String studentID) - Register new student
findStudent(String studentID) - Search for a student
displayAllStudents() - Show all students
generateSummaryReport() - Create class report
displayStudentDetails(String studentID) - View individual student stats


3. StudentGradeTracker Class

Main class with menu-driven user interface.

📊 Grading Scale

Average ScoreLetter Grade90-100A80-89B70-79C60-69DBelow 60F

🔍 Data Structures Used


ArrayList - Dynamic storage for students and grades
Scanner - User input handling
Collections - Built-in Java utilities for data management


✅ Features Breakdown

Input Validation


Student ID uniqueness check
Grade range validation (0-100)
Empty field prevention
Error handling for invalid input


Statistical Calculations


Individual student average
Class-wide average
Highest and lowest scores (individual & class)
Letter grade conversion
Count of grades per student


Reporting


Formatted table output
Clear visual hierarchy
Comprehensive statistics
Student-specific detailed views


🛠️ How It Works

┌─────────────────────┐
│   Start Program     │
└──────────┬──────────┘
           │
    ┌──────▼──────┐
    │  Main Menu  │
    └──────┬──────┘
           │
    ┌──────┴─────────────────────────────┐
    │                                    │
    ▼                                    ▼
Add Student                        Add Grade
    │                                    │
    ▼                                    ▼
View Students                    View Reports
    │                                    │
    └──────────────┬─────────────────────┘
                   │
            ┌──────▼──────┐
            │   Exit?     │
            └─────────────┘

📝 Sample Student Data

javaStudent S001: John Doe
  Grades: [85, 90, 88, 92]
  Average: 88.75
  Highest: 92
  Lowest: 85
  Letter Grade: B

Student S002: Jane Smith
  Grades: [95, 98, 92, 96]
  Average: 95.25
  Highest: 98
  Lowest: 92
  Letter Grade: A

🎯 Possible Enhancements


 Database integration (MySQL, SQLite)
 Graphical User Interface (GUI) with Swing
 Export reports to PDF/Excel
 Student attendance tracking
 Subject-wise grade tracking
 Email grade notifications
 File persistence (save/load data)
 Search and filter functionality
 Grade curve analysis


🐛 Troubleshooting

IssueSolution"Unrecognized command"Make sure Java is installed correctlyGrade not addedEnter a number between 0-100Student not foundCheck the Student ID is correctProgram crashesEnsure you're using Java 8 or higher

📄 License

This project is open source and available for educational purposes.

👨‍💻 Author

Yash Dharmik


GitHub: @YashDharmik278
Repository: StudentsGradeTrackerSystem


📞 Support

For issues, questions, or suggestions, please open an issue on the GitHub repository.


🎓 Learning Outcomes

This project demonstrates:


Object-Oriented Programming (OOP) principles
ArrayLists and dynamic data structures
User input handling and validation
Statistical calculations
Report generation
Code organization and best practices
Exception handling
Menu-driven application design
