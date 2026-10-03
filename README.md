# Employee Management System

**An Employee Management System is a software application used by organizations to manage their employee data. It helps to keep track of employee information such as their personal details, job position, salary, and other related data. It is designed to streamline HR operations and automate administrative tasks related to employees.**\
\
**You** have to build a basic employee management system using python which should perform the following functions -

1. **Add Employee**\
   In this, employee details can be added. The details will include the **ID,** **Name, Age, Gender, Job Position** and **salary**. Also a check will be applied to ensure uniqueness of the **Employee ID.**
2. **Update Employee**\
   In this, employee detail can be updated using **employee id**\

3. **Delete Employee**\
   In this, An employee can be deleted using the **employee ID.**
4. **List Employee**\
   In this,  List of all the employees will be shown to the user in tabular format.
5. **Exit**\
   **Now at the end your program will ask the user to exit from the program.** <br>

**These options will be provided to the user each and every time the user performs an operation successfully such as addition or deletion of the employee.** \
This program doesn't to be a **GUI** application, it will be simple console based and will not involve the use of database and database applications such as MY SQL, SQL Server, etc.\
\
Here are some Examples:


**----Employee Management System-----**

1. **Add Employee**
2. **Update Employee**
3. **Delete Employee**
4. **List Employees**
5. **Exit**&#x20;

**Enter your choice:** 1


{tab title="Add Employee" }
**Enter Employee Details:**

**ID**: 101 \
**Name:** Mohan \
**Age:** 20 \
**Gender:** Male \
**Position:** Manager \
**Salary:** 100000 \
**Employee added successfully.**


{ tab title="Update Details" }
**Enter the Employee ID**

**ID: 101** \
Which Information you want to update :

1. Name
2. Age
3. Gender
4. Position
5. Salary \
   **Enter Your choice :** 3 \
   **Gender : Male** \
   **Enter the Gender :** Female \
   **Employee Details updated Successfully**
   { endtab }

{ tab title="Delete Employee" }
Enter Employee ID: \
ID: 101 \
Employee deleted successfully

<summary>Code Explanation</summary>

The above code starts from the while loop and that is the user view means first time the user interacts with the options provided there.

On choosing the options user is asked for the necessary details to be added.

A list `employees = []` has been declared globally to add employees with their details in the form of **dictionary**. It is declared globally so that it is available throughout the program.

`add_employee()` function is defined to add the employee which takes the employee id from the user and checks whether any user with the ID provided exists or not. If yes then a message is displayed that user already exist otherwise the details are added in the form of **dictionary in the list employees\[] declared globally**

`update_employee()` function updates the employee details by taking the user id and finds the employee with that employee id and displays a submenu to the user asking which detail user want to update. Each option shows its old value and asks for the new value from the user.

`delete_employee()` function deleted the employee on the basis of employee ID.

`list_employees()`function displays list of all the employees in the tabular format.

Inside these functions on few places **return** is used to return the control to the while loop if the employee is found and the necessary operation is performed successfully. If the employee is not found then this **return** statement will not be executed as the control will not come inside the if block then **a message&#x20;*****Employee not found*****&#x20;is displayed to the user.**
