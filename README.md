# ai-assessment-question-controller
AI Assessment Question Structure Controller - Internship Task
Description

This module manages the structure and validation of AI assessment questions used in an interview monitoring system.

It ensures that questions follow a defined format before being stored or used in assessments.

Project Features

• Question structure validation
• AI assessment question controller
• JSON based question handling
• Input validation rules
• Sample output generation

Project Structure
controllers/
Handles question request processing.

data/
Contains the question bank dataset.

utils/
Contains validation logic for question structure.

reports/
Stores sample output results.

app.py
Main Flask application to run the system.
How It Works

1️⃣ User sends question data to the system

2️⃣ assessment_controller.py processes the request

3️⃣ validator.py checks question structure rules

4️⃣ Valid questions are accepted

5️⃣ Output stored or returned as JSON

Run the Project

Install dependencies:

pip install -r requirements.txt

Run server:

python app.py

Server runs on:

http://127.0.0.1:5000
