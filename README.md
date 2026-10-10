# Project

## Objective
The Suspicious Login Detector project aimed to develop a Bash script for analyzing authentication logs and identifying potentially suspicious login activity. The primary focus was to count successful and failed login attempts, extract IP addresses associated with repeated failures, and generate security alerts based on a defined threshold. This hands-on experience was designed to develop practical skills in Linux scripting, log analysis, and basic security monitoring.

### Skills Learned
Students will practice the following skills:
Creating and running a Bash script.
Using variables to store filenames and other values.
Using if statements to check whether a file exists.
Using grep to search log files for specific events.
Using grep -c to count matching log entries.
Using awk to extract specific information from a line of text.
Using sort and uniq -c to organize and count repeated values.
Using pipes (|) to pass the output of one command to another.
Using loops to process multiple results.
Using conditional statements to identify suspicious activity.
Redirecting script output to a report file.
Interpreting authentication logs from a cybersecurity perspective.

### Tools Used
Kali Linux for the scripting and testing environment.
Bash for developing the login detection script.
grep for searching and counting authentication events.
awk for extracting IP addresses from log entries.
sort and uniq for organizing and counting repeated IP addresses.
Nano for creating and editing project files.

### Steps
Figure 1: Kali Linux Project Directory Setup

<img width="257" height="82" alt="image" src="https://github.com/user-attachments/assets/c1e4a60b-4697-4103-97d0-1bfbe5fa19c9" />


Create a project directory named login-project in Kali Linux to organize the authentication log, Bash script, and generated security report.

Figure 2: Authentication Log Creation

<img width="922" height="287" alt="image" src="https://github.com/user-attachments/assets/eb4d5f57-56be-4cc2-9f23-0e8eb74962b7" />


Create a simulated auth.log file containing successful and failed SSH login attempts. The sample records provide test data for analyzing authentication activity without accessing real system security logs.

Figure 3: Bash Login Detector Script Creation

<img width="950" height="787" alt="image" src="https://github.com/user-attachments/assets/b22971cb-df37-4e87-8556-6e651fa6a198" />


Create login_detector.sh using the Nano text editor. The script checks whether the log file exists, counts successful and failed login attempts, extracts IP addresses associated with failed logins, and identifies addresses that meet the suspicious activity threshold.

Figure 4: Script Permissions and Execution

<img width="440" height="297" alt="image" src="https://github.com/user-attachments/assets/21296140-1702-42a9-b21b-681c6c76372c" />


Add execute permissions to the Bash script and run it in the Kali Linux terminal. Verify that the script processes the sample authentication records and displays the results without errors.

Figure 5: Security Report Generation

<img width="440" height="297" alt="image" src="https://github.com/user-attachments/assets/382f44e0-99a6-4fcc-a33a-b62d1d12fe40" />


<img width="510" height="97" alt="image" src="https://github.com/user-attachments/assets/d81026a2-9c08-4554-ba0b-ee2e7b2c63d3" />



Generate security_report.txt containing the total number of successful and failed login attempts, the number of failures associated with each IP address, and alerts for addresses with three or more failed attempts.

### Results

Testing with the supplied sample log data produced seven failed login attempts and three successful login attempts. The script identified two suspicious IP addresses: 10.0.0.50, associated with three failed attempts, and 172.16.0.25, associated with four failed attempts.

The project demonstrates how Bash scripting can automate basic authentication log analysis and help identify patterns that may warrant further security investigation.
