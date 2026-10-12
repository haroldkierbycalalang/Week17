# Simulated Device Monitoring and Alert System
 
**Student Name:** Harold Kierby T. Calalang
**Student Number:**  2601326
**Section:** 1CPE-A
 
## Project Description
This program is an integrated development project that monitors simulated device temperature readings. It stores temperatures in a list, classifies individual data points into strict categories, and computes a comprehensive tracking summary with an overall device operational status. The entire solution is engineered with a modular function structure and relies completely on manual mathematical tracking algorithms.
 

## Features
- View all stored temperature readings
- Add a new reading (whole numbers from 0 to 100 only)
- Classify every reading
- Generate a numerical summary and overall status
- Reject invalid menu choices and invalid readings
 
## Requirements
- Python 3 
 
## How to Run
1. Open a terminal inside the Week17 folder.
2. Type: python device_monitor.py
   (On macOS or Linux, type: python3 device_monitor.py)
 
## Sample Output
```text
CPU CORE MONITORING SYSTEM

[1] View Readings
[2] Add Reading
[3] Classify Readings
[4] Generate Summary
[5] Exit
Enter choice: 1

CURRENT READINGS
----------------
Reading 1: 30 °C
Reading 2: 28 °C
Reading 3: 35 °C
Reading 4: 40 °C
Reading 5: 60 °C
 ```
## Test Cases
I performed 10 tests. 10 passed and 0 failed.
Full details are in test_cases.md.
 
## Known Limitations
- Readings are held entirely in volatile RAM memory loops and wipe cleanly when the instance terminates.
- The application processes integer numeric entries only and rejects floating-point/decimal temperature data points.

## Reflection
The hardest part of this project was enforcing a strict modular layout where state metrics navigate safely between boundaries through arguments and return channels without depending on a global statement keyword. During validation testing, I identified and corrected a logical error where the inclusive upper edge parameter of 80 °C was misclassified as CRITICAL instead of WARNING due to a poorly mapped relational operator. In future releases, I would expand this architecture to preserve operational data metrics over long runs by adding text file-handling storage logic.
