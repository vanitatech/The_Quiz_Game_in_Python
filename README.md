# Python Quiz Game

A command-line True/False quiz game built with Python. This project was created to help me practise **Object-Oriented Programming (OOP)**, classes, objects, lists, dictionaries, loops, functions, and working with multiple Python files.

## Features

* Displays a series of True/False questions
* Accepts answers from the user
* Checks answers automatically
* Keeps track of the user's score
* Displays the correct answer when the user answers incorrectly
* Displays the current score after each question
* Displays the final score when the quiz is complete
* Uses classes and objects to organise the quiz logic

## Project Structure

```text
Quiz_game_python/
│
├── main.py
├── data.py
├── question_model.py
├── quiz_brain.py
└── README.md
```

### `main.py`

The main program that:

* Imports the question data and classes
* Creates the question bank
* Creates the `QuizBrain` object
* Runs the quiz until all questions have been answered
* Displays the final score

### `data.py`

Contains the quiz questions and their correct answers.

### `question_model.py`

Contains the `Question` class used to create Question objects.

```python
class Question:

    def __init__(self, q_text, q_answer):
        self.text = q_text
        self.answer = q_answer
```

### `quiz_brain.py`

Contains the `QuizBrain` class, which manages:

* Current question number
* Question selection
* User answers
* Answer checking
* Score tracking
* Checking whether more questions remain

## OOP Concepts Practised

This project helped me understand several important Object-Oriented Programming concepts.

### Classes

A class acts as a blueprint for creating objects.

```python
class Question:
    ...
```

### Objects

Each question is represented as a `Question` object.

```python
new_question = Question(question_text, question_answer)
```

### Attributes

Each Question object stores its own text and answer.

```python
self.text = q_text
self.answer = q_answer
```

### Methods

The `QuizBrain` class contains methods that perform different tasks:

```python
still_has_questions()
next_question()
check_answer()
```

### `self`

I also practised using `self` to access data belonging to a particular object.

For example:

```python
self.score
self.question_number
self.question_list
```

## How the Quiz Works

The program follows this basic flow:

```text
Question data
      ↓
Create Question objects
      ↓
Store questions in a question bank
      ↓
Create QuizBrain object
      ↓
Display question
      ↓
Get user's answer
      ↓
Check answer
      ↓
Update score
      ↓
Move to next question
      ↓
Display final score
```

## Example

```text
Q.1: A Mac is not a PC (True/False): False

You got it right!
The correct answer was: False.
Your current score is: 1/1
```

At the end of the quiz:

```text
You've completed the quiz.
Your final score was: 8/10
```

## Technologies Used

* Python 3
* Object-Oriented Programming
* Python lists
* Python dictionaries
* Functions
* Classes and objects
* Loops
* Conditional statements
* Multiple Python modules

## How to Run

Clone the repository and navigate to the project directory:

```bash
cd Quiz_game_python
```

Run the program:

```bash
python3 main.py
```

Follow the instructions displayed in the terminal.

## What I Learned

Through this project I practised:

* Creating classes and objects
* Creating and using methods
* Using `__init__`
* Understanding `self`
* Creating object attributes
* Working with lists of objects
* Accessing dictionary values
* Importing code from different Python files
* Passing lists into classes
* Using loops to control a program
* Comparing user input with stored answers
* Building a simple multi-file Python application
* Using Git and GitHub to version-control my project

## Future Improvements

Possible improvements for this project include:

* Adding multiple-choice questions
* Adding different quiz categories
* Randomising the question order
* Adding difficulty levels
* Adding a graphical user interface
* Getting questions from an online API
* Adding a high-score system
* Adding unit tests

## Learning Project

This project was created as part of my ongoing Python learning and software engineering development journey.
