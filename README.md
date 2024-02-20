<h1>Bank Management System</h1>

Welcome to the Bank Management System project repository! This collaborative effort aims to provide a comprehensive solution for managing banking operations efficiently. We've successfully implemented both the front-end and back-end components, with a focus on user-friendly interfaces and robust backend functionality.

<h3>Technologies Used</h3>
Frontend: Angular, TypeScript, HTML, Tailwind CSS
Backend: Spring Boot, Java, Spring Data JPA, Maven, JAVA JDK 17, REST API.
Database: Oracle

<h3>Getting Started</h3>
* Clone the repository.
* Refresh maven file.
* Set up the property: Edit and enter your database username password. 
* Run the application: The API should now be running at localhost.
* Set up the frontend: Follow the instructions in the frontend/README.md file.

<h3>Endpoints</h3>

Sign Up:

Endpoint: POST '/customer/signup'
Description: Register a new customer.
Request Body: Customer object.

Login:

Endpoint: POST '/customer/login'
Description: Authenticate a customer.
Request Body: CustomerWrapper object containing username and password.

Get All Customers:

Endpoint: GET '/customer/get'
Description: Retrieve a list of all customers.

Get Customer by Username:

Endpoint: GET '/customer/get/{username}'
Description: Retrieve a customer by their username.
Path Variable: username

Check Username Availability:

Endpoint: GET '/customer/{username}'
Description: Check if a username is available.
Path Variable: username

Get All Transactions:

Endpoint: GET '/customer/gettransactions'
Description: Retrieve a list of all transactions.

Get Transactions by Username:

Endpoint: GET '/customer/transactions/{username}'
Description: Retrieve transactions for a specific customer.
Path Variable: username

Save Transaction:

Endpoint: POST '/customer/transactions/{username}'
Description: Save a new transaction for a customer.
Path Variable: username
Request Body: Transaction object.
Bill Payment:

Endpoint: PUT '/customer/billpayment/{username}'
Description: Process a bill payment for a customer.
Path Variable: username
Request Parameters: amount, billerWrapper (as request body).

Delete Customer:

Endpoint: DELETE '/customer/delete/{username}'
Description: Delete a customer.
Path Variable: username

Deposit:

Endpoint: PUT '/customer/deposit'
Description: Deposit funds into a customer's account.
Request Parameters: username, amount

Withdraw:

Endpoint: PUT '/customer/withdraw'
Description: Withdraw funds from a customer's account.
Request Parameters: username, amount

Update Customer Password:

Endpoint: PUT '/customer/updateCustomerPassword'
Description: Update a customer's password.
Request Parameters: username
Request Body: Map containing currentPassword and newPassword.

Fund Transfer:

Endpoint: PUT '/customer/fundTransfer'
Description: Transfer funds between customer accounts.
Request Parameters: senderUsername, receiverAccountNo, amount

<h1>Thank You</h1>
