# attendence-check
# Attendance Certificate Allocation System

This Python project automates attendance calculation from multiple Zoom attendance CSV reports. It processes daily attendance files, combines session durations for students who joined multiple times, and calculates overall attendance percentages.

## Features

* Reads multiple attendance CSV files from a folder.
* Merges rejoined session durations for each student.
* Excludes host entries from attendance calculations.
* Marks a student as present if their total attendance duration is at least 90 minutes for a session.
* Calculates attendance percentage across all sessions.
* Automatically determines certificate eligibility:

  * **Allocated**: Attendance ≥ 80%
  * **Not Allocated**: Attendance < 80%
* Generates a sorted summary report (`attendance_summary.csv`).

## Technologies Used

* Python
* Pandas
* OS Module

## Output

The script generates an `attendance_summary.csv` file containing:

* Student Name
* Present Days
* Total Days
* Attendance Percentage
* Certificate Status

This project helps automate attendance tracking and certificate allocation for online classes, workshops, webinars, and training programs.
