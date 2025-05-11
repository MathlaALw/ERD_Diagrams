# Normalization Practice

[Normalization Practice File](./PDF/Normalization-Task5.pdf)


## Case1: Company system – UNF table

![## Case1: Company system – UNF table
](./images/case1-CompanySystem.PNG)


### 1NF 
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

### 2NF
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


------------------------------
