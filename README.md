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

Create a project directory named login-project in Kali Linux to organize the authentication log, Bash script, and generated security report.

Figure 2: Authentication Log Creation

Create a simulated auth.log file containing successful and failed SSH login attempts. The sample records provide test data for analyzing authentication activity without accessing real system security logs.

Figure 3: Bash Login Detector Script Creation

Create login_detector.sh using the Nano text editor. The script checks whether the log file exists, counts successful and failed login attempts, extracts IP addresses associated with failed logins, and identifies addresses that meet the suspicious activity threshold.

Figure 4: Script Permissions and Execution

Add execute permissions to the Bash script and run it in the Kali Linux terminal. Verify that the script processes the sample authentication records and displays the results without errors.

Figure 5: Security Report Generation

Generate security_report.txt containing the total number of successful and failed login attempts, the number of failures associated with each IP address, and alerts for addresses with three or more failed attempts.

### Results

Testing with the supplied sample log data produced seven failed login attempts and three successful login attempts. The script identified two suspicious IP addresses: 10.0.0.50, associated with three failed attempts, and 172.16.0.25, associated with four failed attempts.

The project demonstrates how Bash scripting can automate basic authentication log analysis and help identify patterns that may warrant further security investigation.
