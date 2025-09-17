Online Quiz Application 📝
A Python-based online quiz application using object-oriented programming (OOP) principles.

Features
Multiple Question Types: Supports both multiple-choice and true/false questions.

User Management: Allows multiple users to take the quiz.

Scoring System: Calculates and displays scores for each user.

Leaderboard: Shows a ranked list of users based on their scores.

Interactive Interface: Provides a user-friendly command-line interface.

Core Principles: The Anatomy of the Code
The strength of this application lies in its design, which is based on several key OOP principles.

Inheritance and Polymorphism
The code uses a Question base class, which defines the fundamental characteristics of a question (text and a correct answer). 
The MCQ and TrueFalse classes then inherit from this base class. This is an efficient way to reuse code and ensures that all question types share a common foundation. 
A great example of polymorphism is the check_answer method. While the base Question class has a generic check_answer method, the MCQ class overrides it to handle numerical user input, converting the option number to the correct text before checking the answer. 
This allows the quiz to treat different question types in a unified way, calling q.
check_answer(answer) regardless of whether q is an MCQ or a TrueFalse object.

Encapsulation and Modularity
The code is broken down into distinct, self-contained classes. 
The User class, for instance, encapsulates all user-related data (name and score). 
The Result class handles all score-related logic. This modular design makes the code cleaner and easier to maintain. 
If you wanted to change how the leaderboard is sorted, you'd only need to modify the leaderboard method in the Result class, without affecting any other part of the program. 
The quiz logic itself is contained within the Quiz class, which is responsible for the overall flow of the game.

Static Methods
The Result class also demonstrates the use of static methods (display_score and leaderboard). 
These methods are associated with the class itself rather than with a specific instance of the class. 
They don't need access to any instance-specific data (like self.username) to function, making them perfect for utility functions that perform a task related to the class concept but not a specific object


Online Quiz Application 📝
A Python-based online quiz application using object-oriented programming (OOP) principles.

Features
Multiple Question Types: Supports both multiple-choice and true/false questions.

User Management: Allows multiple users to take the quiz.

Scoring System: Calculates and displays scores for each user.

Leaderboard: Shows a ranked list of users based on their scores.

Interactive Interface: Provides a user-friendly command-line interface.


How to Run
Clone the repository:
git clone https://github.com/your-username/online-quiz-application.git

Navigate to the project directory:
cd online-quiz-application

Run the application:
python "Online Quiz Application.ipynb"
You can also use jupyter notebook to run this file.

Code
The application is built using several classes to demonstrate OOP concepts:

Question Class
This is the base class for all question types.

MCQ Class
This class inherits from Question and is used for multiple-choice questions. It includes methods to display options and check the answer against the correct option.

TrueFalse Class
This class also inherits from Question and is specifically for true/false questions.

Quiz Class
This is the core class that manages the quiz flow, iterating through questions and handling user input.

User Class
This class represents a quiz participant and tracks their score.

Result Class
This class contains static methods to display the user's score and generate the leaderboard.

Contributing
Feel free to fork the repository and contribute! You can add more question types, a graphical user interface, or a feature to save quiz results to a file.


