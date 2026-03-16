# AI Assessment Question Structure Controller

## Project Overview

The **AI Assessment Question Structure Controller** is a core module of the **AI Assessment Monitoring System**.
It ensures that every AI assessment follows a **fixed and validated question structure** before it is delivered to candidates.

This module guarantees fairness, consistency, and proper question sequencing across all domains such as **AI/ML, Web Development, Data Science**, and others.

---

## Objective

The goal of this module is to enforce a **standard structure for AI assessments** so that:

* Every candidate receives **exactly 10 questions**
* The **question format remains consistent**
* Difficulty levels increase gradually
* Duplicate or missing questions are prevented

This ensures a **fair and structured evaluation process**.

---

## Assessment Rules

The controller validates the following rules:

1. Each assessment must contain **exactly 10 questions**

2. The **first question must always be**:

   **"Please introduce yourself."**

3. The remaining **9 questions are domain-specific**

4. Questions must follow **increasing difficulty levels**

5. Duplicate questions are **not allowed**

6. Missing questions are **not allowed**

If any of these rules are violated, the assessment will be **rejected by the controller**.

---

## How the System Works

1. The system receives a list of questions.
2. The controller validates the question structure.
3. It checks:

   * Total number of questions
   * First question rule
   * Duplicate questions
   * Difficulty order
4. If validation passes, the assessment is approved.
5. If validation fails, an error message is returned.

---

## Project Structure

```
ai-assessment-monitoring-controller
│
├── controller
│   └── assessment_controller.py
│
├── tests
│   └── test_controller.py
│
└── README.md
```

### controller/

Contains the main validation logic for the AI assessment question structure.

### tests/

Contains unit tests used to verify that the controller works correctly.

---

## Running the Project

Make sure **Python 3** is installed.

### Step 1: Open Terminal

Navigate to the project folder.

### Step 2: Run Unit Tests

```bash
python -m unittest discover tests
```

---

## Expected Output

If all validations work correctly, you will see:

```
.....
----------------------------------------------------------------------
Ran 5 tests

OK
```

This confirms that the controller correctly validates the assessment structure.

---

## Technologies Used

* Python 3
* JSON-style data structures
* Python `unittest` framework

---

## Use Case

This controller can be integrated into:

* AI Interview Platforms
* Online Technical Assessments
* Automated Recruitment Systems
* AI Monitoring & Evaluation Systems

---

## Author

**Chithranjan Agapu**

AI Assessment Monitoring System
Internship Project – Assessment Question Structure Controller
