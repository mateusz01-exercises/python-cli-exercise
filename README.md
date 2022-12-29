# Python CLI Exercise v1
Your task will be to create **CLI** (Command Line Interface) application for **company employees management**.

## Functionalities
1. Saving employee data to the file.
2. Reading list of all employees data from file and displaying to the user.
3. Reading one employee data by first and last name (eg. "John Doe") from file and displaying to the user.
4. Reading total number of employees by processing information from the file and displaying to the user.
5. Reading total wages (sum of salaries) of all the employees by processing information from the file and displaying to the user.
6. Reading average employee age (rounded to the two decimal places, eg. "44.35") by processing information from the file and displaying to the user.
7. Reading employees names by excluding duplicates and displaying to the user.
8. Reading occurrence count of each employee name by processing information from the file and displaying to the user.
9. Exiting app.

## Requirements:
- Employee data should be kept in **space separated** format:
    ```
    first_name last_name age salary
    ```
    Example:
    ```
    John Doe 28 4000
    Anna Merry 35 8000
    ```
- When user starts app, the initial screen should look like this:
    ```
    COMPANY EMPLOYEES MANAGEMENT
    1. Save employee data to the file.
    2. Show list of all the employees data.
    3. Show employee data by name and lastname.
    4. Show total number of employees.
    5. Show total wages.
    6. Show average employee age.
    7. Show distinct employees names.
    8. Show occurence count of each employee name.
    9. Exit app.

    Provide option number: [you need to gather user input here]
    ```
- User chooses functionality by providing associated number.
- Application must work in a loop until user explicitly states that app should be closed by choosing option number 9.
- After concluding functionality associated with a given number, it should display initial screen again:
    ```
    COMPANY EMPLOYEES MANAGEMENT
    1. Save employee data to the file.
    2. Show list of all the employees data.
    3. Show employee data by name and lastname.
    4. Show total number of employees.
    5. Show total wages.
    6. Show average employee age.
    7. Show distinct employees names.
    8. Show occurence count of each employee name.
    9. Exit app.

    Provide option number: 1 [user provided option number 1]

    Provide name: [you need to gather user input here]
    Provide lastname: [you need to gather user input here]
    Provide age: [you need to gather user input here]
    Provide salary: [you need to gather user input here]

    User successfully saved.

    COMPANY EMPLOYEES MANAGEMENT
    1. Save employee data to the file.
    2. Show list of all the employees data.
    3. Show employee data by name and lastname.
    4. Show total number of employees.
    5. Show total wages.
    6. Show average employee age.
    7. Show distinct employees names.
    8. Show occurence count of each employee name.
    9. Exit app.

    Provide option number: [you need to gather user input here]
    ```

## Assumptions
- You can assume that file already exists in directory from where application script is being run. You can assume it is named "employees_data.txt" (remember to create this file manually before running app)
- You can assume that each employee data record is just a list of 4 elements when processing file data in your application (you do not need to use objects and classes)

## Tips
- What kind of loop would be the best for exiting only if stated explicitly (also - is it possible to run loop infinitely and is this observation beneficial in case of our app)?
- How to round number to the custom decimal point - maybe string has some nice formatting methods?
- How to display only distinct employees names - is there a structure that disallows duplicates?
- How to display occurence count of each employee name - is there a structure that allows association of string with a number?
