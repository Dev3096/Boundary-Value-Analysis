*********************************************************** PROBLEM DESCRIPTION *******************************************************************************************

Grader Component
The Grader component is a software implementation designed to automatically compute grades for a course. 
This README provides an overview of the problem statement and outlines the approach to be taken for Boundary-Value Testing.

Problem Statement
The course consists of two exams (Exam-1 and Exam-2) and a project. The passing criteria for the course are as follows:

Grade C: A student must score at least 45 points in Exam-1, 50 points in Exam-2, and 50 points in the Project.
Grade B: A student must score at least 60 points in Exam-1, 55 points in Exam-2, and 60 points in the Project. Additionally, the average of the exams must be at least 80 points.
Grade A: A student must fulfill the requirements for Grade B and score at least 70 points in the Project.
The final grades for the course are categorized as A, B, C, or E (indicating failure).

Input Parameters
The Grader component accepts the following inputs:

Last name: The last name of the student (maximum 20 characters).
First name: The first name of the student (maximum 15 characters).
Student #: A 9-character string in the format "AXXXXXXXX", where X represents a digit.
Exam-1: An integer representing the score for Exam-1 (0 to 90).
Exam-2: An integer representing the score for Exam-2 (0 to 100).
Project: An integer representing the score for the Project (0 to 80).
Assumptions
The following assumptions are made for the Grader component:

Exam-1, Exam-2, and Project scores are represented as integers.
The score ranges for exams are:
0 ≤ Exam-1 ≤ 90
0 ≤ Exam-2 ≤ 100
0 ≤ Project ≤ 80
The maximum size for the "First name" field is 15 characters, and for the "Last name" field is 20 characters.
Student # is a 9-character string in the format "AXXXXXXXX", where X represents a digit.
Sample Test Case
Here is a sample test case for the Grader component:

Test #1:

Last name: Smith
First name: John
Student #: A11112222
Exam-1: 57
Exam-2: 64
Project: 75
Design
For the purpose of Boundary-Value Testing, the following test cases will be considered:

Normal Boundary-Value Analysis Test Cases: Test cases that examine the behavior of the system at the boundaries of the input ranges, such as minimum and maximum values.
Robust Boundary Value Test Cases: Test cases that test the system's behavior beyond the boundaries, checking for potential issues or unexpected behavior.
These test cases will help ensure that the Grader component functions correctly and handles input values within the specified ranges.

Please refer to the code implementation for the specific test cases and their expected results.

Implementation
The implementation of the Grader component, along with the test cases, can be found in the provided code files.

Thank you for using the Grader component. For any inquiries or assistance, please contact the development team.

** BOUNDARY VALUE ANALYSIS ** 

Boundary Value Analysis (BVA) is a software testing technique used to identify errors and defects at the boundaries of input or output conditions. 
It focuses on testing the values that lie at the edges or boundaries of input domains, as these values are more likely to cause issues.

The principle behind BVA is that errors often occur at the boundaries due to the way the software handles these values. 
By testing the boundary values, we can uncover defects related to input validation, data range checking, and other boundary-related issues.

BVA involves selecting test cases that represent the minimum, maximum, and just beyond the boundaries of valid input ranges. 
It typically involves three categories of values:

1. Valid Boundary Values: These are the values at the lower and upper boundaries of the input domain. 
   For example, if an input field accepts values between 1 and 100, valid boundary values would be 1 and 100.

2. Invalid Boundary Values: These are values just outside the valid input range. 
   For example, if the valid input range is 1 to 100, invalid boundary values would be 0 and 101.

3. Special or Extreme Boundary Values: These are values that may cause different behavior in the software.
   They are typically the minimum or maximum possible values for a given input field.
   For example, if an input field accepts numbers up to 100, an extreme boundary value could be a very large number like 10^9.

By testing these boundary values, we can uncover defects such as off-by-one errors, incorrect handling of minimum and maximum values, truncation issues, and other boundary-related problems.

Boundary Value Analysis helps improve the efficiency and effectiveness of testing by focusing on critical areas where defects are more likely to occur. 
It complements other testing techniques and provides insights into the behavior of the software at the edges of its operational limits.

Overall, Boundary Value Analysis is a valuable technique to enhance test coverage and identify potential issues related to input boundaries in software applications.
