# Bug Fixing Using Cursor AI

## 📌 Project Overview

This project demonstrates how Cursor AI can assist in identifying, understanding, and fixing bugs in Python code. It focuses on debugging a student utility module and verifying the corrections using Python's built-in `unittest` framework.

The project helps develop practical debugging skills by analyzing test failures, identifying logical errors, applying fixes, and checking whether the corrected code behaves as expected.

## 🎯 Objectives

- Identify logical errors in Python functions.
- Understand why unit tests fail.
- Use Cursor AI to assist with debugging and code correction.
- Implement fixes while maintaining the intended program functionality.
- Verify corrected code using automated unit tests.

## 🛠️ Technologies Used

- **Python** — Programming language.
- **Cursor AI** — AI-assisted coding and debugging.
- **unittest** — Python's built-in unit testing framework.
- **Google Colab** — Environment used to execute Python code and tests.
- **Git and GitHub** — Version control and project hosting.

## 📂 Project Structure

```text
bug-fixing-using-cursor-ai/
│
├── student_utils.py
├── test_student_utils.py
└── README.md
```

## ⚙️ Features

### 1. Calculate Average

Calculates the average of a list of student marks.

### 2. Check Passing Status

Checks whether a student's mark meets the passing threshold of 40.

### 3. Assign Grades

Assigns grades according to the following criteria:

| Average Marks | Grade |
|---|---|
| 90 and above | Distinction |
| 60–89 | First |
| 45–59 | Second |
| Below 45 | Fail |

## 🐛 Bugs Identified and Fixed

- **Incorrect pass-mark condition:** Using `>` instead of `>=` incorrectly classified a score of exactly 40 as failing.
- **Unit-test execution in Google Colab:** The default `unittest.main()` can interpret notebook-specific arguments as test-runner arguments. Passing an explicit `argv` avoids this issue.
- **Indentation errors:** Inconsistent indentation can prevent Python from executing the test code.

## 🧪 Testing

The project includes eight unit tests covering:

1. Average of three marks.
2. Average of a single mark.
3. Marks above the passing threshold.
4. Marks exactly at the passing threshold.
5. Marks below the passing threshold.
6. Distinction grade.
7. First grade.
8. Second and Fail grades.

Run the tests locally using:

```bash
python -m unittest -v test_student_utils.py
```

A successful run should report that all eight tests pass, provided the implementation matches the expected behavior.

## 🚀 Getting Started

### Prerequisites

- Python 3 installed.
- Git installed (for cloning the repository).

### Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/bug-fixing-using-cursor-ai.git
```

Navigate to the project directory:

```bash
cd bug-fixing-using-cursor-ai
```

Run the unit tests:

```bash
python -m unittest -v test_student_utils.py
```

Replace `YOUR-USERNAME` with your GitHub username.

## 📚 Learning Outcomes

- Improved understanding of Python debugging.
- Experience with automated testing.
- Ability to interpret test failures and error messages.
- Practical use of AI-assisted development tools.
- Better understanding of code correctness and boundary conditions.

## 🤖 Role of Cursor AI

Cursor AI is used as a debugging assistant to help analyze error messages, locate potential bugs, understand their causes, and suggest corrections. The proposed fixes should be reviewed and validated through testing rather than accepted without verification.

## 👨‍💻 Conclusion

This project demonstrates a simple, test-driven approach to debugging Python programs with AI assistance. It highlights the importance of understanding the root cause of an error, applying an appropriate fix, and verifying the result through automated tests.

---

**Project Name:** Bug Fixing Using Cursor AI  
**Language:** Python  
**Testing Framework:** unittest
