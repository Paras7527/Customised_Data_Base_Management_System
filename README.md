# Customised DBMS Documentation 💻

## Introduction
The "Customised DBMS" is a custom database management system implemented in Java. It is designed to manage employee records, offering functionalities such as inserting, viewing, updating, and deleting data. Additionally, it provides aggregate operations like calculating the count, sum, average, maximum, and minimum of employee salaries.

---

## Features
1. **Insert Records:** Add new employee data to the database.
2. **View Records:**
   - Display all employee records.
   - Display specific records by ID or name.
3. **Delete Records:**
   - Delete a record by name or ID.
4. **Update Records:** Modify the address of an employee by ID.
5. **Aggregate Operations:**
   - Count the number of records.
   - Calculate the total, average, maximum, and minimum salaries.
6. **Database Management:**
   - Clear all records.
   - Terminate the database session.

---

## Class Descriptions
### 1. **Employee**
This class represents an employee entity with the following attributes:
- `Eno`: Employee number (auto-incremented).
- `Ename`: Name of the employee.
- `Eage`: Age of the employee.
- `Eaddress`: Address of the employee.
- `Esalary`: Salary of the employee.

**Methods:**
- **Constructor:** Initializes employee details and assigns a unique ID.
- **DisplayInformation():** Prints the employee's details.

### 2. **CustomisedDBMS**
This class manages the database operations.

**Attributes:**
- `lobj`: A linked list to store employee objects.

**Methods:**
- `InsertIntoTable(String name, int age, String address, int salary)`: Adds a new employee record.
- `SelectStarFrom()`: Displays all records.
- `SelectSpecific(int id)`: Displays a specific record by ID.
- `SelectSpecific(String name)`: Displays a specific record by name.
- `DeleteData(int id)`: Deletes a record by ID.
- `DeleteData(String name)`: Deletes a record by name.
- `AggregateCount()`: Counts the total number of records.
- `AggregateSum()`: Calculates the sum of all salaries.
- `AggregateAvg()`: Calculates the average salary.
- `AggregateMax()`: Finds the highest salary.
- `AggregateMin()`: Finds the lowest salary.
- `UpdateRecord(int id, String address)`: Updates the address of an employee by ID.
- **Destructor:** Clears all resources when the database is terminated.

## Usage Instructions
1. **Run the Program:**
   Compile and execute the `program570.java` file.

   ```
   javac program570.java
   java program570
   ```

2. **Select Options:**
   Use the menu displayed to perform desired operations. For example:
   - Enter `1` to insert a new record.
   - Enter `2` to display all records.
   - Enter `13` to terminate the DBMS session.

---

## Example Commands
**1. Insert a Record:**
```
Option: 1
Enter the name of the employee: John
Enter the age of the employee: 30
Enter the salary of the employee: 50000
Enter the address of the employee: New York
```

**2. View All Records:**
```
Option: 2
Output:
----------------------------------------------------------------
No	 Name 	 Address 	 Age 	 Salary 
----------------------------------------------------------------
1	John	New York		  30	50000
----------------------------------------------------------------
```

**3. Delete a Record by Name:**
```
Option: 5
Enter the employee name that you want to delete: John
```

---

## Notes
- Ensure the Java Development Kit (JDK) is installed on your system to compile and run the program.
- The system assigns unique IDs to employees automatically.
- Aggregate operations work on numeric salary data only.

---

## Future Enhancements
- Implementing data persistence to store records in a file or database.
- Adding support for searching and filtering records with multiple criteria.
- Enhancing the user interface with a graphical front end.

---

## Conclusion
The Customised DBMS provides a basic yet robust system for managing employee records, demonstrating fundamental database operations using Java. It can be extended further for more advanced features and real-world applications.

