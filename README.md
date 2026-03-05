# Baseball Team Manager – Midterm Project

CPRO 2201 – Python Programming II  
Winter 2026 – Red Deer Polytechnic  

## Project Overview

This project is based on the Baseball Case Study from Murach’s Python Programming book.  
The purpose of the program is to manage a baseball team lineup using a CSV file.

The program allows the user to:

- Display the lineup
- Add a player
- Remove a player
- Move a player
- Edit player position
- Edit player stats
- Calculate batting average automatically

The project was developed in three stages as required by the instructor.

---

## Section 1 – Procedural Version

In Section 1, I implemented the program using a procedural approach.

Features:

- Player data stored using a list of lists
- Valid positions stored in a tuple
- Batting average calculated as hits ÷ at bats
- Batting average displayed to 3 decimal places
- Input validation (no negative numbers, hits cannot exceed at bats)
- Handles missing CSV file
- First names only displayed in lineup (as shown in specification)

---

## Section 2 – Improved Procedural Version

In Section 2, I improved the program structure and formatting.

Enhancements:

- Each player stored as a dictionary
- Separator lines created using repetition operator ("=" * 64)
- Current date displayed in YYYY-MM-DD format
- Program prompts for game date
- Displays number of days until game (if game date is in the future)
- Improved formatting and alignment
- Continued use of CSV file for data storage

---

## Section 3 – Object-Oriented Version

In Section 3, I converted the program to an object-oriented design.

The program now includes:

### Player Class
- Stores first name, last name, position, at bats, and hits
- Provides a full_name property
- Provides a batting_average property
- Validates position and statistics
- Ensures hits cannot be greater than at bats

### Lineup Class
- Stores Player objects
- Allows adding, removing, and moving players
- Implements __len__() and __iter__()
- Separates business logic from user interface

### Layered Structure
- main.py → program control
- ui.py → user interface
- objects.py → business logic
- db.py → file handling (CSV read/write)

The functionality remains the same, but the structure is cleaner and more maintainable.

---

## How to Run

Navigate to the desired section folder and run:

python main.py

Example:

cd section3_oop
python main.py

---

## Notes

- The same players.csv file is used across all sections.
- GitHub commit history shows development from procedural to object-oriented version.
- The program follows the midterm project specifications.