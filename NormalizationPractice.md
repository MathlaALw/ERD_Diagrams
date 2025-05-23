﻿# Normalization Practice

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


## Case2: University System – UNF Table 

![## Case2: University System – UNF Table](./images/Case2-UniversitySystem.PNG)


### 1NF

#### Student Table
|StudentID    | StudentName   |  Department  |Advisor       |
|-------------|---------------|--------------|--------------|
|S001         | Reem          | CS           | Dr. Omar     |
|S002         | Tariq         | Business     | Dr. Sarah    |
|S003         | Noura         | CS           | Dr. Omar     |



#### Course Table
|CourseCode   | CourseName    |  
|-------------|---------------|
|C101         | DB            |
|C102         | AI            |
|C103         | Marketing     |
|C104         | Networking    |


### 2NF
#### Student Table
|StudentID    | StudentName   |  Department  |Advisor       |
|-------------|---------------|--------------|--------------|
|S001         | Reem          | CS           | Dr. Omar     |
|S002         | Tariq         | Business     | Dr. Sarah    |
|S003         | Noura         | CS           | Dr. Omar     |

#### Course Table
|CourseCode   | CourseName    |
|-------------|---------------|
|C101         | DB            |
|C102         | AI            |
|C103         | Marketing     |
|C104         | Networking    |

#### Student_Course Table
|StudentID    | CourseCode    |
|-------------|---------------|
|S001         | C101          |
|S001         | C102          |
|S002         | C103          |
|S003         | C101          |
|S003         | C104          |


------------------------------

## Case3: Airline System – UNF Table

![## Case3: Airline System – UNF Table](./images/Case3-AirlineSystem.PNG)


### 1NF
#### Booking Table
|BookingID    | PassengerName |PaymentMethod   |
|-------------|---------------|----------------|
|B001         | Salem         | Credit Card    |
|B002         | Fatma         | PayPal         |
|B003         | Zayed         | Cridit Card    |

#### Flight Table
|BookingID     | FlightNumber  | From    | To       |
|-------------|---------------|-------   |-------   |
|B001         | F101          | Muscat   | Dubai    |
|B001         | F102          | Dubai    | London   |
|B002         | F103          | Muscat   | Istanbul |
|B003         | F104          | Istanbul | Paris    |
|B003         | F105          | Paris    | Oslo     |

#### Passenger Table
|BookingID    | FlightID      | SeatNumbers|
|-------------|---------------|------------|
|B001         | F101          | 12A        |
|B001         | F102          | 14B        |
|B002         | F103          | 10B        |
|B003         | F104          | 9A         |
|B003         | F105          | 13A        |

### 2NF
#### Booking Table
|BookingID    | PassengerName |PaymentMethod   |
|-------------|---------------|----------------|
|B001         | Salem         | Credit Card    |
|B002         | Fatma         | PayPal         |
|B003         | Zayed         | Cridit Card    |
#### Flight Table
|FlightID     | FlightNumber  | From     | To       |SeatNumbers|
|-------------|---------------|-------   |-------   |------------|
|F101         | F101          | Muscat   | Dubai    | 12A        |
|F102         | F102          | Dubai    | London   | 14B        |
|F103         | F103          | Muscat   | Istanbul | 10B        |
|F104         | F104          | Istanbul | Paris    | 9A         |
|F105         | F105          | Paris    | Oslo     | 13A        |

### Passenger Table
|BookingID    | FlightID      | 
|-------------|---------------|
|B001         | F101          |
|B001         | F102          |
|B002         | F103          |
|B003         | F104          |
|B003         | F105          |


------------------------------
