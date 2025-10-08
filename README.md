# ICT1222 Mini Project - Student Management System

## Overview
This repository contains the database schema and sample data for the ICT1222 Mini Project, a student management system designed to handle student records, course enrollments, attendance, assessments, and eligibility tracking for the University of Ruhuna. The system supports a minimum of 10 proper students, 5 repeat students, 5 lecturers, 5 technical officers, 1 dean, and 1 admin, as per the project requirements. The database is designed to manage the Level 1 Semester 2 courses for the 2024/2025 academic year, with data current as of October 08, 2025.

## Features
- **Student Management**: Tracks student details, including proper and repeat students, with batch assignments (2020-2024).
- **Course and Session Management**: Manages course details, session schedules, and attendance for 15 weeks per course.
- **Assessment Tracking**: Records continuous assessment (CA) marks (e.g., Quiz, Assessment) and final exam marks.
- **Attendance Monitoring**: Provides attendance summaries for each student per course.
- **Eligibility Assessment**: Determines student eligibility based on attendance, CA, and final marks.
- **Views**: Includes pre-defined SQL views for attendance, CA marks, final marks, overall performance, and eligibility.

## Database Schema
The database consists of the following tables:

### Tables
- **User**: Base table for all roles (students, lecturers, etc.) with personal details.
- **Student**: Subtype of User, with `registration_no` and `status` (proper/repeat).
- **Lecturer**: Subtype of User, with teaching assignments.
- **TechnicalOfficer**: Subtype of User, with lab roles.
- **Dean**: Subtype of User, with departmental leadership.
- **Admin**: Subtype of User, with administrative access.
- **Department**: Stores department details (e.g., ICT, ET).
- **Course**: Defines courses with theory/practical components and lecturer assignments.
- **AssessmentComponent**: Defines assessment types (e.g., Quiz, Final_Theory) with weights.
- **Mark**: Stores individual student marks per assessment component.
- **Session**: Schedules theory and practical sessions over 15 weeks.
- **Attendance**: Tracks student attendance status per session.
- **Batch**: Manages student batches (2020-2024).
- **Enrollment**: Links students to courses and batches.
- **ExamSchedule**: Schedules exams for assessment components.

### Prerequisites
- MySQL or a compatible relational database management system.
- Basic knowledge of SQL for querying and managing the database.

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Book-Store-Mini-Project/DBMS-GROUP-01.git
   