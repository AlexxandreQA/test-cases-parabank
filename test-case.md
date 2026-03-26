## CT-001 — Login with valid credentials

**Precondition:**
User must be registered and active in the system.

**Test Data:**
Username: qa.squad@test.com
Password: Squad@2026

**Steps:**
1. Access the login page
2. Enter valid username
3. Enter valid password
4. Click on "Log In"

**Expected Result:**
User is redirected to "Accounts Overview" page with account balance visible.

## CT - 002 - Creating a new savings account at Parabank

**Precondition:**
Create a second account on the website, provided you already have an existing account and a minimum balance of 90 euros.

**Test Data:**
New account creation

**Steps:**
1) Access parabank.parasoft.com/parabank/login.htm
2) Enter username: qa.squad@test.com
3) Enter password: Squad@2026
4) Click the 'open new account' button
5) Select the “checking” option

**Expected Result:**
The message “Account Opened” appears along with the new savings account number.

**Status**
Passed
   
## CT - 003 - Transfer of 50 euros from current account to savings account at Parabank

**Precondition:**
A current account and a savings account must already exist.

**Test Data:**
Transfer of funds

**Steps:**
1) Access parabank.parasoft.com/parabank/login.htm
2) Enter username: qa.squad@test.com
3) Enter password: Squad@2026
4) Click the 'Transfer Funds' button
5) Add the amount of 50 euros
6) Select the "debited" and "received" accounts
7) Click 'transfer'

**Expected Result:**
The message “Transfer Complete” appears with the amount and account debited and account received.

**Status**
✅ Passed


## CT - 004 - Transfer of an amount exceeding the existing balance of the checking account to the savings account is permitted, provided the balance is not negative.

**Precondition:**
There is already a current account with a balance of 360 euros.

**Test Data:**
Value Transfer to a Larger

**Steps:**
1) Access parabank.parasoft.com/parabank/login.htm
2) Enter username: qa.squad@test.com
3) Enter password: Squad@2026
4) Click the 'Transfer Funds' button
5) Add the amount of 400 euros
6) Select the "debited" and "received" accounts
7) Click 'transfer'

**Expected Result:**
The message "Transfer denied" indicates that there are insufficient funds for the transaction.

**Status**
It didn't go through; the message was that the transfer was completed. The balance remains negative.






