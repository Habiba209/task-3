task # 3
Password Complixety Checker
Overview of Your Code
Function assess_password_strength(password):

Checks five criteria: length (≥8), uppercase, lowercase, numbers, special characters.
Uses regular expressions (re.search) to verify character types.
Calculates a strength score based on how many criteria are met.
Returns a strength label ("Strong", "Moderate", "Weak") and the criteria dictionary.
Function main():

Runs an interactive loop to input passwords.
Displays the strength and which criteria are met.
Allows exiting by typing "exit".
Sample Output

Run
Copy code
Password Strength Assessment Tool

Enter a password to assess its strength (or type 'exit' to quit): Pass123!
Password Strength: Strong
Criteria Assessment:
  Length: ✔
  Uppercase: ✔
  Lowercase: ✔
  Numbers: ✔
  Special_characters: ✔
Suggestions for Improvement
Enhance special characters set: You might want to include more or fewer special characters depending on your policy.
Add feedback messages: Suggest how to improve weak passwords.
Hide password input: Use getpass module to hide input for privacy.
Add minimum length parameter: Make length requirement configurable.
Normalize output formatting: Replace underscores with spaces in criteria display.
Example for improved criteria display:

python
2 lines
Copy code
Download code
Click to close
for criterion, met in criteria.items():
print(f" {criterion.replace('_', ' ').capitalize()}: {'✔' if met else '✘'}")
