<img width="132" alt="logo" src="https://github.com/user-attachments/assets/c0641cf3-4421-49be-b3db-c7f82cba3a97">

# Automated Testing with Postman

## Welcome!

This project focuses on testing different functionalities of the **Automation Exercise Website** through comprehensive API testing using **Postman**. Additionally, the project includes continuous integration (CI) with **GitHub Actions**.

### 14 Scenarios Tested:
- **API 1**: Get All Products List
- **API 2**: POST To All Products List
- **API 3**: Get All Brands List
- **API 4**: PUT To All Brands List
- **API 5**: POST To Search Product
- **API 6**: POST To Search Product without search_product parameter
- **API 7**: POST To Verify Login with valid details
- **API 8**: POST To Verify Login without email parameter
- **API 9**: DELETE To Verify Login
- **API 10**: POST To Verify Login with invalid details
- **API 11**: POST To Create/Register User Account
- **API 12**: DELETE METHOD To Delete User Account
- **API 13**: PUT METHOD To Update User Account
- **API 14**: GET user account detail by email

## Prerequisites
Before you begin, ensure you have the following installed on your machine:
- Node.js.
- npm (Node Package Manager): Comes with Node.js installation.
- Postman for testing API requests.

## Set up
1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Install dependencies: `npm install`.

## Testing
Test scenarios are available in `automation-exercise.postman_collection.json`, and you can run them using Postman.

### Importing Postman Collection
1. From this repository, download `automation-exercise.postman_collection.json` file to your local machine.
2. In Postman, click on the "Import" button located at the top left and drop `automation-exercise.postman_collection.json` file.
3. Postman will automatically add the collection, and you will see all predefined API requests.

### Running Tests with Newman
1. Open terminal window and execute the test script: `npm run test`.

## CI Integration with GitHub Actions
This project includes a GitHub Actions workflow that automatically runs the tests each time the main branch is updated.

### GitHub Actions Workflow
The CI process is defined in the `.github/workflows/main.yml` file.

## How to View Test Results
Test results can be viewed in the "Actions" tab of your GitHub repository. Each workflow run will show the logs of the test execution, including any failures or errors encountered during the test runs.

