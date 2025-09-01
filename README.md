# ATM

# 🏦 Online Net Banking App

This is a simple **command-line based Net Banking application** built in Python. It simulates basic banking operations such as checking balance, withdrawing money, depositing funds, transferring money between accounts, and logging out.

---

## 📂 Project Structure

```
app.py   # Main script containing the entire banking system



## 🚀 Features

1. **User Login System**

   * Users must log in using their **account number** and **password**.
   * Validates credentials from the `accounts` dictionary.

2. **Banking Operations**
   After successful login, users can perform the following:

   * **Balance Inquiry** → Check current account balance.
   * **Withdraw** → Withdraw money if sufficient funds exist.
   * **Deposit** → Deposit money into account.
   * **Transfer** → Transfer money to another valid account.
   * **History (Mini Statement)** → Placeholder (not fully developed).
   * **Logout** → End session safely.

3. **Data Simulation**

   * Accounts and balances are **stored in dictionaries**:

     * `accounts` → Stores account number and password.
     * `user_details` → Stores name, balance, and email.

---

## 🛠️ Requirements

* Python **3.6+**

No external libraries are required – everything uses **standard Python**.

---

## ▶️ How to Run

1. Clone/download the repository.
2. Run the Python file:

```bash
python app.py
```

3. Enter your **account number** and **password**.
   Example login:

   ```
   Account Number: 12345
   Password: 6789
   ```

---

## 📖 Example Usage

### 🔑 Login

```text
Welcome to the Codegnan Online net banking app
Please enter your account number: 12345
Please enter your password: 6789
Successfully logedin to codegnan online netbanking
```

### 📋 Menu Options

After login, you’ll see:

```
1. Balence
2. Withdraw
3. Deposite
4. Transfer
5. History
6. Logout
```

### 💰 Sample Transactions

* **Check Balance**

  ```
  Current balance is 1000
  ```

* **Withdraw**

  ```
  Please enter your withdraw amount: 200
  Successfully withdraw your amount 200
  Current Balance is 800
  ```

* **Deposit**

  ```
  Please enter your deposit amount: 500
  Current balance is 1300
  ```

* **Transfer**

  ```
  Please enter your receiver account number: 12346
  Please enter your transfer amount: 300
  Current Balance is 1000
  ```

* **Logout**

  ```
  User successfully logout
  


## 🧩 Code Overview

* **`login(user_name, password)`** → Handles user authentication.
* **`balance(user_name)`** → Displays user balance.
* **`withdraw(user_name, withdraw_amount)`** → Deducts funds if sufficient balance exists.
* **`deposit(user_name, deposit_amount)`** → Adds funds to the account.
* **`transfer(user_name, to_account, transfer_amount)`** → Moves funds between accounts.
* **`history(user_name)`** → Placeholder for mini statement.
* **`logout()`** → Ends the session.


## ⚠️ Limitations

* No **database support** – accounts are stored in Python dictionaries.
* No **transaction history** yet (just a placeholder).
* Passwords are stored in plain text (for demo purposes only).
* Input validation is basic.


## 📌 Future Enhancements

* Add **transaction history** with timestamps.
* Improve **password security** (e.g., hashing).
* Store account data in **SQLite / PostgreSQL database**.
* Build a **GUI / Web interface**.


✅ This project is a **beginner-friendly banking system simulation**, helpful for learning Python fundamentals such as functions, loops, conditionals, and dictionaries.

Would you like me to also **add a usage diagram (flowchart of how the app works)** in the README for better understanding?
