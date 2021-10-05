# BashScriptingProject
 
INSTRUCTIONS (check the required deliverables – cover page):
1. Create a directory named COURSEWORK in your home directory at the College’s Linux server. The main script(s) and all related files should be stored there.
2. Make sure that you test the proper execution without any error messages and the required functionality of your scripts before submission. User interface has to be simple but intuitive, validating all user inputs and cases, providing meaningful instructions and error messages.
3. Your scripts have to be properly formatted and documented using appropriate comments, to allow for easy code inspection and debugging.
4. The PDF document should include the answers to the questions of part 2, along with a cover page stating your full name, the module code, the module title, and the date of submission.

Part 1: Create the scripts fUser and cMail to generate and send an email to a user with information about their logon history.
1. Utilize a menu with three options: a) retrieve a certain user logon history and generate a file, b) execute another script (cMail) to send the user a message and c) exit the program.
2. Validate user input, displaying meaningful error messages for any invalid input.
3. Check whether a file named cMail exists under the current directory and if it does not, display an error message and terminate the program.
4. Ask the user to enter a username to search for. Use some particular input to cancel and exit the program.
5. Validate the existence of the given username. If the username is not existent in the system, display an error message and repeat step 4.
6. Request a directory for the files to be created, under the working directory (COURSEWORK).
7. Check whether the given directory already exists and if it does, inform the user and ask whether it should proceed using it or not:
A. If the answer is affirmative, proceed and use the existing directory.
B. If the answer is negative, repeat step 5 until either a new directory is given, or an affirmative answer is received (as per the step 7A).
8. Create a content file in the specified directory, named <username>.txt (e.g. for user “root” it would be: “root.txt”).

Informat ion Technology:
9. If the file already exists, it is overwritten. The content file should contain:
A. A title line “Login information about user: ” and the given username.
B. Information about the last 10 (most recent) logon sessions of the given user.
C. A line indicating whether the user is now online or offline
D. A line with a timestamp (current date and time)
10. Using the second menu option (execute script), the cMail script should be executed.
A. The user should not be able to select script execution if cMail script does not exist.
B. After the cMail script is executed, with or without an error, the fUser script should return to the menu.
11. Exiting the fUser script should display a relevant message.
The script cMail should: (LO 2: 35 points)
12. Take a username (already validated) and a directory as passing arguments. The directory may be a relative or an absolute path.
13. Log passing arguments given, successful actions and all error messages to file cMail.log, along with a timestamp, for every execution of the cMail script. Log file should not be overwritten.
14. Validate the number of passing arguments:
A. If only one passing argument is given then this is the username, while the directory should be considered to be the working one.
B. If no passing arguments are given, then display an error message and terminate the cMail script execution.
15. Validate the existence of the content file (named <username>.txt) under the given directory. If the content file does not exist, display an error message and terminate the cMail script execution.
16. Send an email message to the user, using the content file as body text, with the subject “Your logon history”.
17. Display a message for successful script execution.
18. Have read, write and execute access rights for the owner and read, execute for everyone else.

Full points awarded when commands are efficiently used and additional relevant functionality is implemented beyond the given requirements. Total (100%): 45 35
Part 2 (LO 1): Prepare and submit a 1-page PDF document with answers to the following questions:
1. Identify 2 instances of operating system storage management tasks in your script(s). In each case, state the command, its location in your script(s), and the storage management activity it performs (e.x. file deletion). (10 points)
2. Identify 1 instance of inter-process communication using pipes in any of the scripts and briefly explain how it works, mentioning the producer and the consumer processes. In case you did not use IPC using pipes in any of your scripts, please provide an example, demonstrating its use. (10 points)