**Name:** SALMANUL FARISI.
**Company:** CODETECH IT SOLUTIONS.
**ID:** CT08DS5913.
**Domain:** CYBER SECURITY&ETHICAL HACKING.
**Duration:** August 15 to September 15 2024.
**Mentor:** Neela Santhosh Kumar .

## Overview of the Project
**Project:** Vulnerability Scanning Tool

## Objective:
The objective of this project is to develop a Python script that scans a network or website for common security vulnerabilities, such as open ports, outdated software versions, and misconfigurations.

## Key Activities
**Port Scanning:**

The script scans a specified host for open TCP ports within a defined range. It identifies which ports are open and potentially accessible.

**Software Version Checking:**

The script checks for known vulnerabilities in specified software versions by querying the CVE database. It compares the software versions against known security advisories.


**Misconfiguration Checking:**

The script examines HTTP headers for common security misconfigurations, such as missing security headers that could make the host vulnerable to attacks.


## Technologies Used
**Python:** The primary programming language used to write the vulnerability scanning tool.
**socket:** Used for creating network connections and performing port scans.
**requests:** Utilized to send HTTP requests and analyze HTTP responses for misconfiguration checking and software version queries.
**threading:** Employed to run multiple scanning tasks concurrently, improving efficiency.

## Code Explanation
The Python script performs a series of checks to identify vulnerabilities:

**Port Scanning:**

Function: scan_ports(host)
Purpose: Scans for open ports on the specified host by attempting to connect to each port within the range 1-1024.


**Software Version Checking:**

Function: check_software_versions(software_list)
Purpose: Checks if specified software versions have known vulnerabilities by querying the CVE database and analyzing the response for matches.

**Misconfiguration Checking:**

Function: check_misconfigurations(host)
Purpose: Checks the HTTP headers of the specified host for common security misconfigurations, such as missing X-Frame-Options and Content-Security-Policy headers.

**Main Execution:**

Function: run_scan(target_host, software_list)
Purpose: Manages the execution of the scanning functions using threads for concurrent operations, and prints the results of the scans.
Usage

**Set the Target Host:**

Replace "website.com" in the target_host variable with the actual domain or IP address of the host you want to scan.

**Define the Software List:**

Update the software_list dictionary with the software names and their versions that you want to check for vulnerabilities.

**Run the Script:**

Execute the script to start scanning the specified host for open ports, software vulnerabilities, and misconfigurations.

![Screenshot 2024-09-04 144234](https://github.com/user-attachments/assets/6189bb58-0006-4b83-ae21-438d99ee6351)

