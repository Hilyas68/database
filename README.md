# database Queries
This contain 5 SQL queries 

#First Query

SELECT * FROM Lecturers_Info ORDER BY LecturerFirstName;

#Second Query

UPDATE Lecturers_Info SET LecturerFirstName='Alfred', LecturerLastName='Schmidt'
WHERE Lecturer_id = 2;

#Third Query

DELETE FROM Courses WHERE CourseTitle='Introduction to Version Control' AND CourseUnit=3;

#Fourth Query

SELECT Departments.DepartmentNames, Courses.CourseName, Lecturers_Info.LecturerFirstName
FROM Departments
INNER JOIN Courses
ON Departments.Department_id = Courses.Department_id;