🔐 Encrypted File Protection & Recovery System

(Educational Project – Linux Only)

📌 Project Overview

This project is an educational simulation of file encryption and decryption using Python and Fernet symmetric cryptography.
It demonstrates how files can be encrypted and later recovered using a secret key and authentication phrase.

⚠️ Important Note:

This project is created strictly for educational and learning purposes.

It is intended to be executed only on Linux-based systems (Ubuntu, Kali Linux, Parrot OS, etc.).

Running this project on Windows may trigger antivirus or security software.

🖥️ Supported Platform

✅ Linux (Ubuntu / Kali / Parrot / Debian-based)

❌ Windows (not recommended)

❌ macOS (not tested)

⚙️ Requirements
Software Requirements

Python 3.x

pip (Python package manager)

Git

Linux Terminal

Python Dependency

cryptography library (Fernet)

Install dependency using:

pip3 install cryptography

📂 Project Structure
encrypted-file-project/
│
├── encrypt.py        # Encrypts files in the directory
├── decrypt.py        # Decrypts files using secret phrase
├── README.md         # Project documentation
├── .gitignore        # Excludes sensitive files


⚠️ The encryption key file (thekey.key) is generated at runtime and is intentionally excluded from GitHub using .gitignore.

🚀 How to Use (Step-by-Step Guide)
🔹 Step 1: Clone the Repository

Open terminal and run:

git clone https://github.com/USERNAME/encrypted-file-project.git


Navigate into the project directory:

cd encrypted-file-project

🔹 Step 2: Create Test Files (IMPORTANT)

Create 2–3 dummy files for testing:

echo "This is test file 1" > file1.txt
echo "This is test file 2" > file2.txt
echo "This is test file 3" > file3.txt


Check files:

ls

🔹 Step 3: Run Encryption Script

Execute:

python3 encrypt.py


✔️ This will:

Generate an encryption key (thekey.key)

Encrypt all files in the directory except the scripts

Make the files unreadable

🔹 Step 4: Run Decryption Script

Execute:

python3 decrypt.py


You will be prompted:

Enter secret phrase:


Enter:

coffee


✔️ If the phrase is correct:

All files will be decrypted

Original content will be restored

❌ If wrong phrase is entered:

Files will remain encrypted

🔑 Authentication Details

Secret Phrase: coffee

Used as a basic authentication mechanism before decryption

Demonstrates access control in encryption systems

🛡️ Security & Best Practices

The encryption key file is not pushed to GitHub

.gitignore is used to exclude sensitive runtime files

Designed to work only inside a controlled test directory

No system files are modified

🧪 Educational Concepts Covered

File-level encryption & decryption

Symmetric cryptography (Fernet)

Key generation & management

Authentication logic

Linux file handling

Git & GitHub version control

⚠️ Disclaimer

This project is intended only for educational and academic purposes.
Do not use this project on real user data or production systems.
The author is not responsible for misuse of this code.

✅ Conclusion

This project provides hands-on experience with encryption concepts, secure coding practices, and Linux-based execution. It also demonstrates how version control and documentation are handled professionally in real-world software projects.
