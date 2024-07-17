# Novanector_task
This program is a Password Strength Tester developed using Python and the Tkinter library. Its main purpose is to help users evaluate the security of their passwords by assessing various factors that contribute to password strength.

Key Features:
Password Generation: Generate strong and secure passwords.
Password Strength Checker: Evaluate the strength of existing passwords.
Guidelines for Strong Passwords: Provide tips and best practices for creating strong passwords.
User-Friendly Interface: Easy-to-use interface for seamless user experience.

Necessary Libraries:
tkinter:

Tkinter is the standard Python interface to the Tk GUI toolkit. It is used to create the graphical user interface (GUI) for the password strength tester.
Functions and classes used:
tk.Tk: Creates the main window.
tk.Label: Creates a text label.
tk.Entry: Creates an input field.
tk.Button: Creates a button.
tk.messagebox: Provides a simple way to display message boxes.
string:
The string module provides constants and classes related to string operations.
Functions and constants used:
string.ascii_lowercase: Lowercase letters.
string.ascii_uppercase: Uppercase letters.
string.digits: Digits.
string.punctuation: Special characters.

Common Passwords and Dictionary Words Lists:

common_passwords: A list of frequently used and easily guessable passwords.
dictionary_words: A sample list of common dictionary words used to check if a password contains any easily guessable words.
check_password_strength Function:

Length Score:
The length of the password is checked, and a score is calculated by dividing the password length by 8. The score is capped at 1.
Character Diversity Score:
The function checks if the password contains lowercase letters, uppercase letters, digits, and special characters.
Each category present in the password contributes to the diversity score, which is then divided by 4 to normalize it.
Common Password Check:
The function checks if the password is in the common_passwords list. If not, it gives a score of 1.
Dictionary Word Check:
The function checks if any dictionary word from dictionary_words is a substring of the password (case insensitive). If not, it gives a score of 1.
Entropy Calculation:
Entropy is a measure of randomness and unpredictability in the password.
The function determines the pool of characters used in the password (lowercase, uppercase, digits, special characters).
It calculates entropy using the formula len(password) * math.log2(pool).
The entropy score is normalized by dividing it by 50 and capped at 1.
Final Score Calculation:
The final score is the average of the length score, diversity score, common password score, dictionary word score, and entropy score.
Feedback Generation:
Feedback messages are generated based on the weaknesses identified in the password (short length, lack of diversity, common password, presence of dictionary words, low entropy).
Return Values:
The function returns the final score and feedback messages.
evaluate_password Function:

Password Retrieval:
The function retrieves the password entered by the user in the Tkinter entry widget (password_entry).
Password Evaluation:
It calls check_password_strength to evaluate the password and obtain the score and feedback.
Display Results:
The results are displayed in a message box using messagebox.showinfo, showing the password strength score and feedback messages.
This code provides a comprehensive evaluation of password strength and gives users feedback to improve their password security.

HOW IT WORKS:
The user inputs a password into the interface, and upon clicking the evaluation button, the program analyzes the password using various criteria.
It calculates scores for length, character diversity, common password presence, dictionary word presence, and entropy.
The results, including an overall strength score and detailed feedback on potential weaknesses, are displayed in a message box.
This tool serves as an educational resource, helping users understand the importance of creating strong passwords and how to do so effectively.
