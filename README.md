# Ventilator System ReadMe

Overview
The Ventilator System is a safety-critical program designed to monitor and manage the settings of a ventilator, a device essential for assisting patients with breathing. The program ensures that the ventilator operates within safe parameters by continuously checking and reporting various metrics. It features a set of procedures to handle key tasks, including initializing settings, performing critical checks, and providing real-time status updates.

## Language Used

This project is developed in [SPARK Ada](https://www.adacore.com/sparkada), a formal subset of the Ada programming language designed for high-integrity and high-assurance software. 

## Files

- `.ada`, `.ads`, `.adb` files are used in this project and are written in SPARK Ada.

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/KamileSimkute/yourrepository.git

Key Features
1. Start Procedure
Initializes global variables required for the ventilator system.
2. Ventilator_Critical_Check Procedure
Monitors the ventilator to ensure the total air supply is sufficient.
Calculates the total air by summing Input_supply and Total_Volume.
Checks if the total air is less than 5 units.
3. Volume_delivered Procedure
Continuously prompts users to input the volume of air delivered.
Utilizes the Air_Range function to validate that the input is between 0 and 7000 units.
4. Breaths_delivered Procedure
Prompts users to input the number of breaths delivered.
Uses the Air_Range function for validation of input values.
5. Print_Status Procedure
Provides a visual status report of the ventilator system.
Specifications
Question 1
(a) Program Description
The Ventilator System is designed to simulate a safety-critical system, focusing on maintaining and monitoring the operational parameters of a ventilator. It ensures the ventilator's air supply and breathing parameters are within safe limits, crucial for life-supporting applications. The system continuously checks these parameters and updates the user with the current status, making sure the ventilator operates safely.

(b) Compilation and Execution
Ensure that the program is compatible with the SPARK Ada compiler. The program should compile successfully and produce output demonstrating its main features, including the initialization of variables, critical checks, and status reporting.

Example Runs:

Starting Ventilator System...
Enter volume delivered: 3500
Enter breaths delivered: 15
Checking ventilator status...
Total air supply is sufficient.
Current status: OK


(c) Data and Information Flow Analysis
Include appropriate depends clauses to ensure that the program passes SPARK Ada’s data and information flow analysis, demonstrating correct usage of variables and data handling.

(d) Pre- and Post-Conditions
Add suitable pre-conditions and post-conditions to verify that the program operates correctly with respect to these conditions. Utilize SPARK Ada to validate that the program adheres to these specifications.

(e) Advanced Solutions
Look for opportunities to enhance the program with advanced and insightful solutions that go beyond the basic requirements. These solutions should demonstrate a deeper understanding and clever use of SPARK Ada features.

Additional Notes
Ensure that all procedures are tested thoroughly to confirm they meet safety and operational requirements.
Maintain clear and concise documentation to facilitate understanding and further development.
