# Test Cases – Simulated Device Monitoring and Alert System

Tested by: Harold Kierby T. Calalang       Date: October 12, 2026

| Test Case | Input or Action | Expected Result | Actual Result | Pass/Fail |
|------|----------|-----------------------------------|---|---|
| TC01 | Choose 1 | Five readings: 30, 28, 35, 40, 60 | Displayed the five readings correctly. | Pass |
| TC02 | Choose 2, enter 33 | Reading added successfully | It shows "Reading added successfully." | Pass |
| TC03 | Choose 2, enter abc | Invalid input. Enter a whole number only. | It shows "Invalid input. Enter a whole number only." | Pass |
| TC04 | Choose 2, enter -5 | Invalid reading. Enter a value from 0 to 100. | It shows "Invalid reading. Enter a value from 0 to 100." | Pass |
| TC05 | Choose 2, enter 101 | Invalid reading. Enter a value from 0 to 100. | It shows "Invalid reading. Enter a value from 0 to 100." | Pass |
| TC06 | Choose 2, enter 0 | Reading added successfully | It shows "Reading added successfully." | Pass |
| TC07 | Choose 2, press Enter without entering a value | Invalid input. The reading cannot be empty. | It shows "Invalid input. The reading cannot be empty." | Pass |
| TC08 | Choose 3 | Display the classification of all readings. | Classified 30, 28, 35, and 40 °C as NORMAL and 60 °C as WARNING. | Pass |
| TC09 | Choose 4 | Display the monitoring summary, including total, average, minimum, maximum, percentages, and overall status. | Displayed a total of 193, an average of 38.60 °C, a minimum of 28 °C, a maximum of 60 °C, and the overall status "WARNING HEAVY WORK LOAD." | Pass |
| TC10 | Choose 5 | Display the thank-you message and exit the program. | It shows "Thank you for using the Device Monitoring System." | Pass |
| TC11 | Enter 6 at the menu | Invalid choice. Please enter a number from 1 to 5. | It shows "Invalid choice. Please enter a number from 1 to 5." | Pass |
| TC12 | Choose 2, enter 59 | Reading added successfully; classify the reading as WARNING. | It shows "Reading added successfully." The reading is classified as WARNING. | Pass |
| TC13 | Choose 2, enter 80 | Reading added successfully; classify the reading as CRITICAL. | It shows "Reading added successfully." The reading is classified as CRITICAL. | Pass |
| TC14 | Choose 2, enter - | Invalid input. Enter a whole number only. | It shows "Invalid input. Enter a whole number only." | Pass |

## Bugs Found and Fixed
- The test that was hardest to pass. 
