AI Assessment Question Structure Controller
Project Description

The AI Assessment Question Structure Controller is a backend module developed for an AI Interview Monitoring System.
The purpose of this project is to validate and manage the structure of assessment questions before they are stored or used in the system.

This module ensures that every question follows a standard format so that the AI system can process the questions correctly during assessments.

Features

Question structure validation

JSON-based question handling

Input validation rules

Controller for processing questions

Sample output generation

Technologies Used

Python

Flask

JSON

Project Structure
ai-assessment-question-controller
│
├── controllers
│   └── assessment_controller.py
│
├── utils
│   └── validator.py
│
├── data
│   └── questions.json
│
├── reports
│   └── sample_output.json
│
├── app.py
│
└── requirements.txt
How the System Works

The user sends question data in JSON format to the system.

The assessment_controller.py receives the request.

The controller sends the data to validator.py.

The validator checks whether the question follows the required structure.

If the validation is successful, the question is accepted.

The system returns the result as JSON output.

Example Input
{
  "question": "What is Artificial Intelligence?",
  "options": [
    "Machine learning",
    "Artificial Intelligence",
    "Database",
    "Operating system"
  ],
  "answer": "Artificial Intelligence",
  "difficulty": "Easy"
}
Example Output
{
  "status": "success",
  "message": "Question validated successfully"
}
How to Run the Project

Install required packages:

pip install -r requirements.txt

Run the application:

python app.py
Server

After running the project, the Flask server will start at:

http://127.0.0.1:5000

You can test the API using Postman or any API testing tool.

Internship Contribution

In this internship task, the main objective was to develop a controller that validates the structure of AI assessment questions.
The module checks whether the questions follow the required format and ensures that only valid questions are used in the AI interview system.
