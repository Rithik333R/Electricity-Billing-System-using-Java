# Electricity-Billing-System-using-Java



# Electricity Billing System

This Java-based **Electricity Billing System** is a GUI application developed using **Java Swing**. It allows users to manage electricity billing operations efficiently and securely. The system supports multiple functionalities such as customer management, bill generation, and payment tracking.

## Features

1. **User Authentication**  
   - Secure login system for user access with personalized credentials.

2. **Customer Management**  
   - Add new customers and manage their details.
   
3. **Bill Calculation**  
   - Calculate electricity bills based on customer usage and applicable rates.

4. **Bill Payment**  
   - Record and track payments for electricity bills.

5. **Bill Generation**  
   - Generate detailed bills for customers.

## Project Overview

This Java application was developed using **IntelliJ IDEA**. It integrates with a MySQL database through **JDBC (Java Database Connectivity)** to manage customer and billing information. The project is divided into multiple classes, each handling different aspects of the system to create a smooth user experience.

### Key Classes:

- **SplashScreen**: Displays the initial loading screen.
- **LoginScreen**: Handles user authentication.
- **MainSystem**: The main interface where users can access various features.
- **AddCustomer**: Allows users to add new customers.
- **PayBill**: Manages the payment process for bills.
- **GenerateBill**: Generates bills for customers.
- **ShowDetails**: Displays customer and bill details.
- **LastBill**: Shows the details of the last bill.
- **ConnectionSetup (JDBC)**: Manages the database connection and queries.

## Database Structure

The MySQL database used in the system consists of the following tables:

- **Login Table**: Stores usernames and passwords for secure login.
  - Columns: `UserName`, `Password`

- **Bill Table**: Contains details of the electricity bills.
  - Columns: `MeterNumber`, `Units`, `Month`, `Amount`

- **Emp Table**: Stores information about employees and customers.
  - Columns: `Name`, `MeterNumber`, `Address`, `State`, `City`, `Email`, `Phone`

- **Tax Table**: Stores tax and rent details.
  - Columns: `MeterLocation`, `MeterType`, `PhaseCode`, `BillType`, `Days`, `MeterRent`, `MCB_Rent`, `ServiceRent`, `GST`

### Database Connectivity
Java communicates with the MySQL database using **JDBC** to fetch and manipulate data, ensuring seamless interaction between the application and the database.

## Screenshots

### 1. **Login Screen**  
![Login](https://github.com/Rithik333R/Electricity_Billing_System/blob/master/ScreenShots/Login.JPG)  
*User login interface for secure access.*

### 2. **Main System Interface**  
![Main System](https://github.com/Rithik333R/Electricity_Billing_System/blob/master/ScreenShots/Main.JPG)  
*Main system interface with access to all features.*

### 3. **Add Customer**  
![Add Customer](https://github.com/Rithik333R/Electricity_Billing_System/blob/master/ScreenShots/AddC.JPG)  
*Add new customer details.*

### 4. **Calculate Bill**  
![Calculate Bill](https://github.com/Rithik333R/Electricity_Billing_System/blob/master/ScreenShots/CalculateBill.JPG)  
*Calculate the electricity bill based on usage.*

### 5. **Customer Details**  
![Details](https://github.com/Rithik333R/Electricity_Billing_System/blob/master/ScreenShots/Details.JPG)  
*Display customer and billing details.*

### 6. **Generate Bill**  
![Generate Bill](https://github.com/Rithik333R/Electricity_Billing_System/blob/master/ScreenShots/GenerateBill.JPG)  
*Generate and print bills for customers.*

## Setup Instructions

### Prerequisites:
- **Java JDK** (Java Development Kit)
- **MySQL Database** with the provided schema and tables

### Steps to Run:
1. Clone this repository to your local machine.
 
2. Set up the MySQL database and import the schema provided in the project.

3. Configure the **ConnectionSetup** class to connect to your MySQL database (provide your database credentials).

4. Open the project in **IntelliJ IDEA** (or your preferred Java IDE) and run the application.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
