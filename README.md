# Lab 5: Static Code Analysis — Hotel Booking System

## 1. Project Overview

This project focuses on improving the code quality, security, and maintainability of a Python-based Hotel Booking System using static code analysis tools.

The purpose of this lab is to identify potential programming errors, insecure coding practices, and code-style violations, fix the identified issues, and rerun the analysis tools to verify the improvements.

## 2. About the Program

The Hotel Booking System manages hotel room reservations and inventory. The original program is analyzed and improved while preserving its intended functionality.

## 3. Objectives

- Identify code-quality issues and potential programming errors.
- Detect common security vulnerabilities.
- Improve Python coding style and readability.
- Fix at least four identified issues.
- Verify the changes by rerunning the static analysis tools.

## 4. Tools Used

### Pylint
Pylint checks Python code quality, naming conventions, unused variables, programming practices, and potential errors.

### Bandit
Bandit scans Python source code for common security issues and potentially unsafe coding patterns.

### Flake8
Flake8 checks Python code style, formatting, whitespace, and compliance with PEP 8 guidelines.

## 5. Issues Identified and Fixes

The following are examples of issues to document when they are confirmed in the original source code:

- Mutable default arguments.
- Overly broad exception handling.
- Unsafe use of `eval()`.
- Weak hashing algorithms.
- Insecure random-number generation.
- Unnecessary shell command execution.
- Unused imports and variables.
- File-handling and encoding improvements.

Refer to `issues.md` for the verified issue table, including descriptions and fix approaches.

## 6. Installation

Ensure Python is installed, then install the required tools:

```bash
python -m pip install pylint bandit flake8
```

## 7. How to Run the Program

Run the Hotel Booking System:

```bash
python hotel_booking_system.py
```

Follow any prompts displayed by the program.

## 8. Static Code Analysis

Run Pylint and save its output:

```bash
python -m pylint hotel_booking_system.py > pylint_report.txt
```

Run Bandit and save its output:

```bash
python -m bandit -r hotel_booking_system.py > bandit_report.txt
```

Run Flake8 and save its output:

```bash
python -m flake8 hotel_booking_system.py > flake8_report.txt
```

Review the generated reports to identify remaining issues.

## 9. Results

The final results should be recorded based on the actual reports generated after fixing the code.

- **Pylint:** Check the final code-quality score in `pylint_report.txt`.
- **Bandit:** Review the security findings in `bandit_report.txt`.
- **Flake8:** Review any style violations in `flake8_report.txt`.

An empty Flake8 report generally means that no violations were reported for the analyzed file.

## 10. Project Deliverables

| File | Description |
|---|---|
| `hotel_booking_system.py` | Updated Python program |
| `issues.md` | Documented issues and fixes |
| `reflection.md` | Reflection answers |
| `pylint_report.txt` | Pylint analysis output |
| `bandit_report.txt` | Bandit analysis output |
| `flake8_report.txt` | Flake8 analysis output |
| `README.md` | Project documentation |

## 11. Conclusion

This lab demonstrates how static code analysis can help identify programming issues, improve code readability, and detect potential security weaknesses. Fixing the identified issues and rerunning the tools helps verify improvements and supports the development of more maintainable Python software.
