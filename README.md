

# Bank Management System

A simple Python-based bank management application with a Streamlit web interface.

The project demonstrates basic banking operations such as account creation, deposits, withdrawals, viewing account details, updating user information, and account deletion. Account data is stored locally in a JSON file.

## Features

- Create a new bank account
- Validate minimum account age and four-digit PIN
- Automatically generate account numbers
- Deposit money into an account
- Withdraw money from an account
- Check account details
- Update name, email, and PIN
- Delete an account
- Store data locally in `data.json`
- Streamlit-based web interface
- Command-line implementation included in `main.py`

## Project Structure

```text
Bank_Management_System/
├── app.py       # Streamlit web application
├── hello.py     # Bank management logic
├── main.py      # Command-line version
├── data.json    # Local account database
└── README.md    # Project documentation
```

## Technologies Used

- Python
- Streamlit
- JSON
- pathlib
- random
- string

## Installation

Clone the repository:

```bash
git clone https://github.com/RAHUL8687/Bank_Management_System.git
cd Bank_Management_System
```

Install Streamlit:

```bash
pip install streamlit
```

## Run the Web Application

Start the Streamlit application using:

```bash
streamlit run app.py
```

After running the command, open the local URL shown in the terminal.

## Run the Command-Line Version

The project also contains a command-line version:

```bash
python main.py
```

## Available Operations

### Create Account

Users provide:

- Name
- Age
- Email
- Four-digit PIN

The application generates an account number and creates an account with an initial balance of zero.

### Deposit Money

Users enter their account number, PIN, and deposit amount. Deposits are limited to a maximum of 10,000 per transaction.

### Withdraw Money

Users can withdraw money if their account has sufficient balance.

### Show Account Details

Users can view their account information by entering their account number and PIN.

### Update Account Information

Users can update:

- Name
- Email
- PIN

Age, account number, and balance cannot be changed through the update operation.

### Delete Account

Users can delete their account after providing the correct account number and PIN.

## Data Storage

Account information is stored in:

```text
data.json
```

Example account structure:

```json
{
    "name": "Example User",
    "age": 25,
    "email": "example@email.com",
    "pin": 1234,
    "accountNo.": "Ab1@2Cd",
    "balance": 0
}
```

## Security Notice

This project is intended for educational purposes only.

- PINs are stored as plain text.
- Account data is stored in a local JSON file.
- There is no database authentication system.
- There is no encryption or transaction audit log.
- Do not use real banking information or passwords.

For production use, the project should use encrypted credentials, a secure database, authentication controls, input validation, logging, and proper authorization.

## Future Improvements

- Hash and securely store PINs
- Replace JSON storage with SQLite or PostgreSQL
- Add transaction history
- Add user authentication and session management
- Add email and input validation
- Prevent duplicate account numbers
- Add automated tests
- Add an administrator dashboard
- Add database backup and recovery
- Improve error handling and form validation

## License

No license has currently been specified for this project.
