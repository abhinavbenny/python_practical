# Python Practical 10 – Unit Testing, Logging and Code Quality

**Course:** MCA Semester I – Python Programming  
**Platform:** macOS  
**Project:** Order Processing System

## 1. Project Description

This practical demonstrates important Python software development practices, including Unit Testing, Logging, and Code Quality.

The project uses `pytest` for testing Python functions, Python's built-in `logging` module for recording application events, and `Ruff` for identifying code-quality issues and formatting Python code.

## 2. Objectives

- Write unit tests using pytest.
- Test valid and invalid inputs.
- Handle expected exceptions using `pytest.raises()`.
- Implement logging using Python's logging module.
- Understand different logging levels.
- Identify and fix code-quality issues using Ruff.
- Maintain readable and properly formatted Python code.

## 3. Technologies Used

- Python 3
- pytest
- Ruff
- Python Logging Module
- VS Code / macOS Terminal
- Git and GitHub

## 4. Project Structure

```text
practical10/
│
├── order.py
├── test_order.py
├── logging_demo.py
├── bad_code.py
├── application.log
├── screenshots/
│   ├── test_results.png
│   ├── ruff_check.png
│   └── ruff_format.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

**Note:** The `.venv` virtual environment is excluded from GitHub.

## 5. macOS Setup Instructions

### Step 1: Check Python Installation

```bash
python3 --version
```

### Step 2: Clone the Repository

```bash
git clone https://github.com/abhinavbenny/python_practical.git
```

### Step 3: Navigate to the Project

```bash
cd python_practical
```

### Step 4: Create a Virtual Environment

```bash
python3 -m venv .venv
```

### Step 5: Activate the Virtual Environment

```bash
source .venv/bin/activate
```

### Step 6: Install Dependencies

```bash
python -m pip install -r requirements.txt
```

## 6. Execution Instructions

### A. Run the Order Processing Program

```bash
python order.py
```

This program calculates discounts, GST, and the final order amount.

### B. Run Unit Tests

```bash
python -m pytest -v
```

The test suite checks:

- Discount calculation.
- GST calculation.
- Final order calculation.
- Zero discount.
- Negative price validation.
- Invalid discount validation.

### C. Run the Logging Program

```bash
python logging_demo.py
```

View the generated log file:

```bash
cat application.log
```

### D. Run Ruff Code Quality Checks

Check code quality:

```bash
python -m ruff check .
```

Check formatting:

```bash
python -m ruff format --check .
```

## 7. Logging Levels

| Level | Description |
|---|---|
| DEBUG | Detailed debugging information |
| INFO | Normal application events |
| WARNING | Unexpected situations |
| ERROR | An operation has failed |
| CRITICAL | Serious application failures |

## 8. Testing and Code Quality Results

The project includes unit tests to verify the correctness of functions and validation of invalid inputs.

The following checks are performed:

- pytest test execution.
- Ruff linting checks.
- Ruff formatting checks.

Screenshots of the actual terminal results are available in the `screenshots/` folder.

## 9. Expected Order Calculation

For an order of ₹1,000 with a 10% discount and 18% GST:

| Description | Amount |
|---|---:|
| Original Price | ₹1,000 |
| Discount (10%) | ₹100 |
| Discounted Price | ₹900 |
| GST (18%) | ₹162 |
| **Final Amount** | **₹1,062** |

## 10. Learning Outcomes

Through this practical, I learned:

- How to write and execute unit tests using pytest.
- How to validate inputs and handle exceptions.
- How to implement logging in Python applications.
- How to use Ruff for code-quality checking and formatting.
- How to organize a Python project.
- How to use Git and GitHub for project submission.

## 11. Author

**Name:** Abhinav Benny  
**Course:** MCA Semester I  
**Practical:** 10 – Python Programming

---

**End of Practical 10**
