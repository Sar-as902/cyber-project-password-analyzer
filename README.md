# Password Strength Analyzer & Custom Wordlist Generator

## Project Overview

The **Password Strength Analyzer & Custom Wordlist Generator** is a Python-based cybersecurity project that helps users evaluate password security and generate customized wordlists for ethical security testing. The project is designed for cybersecurity students, ethical hackers, and penetration testers who want to understand password strength and practice password auditing in a safe environment.

The Password Strength Analyzer checks the complexity of a password using the **zxcvbn** library and calculates password entropy. It provides a detailed security report, including password length, character distribution, estimated crack time, and recommendations for creating stronger passwords.

The Custom Wordlist Generator creates targeted wordlists using personal information such as a person's name, important date, and pet name. It generates multiple password combinations using leetspeak substitutions and common number patterns, making it useful for educational password-cracking demonstrations in authorized environments.

---

# Objectives

- Analyze password strength using modern password evaluation techniques.
- Calculate password entropy to estimate randomness.
- Display password statistics and security suggestions.
- Generate custom wordlists using personal information.
- Save generated reports and wordlists for future analysis.
- Provide an easy-to-use command-line interface for cybersecurity learning.

---

# Technologies Used

- **Programming Language:** Python 3
- **Library:** zxcvbn
- **Modules Used:**
  - argparse
  - itertools
  - math
  - string
  - os

---

# Project Structure

```
password-analyzer/
│
├── analyzer.py          # Password strength analysis
├── generator.py         # Custom wordlist generator
├── main.py              # Main program
├── utils.py             # Report saving utility
├── requirements.txt     # Required Python packages
├── output/
│   ├── report.txt
│   └── custom_wordlist.txt
└── README.md
```

---

# Features

## 1. Password Strength Analyzer

The analyzer performs the following tasks:

- Calculates password strength score (0–4)
- Calculates password entropy
- Counts uppercase letters
- Counts lowercase letters
- Counts digits
- Counts special characters
- Estimates offline password cracking time
- Provides security recommendations
- Saves password analysis report

---

## 2. Custom Wordlist Generator

The generator creates intelligent password lists using:

- Person's name
- Important dates
- Pet name
- Leetspeak substitutions
- Common years
- Numeric patterns
- Symbol combinations

Generated wordlists are stored in the **output** folder.

---

# Installation

## Step 1

Create Virtual Environment

```bash
python -m venv venv
```

## Step 2

Activate Virtual Environment

Windows

```bash
venv\Scripts\activate
```

Linux/Mac

```bash
source venv/bin/activate
```

## Step 3

Install Required Packages

```bash
pip install -r requirements.txt
```

---

# Running the Project

## Analyze Password

```bash
python main.py --password "MyPassword123!"
```

## Save Analysis Report

```bash
python main.py --password "MyPassword123!" --save
```

## Generate Custom Wordlist

```bash
python main.py --generate --name "Alice" --date "1999" --pet "Tommy"
```

---

# Sample Output

Password Analysis

```
Password Length : 14
Strength Score  : 4/4
Entropy         : 91.74 bits
Estimated Guesses : 125000000000
Offline Crack Time : centuries
Uppercase Letters : 2
Lowercase Letters : 8
Digits : 3
Symbols : 1
```

Wordlist Generation

```
Generated 1450 words.
Saved to output/custom_wordlist.txt
```

---

# Output Files

After execution, the project generates:

```
output/
│
├── report.txt
└── custom_wordlist.txt
```

- **report.txt** contains password analysis results.
- **custom_wordlist.txt** contains generated password combinations.

---

# Applications

- Cybersecurity education
- Ethical hacking laboratories
- Password auditing
- Security awareness training
- Penetration testing practice
- Password policy evaluation

---

# Advantages

- Simple and lightweight
- Easy to understand
- Fast password analysis
- Entropy calculation
- User-friendly command-line interface
- Automatically generates targeted wordlists
- Saves reports for future reference

---

# Limitations

- Command-line interface only
- Requires Python installation
- Uses limited personal information for wordlist generation
- Intended only for authorized educational and ethical security testing

---

# Future Enhancements

- Graphical User Interface (GUI)
- Password history checking
- Dictionary attack simulation
- Export reports in PDF format
- Support for additional password policies
- Integration with cybersecurity tools
- Dark mode interface
- Real-time password strength visualization

---

# Conclusion

The **Password Strength Analyzer & Custom Wordlist Generator** is a practical cybersecurity project that demonstrates password security analysis and customized wordlist generation. It helps users understand the importance of creating strong passwords while providing hands-on experience with password auditing concepts. The project serves as an excellent learning tool for students and beginners in cybersecurity and ethical hacking.
