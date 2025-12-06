# Dmoney API Testing with Postman
This project contains comprehensive API test cases for the Dmoney REST API using Postman.

## 📋 Project Overview

This test suite validates the complete transaction flow of the Dmoney application including:
- User management (Admin, Agent, Customer, Merchant)
- Transaction operations (Deposit, Send Money, Withdraw, Payment)
- Balance inquiries and transaction statements

## 🔗 API Documentation

**Postman Documentation Link:** [View Complete API Documentation](https://documenter.getpostman.com/view/YOUR-LINK-HERE)

## 📊 Test Coverage

### Test Scenarios (15+ Test Cases)

1. **TC01** - Admin Login & Authentication
2. **TC02** - Create Agent Account
3. **TC03** - Create Customer 1 Account
4. **TC04** - Create Customer 2 Account
5. **TC05** - Create Merchant Account
6. **TC06** - Deposit from SYSTEM to Agent (5000 TK)
7. **TC07** - Agent Deposits to Customer 1 (2000 TK)
8. **TC08** - Check Agent Balance
9. **TC09** - Send Money from Customer 1 to Customer 2 (500 TK)
10. **TC10** - Withdraw from Customer 1 to Agent (100 TK)
11. **TC11** - Check Customer 1 Balance
12. **TC12** - Get Transaction Details by Transaction ID
13. **TC13** - Payment from Customer 2 to Merchant (300 TK)
14. **TC14** - Check Customer 2 Balance
15. **TC15** - Get Customer 2 Transaction Statement
16. **TC16** - Check Merchant Balance

## 🚀 Getting Started

### Prerequisites
- [Postman](https://www.postman.com/downloads/) installed
- Dmoney API access credentials

### Installation Steps

1. **Import Collection**
   - Download the collection file from this repository
   - Open Postman
   - Click Import → Upload Files
   - Select `Dmoney_API_Testing.postman_collection.json`

2. **Import Environment**
   - Import `Dmoney_Environment.postman_environment.json`
   - Select the environment from dropdown (top right)

3. **Configure Environment Variables**
```
   baseUrl: [Your API Base URL]
   adminEmail: admin@dmoney.com
   adminPassword: 1234
```

4. **Run Tests**
   - Click on Collection → Run
   - Execute tests in sequence

## 📁 Repository Structure
```
dmoney-api-testing/
│
├── README.md
├── Dmoney_API_Testing.postman_collection.json
├── Dmoney_Environment.postman_environment.json
├── TestCases.xlsx (Detailed test case documentation)
└── screenshots/
    ├── test-execution.png
    └── test-results.png
```

## 🧪 Test Execution

### Running Individual Tests
1. Select a request from the collection
2. Click "Send"
3. View test results in "Test Results" tab

### Running Complete Suite
1. Click collection name → "Run"
2. Select all requests
3. Click "Run Dmoney API Testing"
4. View consolidated report

## ✅ Test Results

- **Total Test Cases:** 16
- **Pass Rate:** 100%
- **Execution Time:** ~2 minutes

*Screenshot of test execution:*

![Test Results](screenshots/test-results.png)

## 📝 Test Case Documentation

Detailed test cases are available in `TestCases.xlsx` with the following format:
- Test Case ID
- Test Case Name
- Priority
- Preconditions
- Test Steps
- Expected Results
- Test Data

## 🛠️ Technology Stack

- **API Testing Tool:** Postman
- **Authentication:** JWT Bearer Token
- **Data Format:** JSON
- **Assertions:** Chai Assertion Library

## 👤 Test Credentials
```
Admin:
Email: admin@dmoney.com
Password: 1234

System Account: SYSTEM
Transaction Range: 10 TK - 10,000 TK
```

## 📞 API Endpoints Tested

- `POST /user/login` - User authentication
- `POST /user/create` - Create new users
- `POST /transaction/deposit` - Deposit money
- `POST /transaction/sendmoney` - Send money between users
- `POST /transaction/withdraw` - Withdraw money
- `POST /transaction/payment` - Make payment
- `GET /transaction/balance/{account}` - Check balance
- `GET /transaction/search/{trnxId}` - Get transaction details
- `GET /transaction/statement/{account}` - Get transaction statement

## 🤝 Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License

This project is created for educational/testing purposes.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your Profile](https://linkedin.com/in/yourprofile)

## 📧 Contact

For any queries, please reach out to: your.email@example.com

---

**Note:** This is a test project. Please use test credentials and avoid using production data.
