
# 🏦 Bank System Console App (C++ OOP Project)

A clean, modular, and fully object-oriented C++ console application that simulates core functionalities of a simple banking system — entirely built without using any external libraries.

---

## 📌 Features

### 🔐 User Management
- Add / Edit / Delete / Search Users
- Case-insensitive username handling
- Login system with maximum 3 failed attempts
- Bitwise permission system using `byte` flags
- Role-based screen access via inheritance
- Login activity reports

### 👥 Client Management
- Add / Edit / Delete / Search clients
- Display all clients in table view
- Store data in text files (no database)

### 💰 Bank Transactions
- Deposit / Withdraw / Transfer between accounts
- View balance for individual or all clients
- Transaction history per client

### 💱 Currency Conversion
- Manage currencies and update exchange rates
- Calculate conversion between any two currencies using updated rates

---

## 📂 Project Structure

```
/SimpleBank
├── Core
│   ├── clsUser.cpp / .h
│   ├── clsClient.cpp / .h
│   ├── clsCurrency.cpp / .h
│   └── clsBankClient.cpp / .h
├── Screens
│   ├── MainMenu.cpp
│   ├── LoginScreen.cpp
│   └── BankTransactionScreens/
├── Globals
│   └── GlobalVars.cpp / .h (e.g., CurrentUser)
├── Helpers
│   ├── clsString.cpp / .h
│   ├── clsInputValidate.cpp / .h
│   └── clsDate.cpp / .h
├── Data
│   └── Text files to store users, clients, currencies
└── main.cpp
```

---

## ⚙️ Technical Highlights

- Full OOP design using classes, inheritance, and encapsulation
- All utility functions (e.g., string manipulation, validation, date parsing) are self-implemented
- File-based persistence using `fstream`
- Custom `split()` and `join()` logic with flexible separators
- Bitwise operations for permissions (`bit & mask`)
- Consistent screen layout and interface by inheriting from a base screen class
- Clean and readable codebase (no code repetition)

---

## 🔧 Tools Used

- Language: C++
- Compiler: Any standard C++ compiler (g++, MSVC)
- Platform: Windows / Linux Terminal

---

## 📝 How to Run

1. Clone the repository.
2. Compile using your C++ compiler:
   ```bash
   g++ -std=c++17 -o SimpleBankApp *.cpp
   ./SimpleBankApp
   ```
3. Follow the on-screen menu.

---

## 📣 Author

Developed with care and precision by [Ahmed Elhwwary].  
Feel free to contribute, suggest features, or report bugs.
---

## ✅ Future Enhancements (Optional)

- Add transaction logs
- Enhance UI with ncurses (Linux) or WinAPI (Windows)
- Encrypt stored passwords
- Add export to CSV or JSON

Telegram Channel For Projects:
https://t.me/ahmedelhwwary3

