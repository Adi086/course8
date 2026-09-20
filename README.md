# Emotion Detection Web Application

## Project Overview

This project is an AI-based web application that analyzes customer feedback and detects the emotions expressed in the text.

The application uses the **Watson NLP library** to identify emotions such as:

* Anger
* Disgust
* Fear
* Joy
* Sadness

The application is developed using Python and Flask and provides a web interface for users to enter text and receive emotion detection results.

## Technologies Used

* **Python** – Application development
* **Watson NLP** – Emotion detection
* **Flask** – Web application deployment
* **HTML/CSS** – User interface
* **PyUnit (unittest)** – Unit testing
* **PyLint** – Static code analysis

## Project Structure

```text
EmotionDetection/
│
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
│
├── test_emotion_detection.py
├── server.py
├── requirements.txt
└── README.md
```

## Features

1. Detects emotions from customer feedback.
2. Identifies anger, disgust, fear, joy, and sadness.
3. Returns emotion scores in a structured format.
4. Identifies the dominant emotion.
5. Provides a Flask-based web interface.
6. Handles blank input and invalid requests.
7. Includes unit tests for validation.
8. Supports static code analysis.

## Emotion Detection Output

The application returns the following information:

* Anger score
* Disgust score
* Fear score
* Joy score
* Sadness score
* Dominant emotion

Example:

```python
{
    "anger": 0.01,
    "disgust": 0.02,
    "fear": 0.01,
    "joy": 0.95,
    "sadness": 0.01,
    "dominant_emotion": "joy"
}
```

*The values above are illustrative. Actual scores depend on the Watson NLP model's response.*

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

Navigate to the project directory:

```bash
cd YOUR_REPOSITORY
```

Create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Running the Application

Run the Flask server:

```bash
python server.py
```

Open the application in a web browser using the local URL displayed in the terminal.

## Testing

Run the unit tests:

```bash
python -m unittest test_emotion_detection.py
```

The tests verify that the emotion detection function returns the expected results.

## Static Code Analysis

Run static code analysis using the configured tool:

```bash
pylint server.py
```

Use the command specified by the course if it differs from the example above.

## Error Handling

The application handles:

* Blank input submitted by the user.
* Invalid or unsuccessful API responses.
* HTTP status code 400.
* Unexpected errors during emotion detection.

## Project Objectives

* Implement an emotion detection application using Watson NLP.
* Format the emotion detection output.
* Validate the Python package.
* Write and execute unit tests.
* Deploy the application using Flask.
* Implement error handling.
* Perform static code analysis.

## Author

**Aditya Subhash Shirse**

## License

This project was developed for educational purposes as part of the final project assessment.
