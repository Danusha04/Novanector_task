# Novanector_task
This program is a Password Strength Tester developed using Python and the Tkinter library. Its main purpose is to help users evaluate the security of their passwords by assessing various factors that contribute to password strength.

Key Features:
Common Passwords and Dictionary Words Lists:

common_passwords: A list of frequently used and easily guessable passwords.
dictionary_words: A sample list of common dictionary words used to check if a password contains any easily guessable words.

Password Evaluation:

Analyzes passwords based on length, character diversity (including lowercase, uppercase, digits, and special characters), and overall complexity.
Common Password Check:

Compares the entered password against a predefined list of commonly used passwords to discourage users from selecting easily guessable options.
Dictionary Word Check:

Checks if the password contains any simple dictionary words to prevent the use of predictable passwords.
Entropy Calculation:

Calculates the entropy of the password, which measures its randomness and unpredictability, providing a score that reflects its strength.
User-Friendly Interface:

Features a simple graphical user interface (GUI) built with Tkinter, allowing users to easily input their passwords and receive instant feedback.
Real-Time Feedback:

Provides immediate feedback on the password's strengths and weaknesses, along with suggestions for improvement to enhance security.
How It Works:
The user inputs a password into the interface, and upon clicking the evaluation button, the program analyzes the password using various criteria.
It calculates scores for length, character diversity, common password presence, dictionary word presence, and entropy.
The results, including an overall strength score and detailed feedback on potential weaknesses, are displayed in a message box.
This tool serves as an educational resource, helping users understand the importance of creating strong passwords and how to do so effectively.
