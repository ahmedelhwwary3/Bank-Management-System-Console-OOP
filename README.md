# 🏦 Bank Management System – C++ Console Application (OOP Design)

A clean, modular, and fully object-oriented C++ console application that simulates core banking operations without relying on external libraries or databases.

---

## 📌 Features

### 🔐 User Management

* Add, Edit, Delete, and Search Users
* Case-insensitive username handling
* Authentication with account lockout after 3 failed attempts
* Bitwise permission system using `byte` flags
* Role-based screen authorization through inheritance
* Login activity tracking

### 👥 Client Management

* Add, Edit, Delete, and Search Clients
* Display all clients in tabular format
* File-based persistence using text files

### 💰 Banking Transactions

* Deposit and Withdraw funds
* Transfer money between accounts
* View balances for individual or all clients
* Transaction history per client

### 💱 Currency Conversion

* Manage currencies and exchange rates
* Convert between any two currencies using updated rates

---

## 🏗 Architecture

```text
SimpleBank
├── Core
│   ├── clsUser.cpp / .h
│   ├── clsClient.cpp / .h
│   ├── clsCurrency.cpp / .h
│   └── clsBankClient.cpp / .h
│
├── Screens
│   ├── MainMenu.cpp
│   ├── LoginScreen.cpp
│   └── BankTransactionScreens/
│
├── Helpers
│   ├── clsString.cpp / .h
│   ├── clsInputValidate.cpp / .h
│   └── clsDate.cpp / .h
│
├── Globals
│   └── GlobalVars.cpp / .h
│
├── Data
│   └── Text files for users, clients, and currencies
│
└── main.cpp
```

---

## ⚙️ Technical Highlights

* Full OOP design using classes, inheritance, and encapsulation
* Self-implemented utility classes for strings, validation, and date handling
* File-based persistence using `fstream`
* Custom `split()` and `join()` implementations
* Bitwise permission management using masks
* Reusable screen framework through inheritance
* DRY-oriented implementation with reusable helper classes
* Clean, readable, and maintainable codebase

---

## 🔧 Tools Used

* C++
* STL
* fstream
* g++ / MSVC

---

## 📝 How to Run

1. Clone the repository.

2. Compile the project:

```bash
g++ -std=c++17 -o SimpleBankApp *.cpp
```

3. Run the application:

```bash
./SimpleBankApp
```

4. Follow the on-screen menus.

---
