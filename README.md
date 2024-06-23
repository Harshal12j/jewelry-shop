Jewelry Shop Management System
This is a JavaFX-based desktop application for managing customer information in a jewelry shop. The application allows users to create new customer records, search for existing customers, and view detailed information about each customer and calculate the customers interest on lending amount in exchange of mortgage Jewelry.

Table of Contents
Features
Requirements
Installation
Usage
Project Structure
Contributing
License
Features
Create Customer: Add new customers with details such as full name, mobile number, address, Aadhar card number, amount borrowed, date of borrowing, picture, digital signature, interest rate, type of ornament, and calculated interest.
Search Customer: Search for existing customers by full name.
Customer List: View a list of all customers.
Customer Details: View detailed information about a selected customer.
Requirements
Java 11 or higher
Maven
JavaFX SDK
Apache HTTPClient
Gson
Installation
Clone the repository:

sh
Copy code
git clone https://github.com/yourusername/jewelry-shop-management.git
cd jewelry-shop-management
Install dependencies:

Ensure you have Maven installed. Run the following command to install the required dependencies:

sh
Copy code
mvn clean install
Set up JavaFX:

Download the JavaFX SDK from Gluon and configure the PATH_TO_FX environment variable to point to the JavaFX SDK lib directory.

Usage
Run the application:

You can run the application using Maven:

sh
Copy code
mvn javafx:run
Main Window:

When the application starts, the main window will appear where you can:

Create a new customer by filling in the required fields and clicking the "Save" button.
Search for an existing customer by entering the full name in the search bar and clicking the "Search" button.
List all customers by clicking the "List All Customers" button.
Customer List Window:

If you search for a customer or list all customers, the customer list window will appear displaying the results. Click on a customer in the list to view their details.

Customer Details Window:

When you click on a customer in the customer list, the customer details window will appear showing all the information about the selected customer.

Project Structure
bash
Copy code
src/
├── main/
│   ├── java/
│   │   └── com/jewelry_shop/
│   │       ├── MainApp.java
│   │       ├── controller/
│   │       │   ├── MainWindowController.java
│   │       │   ├── CustomerListController.java
│   │       │   └── CustomerDetailsController.java
│   │       ├── model/
│   │       │   └── Customer.java
│   │       └── service/
│   │           └── CustomerService.java
│   ├── resources/
│   │   ├── fxml/
│   │   │   ├── MainWindow.fxml
│   │   │   ├── CustomerList.fxml
│   │   │   └── CustomerDetails.fxml
│   │   └── styles/
│   │       └── main.css
│   └── META-INF/
│       └── MANIFEST.MF
└── test/
    └── java/
        └── com/jewelry_shop/
            └── controller/
                └── MainWindowControllerTest.java
Contributing
Contributions are welcome! Please follow these steps:

Fork the repository.
Create a new branch: git checkout -b feature/your-feature-name.
Make your changes and commit them: git commit -m 'Add new feature'.
Push to the branch: git push origin feature/your-feature-name.
Open a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for more details.

