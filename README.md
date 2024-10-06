<img width="132" alt="logo" src="https://github.com/user-attachments/assets/c0641cf3-4421-49be-b3db-c7f82cba3a97">
# Automation Exercise API Testing

## 0. What are we testing and what is this about?
This project consists of automated API tests for the Automation Exercise website. The tests cover various functionalities such as user account creation, product search, and user account deletion. The goal is to ensure that the API endpoints work correctly and respond with the expected results.

## 1. Requirements
- Postman for testing API endpoints.
- GitHub for version control.
- Newman (optional) for running Postman collections in the command line.

## 2. How to install
1. **Clone the repository:**
   - Go to your GitHub repository and copy the clone URL.
   - Use the following command in your terminal or Git Bash:
     ```bash
     git clone <repository-url>
     ```

2. **Install Newman (optional):**
   - If you want to run the tests using Newman, install it via npm:
     ```bash
     npm install -g newman
     ```

## 3. How to run tests
1. **Using Postman:**
   - Open the Postman application.
   - Import the Postman collection and environment provided in the repository.
   - Run the collection to execute all tests.

2. **Using Newman:**
   - Navigate to the directory containing your Postman collection and run:
     ```bash
     newman run <collection-file.json>
     ```

## 4. Any issues with tests or website?
- If you encounter issues with the tests failing, ensure that the expected response codes and messages are correct according to the API documentation.
- Common issues may include:
  - User already exists when trying to create an account.
  - Invalid credentials during login tests.
  - Deletion tests failing if the account does not exist.

## Screenshots
*Insert any relevant screenshots here to demonstrate successful test runs or errors encountered during testing.*

---

### API Tests Included:
1. **API 11: POST To Create/Register User Account**
   - **Endpoint:** `https://automationexercise.com/api/createAccount`
   - **Method:** POST
   - **Parameters:** name, email, password, title, birth_date, birth_month, birth_year, firstname, lastname, company, address1, country, zipcode, state, city, mobile_number
   - **Expected Response:** 201 User created!

2. **API 12: DELETE METHOD To Delete User Account**
   - **Endpoint:** `https://automationexercise.com/api/deleteAccount`
   - **Method:** DELETE
   - **Parameters:** email, password
   - **Expected Response:** 200 Account deleted!

*Feel free to add more API tests as necessary.*
