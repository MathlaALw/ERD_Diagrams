# Normalization Report


## Case1: Company system – UNF table

![## Case1: Company system – UNF table
](./images/case1-CompanySystem.PNG)


### 1NF  -> Removing the repeating groups ( multivalued attributes )
#### Employee Table
|EmployeeID   | EmployeeName  |  Department | Manager       |
|-------------|---------------|-------------|-------------- |
|E001         | Ahmed         | IT          | Eng. Khalid   |
|E002         | Salim         | HR          | Ms. Amal      |
|E003         | Aisha         | IT          | Eng. Khalid   |
#### Project Table
|ProjectID    | ProjectName     |EmployeeID   |
|-------------|---------------  |-------------|
|P101         | Website         | E001        |
|P102         | MobileApp       | E001        |
|P103         | Recruitment     | E002        |
|P102         | Mobile App      | E003        |
|P104         | Database Upgrade| E003        |

-> divide the projects column into two column ProjectID and ProjectName .

### 2NF -> Removing the partial dependencies
#### Employee Table
|EmployeeID   | EmployeeName  |  Department | Manager       |
|-------------|---------------|-------------|-------------- |
|E001         | Ahmed         | IT          | Eng. Khalid  |
|E002         | Salim         | HR          | Ms. Amal     |
|E003         | Aisha         | IT          | Eng. Khalid  |

#### Project Table
|ProjectID    | ProjectName     |
|-------------|---------------  |
|P101         | Website         | 
|P102         | MobileApp       |
|P103         | Recruitment     | 
|P102         | Mobile App      | 
|P104         | Database Upgrade| 

#### Employee_Project Table
|EmployeeID   | ProjectID     |
|-------------|---------------|
|E001         | P101          |
|E001         | P102          |
|E002         | P103          |
|E003         | P102          |
|E003         | P104          |

-> divide the Employee table into two tables Employee and Project table.
and create a new table Employee_Project to store the relationship between Employee and Project tables.

------------------------------



