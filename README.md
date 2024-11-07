# Digital Clock Using Shell Scripting on Linux CentOS

## 1. Introduction
This project involves creating a digital clock using shell scripting on Linux CentOS. Shell scripting is a powerful tool in Unix-like operating systems, allowing automation of various tasks. For this project, the script is designed to display the current time in a real-time, continuous format on the terminal, updating every second.

## 2. Objectives
The main objective of this project is to:
- Develop a shell script that displays a real-time digital clock.
- Update the time display every second to mimic the behavior of a standard digital clock.
- Use basic shell scripting commands and tools available on CentOS, such as `date`, `sleep`, and loops.

## 3. Prerequisites
To run this project, ensure that the following components are available on your system:
- CentOS Linux installed (any recent version).
- Basic understanding of Bash shell scripting.
- Familiarity with terminal and command-line interface.

## 4. Implementation

### Tools Used
- **Shell Scripting (Bash):** The script is written in Bash, the default shell in CentOS.
- **`date` Command:** To fetch the current time.
- **`sleep` Command:** To create a delay of 1 second between each update.
- **`clear` Command:** To refresh the display for the updated time.

## 5. Script Explanation
The following steps are taken in the implementation:
1. **Get the Current Time:** The `date` command is used to fetch the current time in the desired format.
2. **Clear the Screen:** The `clear` command is used to refresh the terminal screen for each time update.
3. **Looping:** A `while` loop is used to ensure that the clock continuously runs and updates every second.
4. **Delay:** The `sleep` command introduces a 1-second pause between each update to simulate the ticking of a clock.

## 6. Explanation of the Script
- `#!/bin/bash`: This line tells the system to use Bash as the interpreter for the script.
- `while true`: Creates an infinite loop that continues until the user stops the script manually.
- `clear`: Clears the terminal screen before each time update to create a clean display.
- `date +"%H:%M:%S"`: Fetches the current time in Hour:Minute:Second format.
- `sleep 1`: Pauses the execution of the script for 1 second to ensure the clock updates in real time.

## 7. How to Run the Script

### Step 1: Prepare the Environment
Ensure you have access to a CentOS system. Bash is the default shell on CentOS, so no additional software is needed beyond the terminal.

### Step 2: Create the Script File
We will create a shell script file to write the clock logic. Follow these steps to create a script file.
1. Open the terminal.
2. Use a text editor like `vi` or `nano` to create a new shell script file. For example, use `vi` to create the file named `digital_clock.sh`:
   ```bash
   vi digital_clock.sh
