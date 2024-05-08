Introduction
This README provides an overview of the DataBase design used for the Guvi Zen Class. The DataBase is designed to manage student, instructor, course, enrollment, class schedule, and payment information within the educational context of Guvi Zen Class.

Database Overview:
Students Table
student_id (Primary Key)
first_name
last_name
email
phone_number
date_of_birth
address
guardian_name
guardian_contact
Instructors Table
instructor_id (Primary Key)
first_name
last_name
email
phone_number
Courses Table
course_id (Primary Key)
course_name
description
start_date
end_date
instructor_id (Foreign Key references Instructors)
Enrollments Table
enrollment_id (Primary Key)
student_id (Foreign Key references Students)
course_id (Foreign Key references Courses)
enrollment_date
ClassSchedule Table
schedule_id (Primary Key)
course_id (Foreign Key references Courses)
day_of_week
start_time
end_time
room_location
Payments Table
payment_id (Primary Key)
student_id (Foreign Key references Students)
course_id (Foreign Key references Courses)
payment_date
amount
payment_method
Usage
This DataBase is integral to the Guvi Zen Class, facilitating the storage and management of student enrollment, instructor information, course details, class schedules, and payments.
