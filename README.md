# ALXprodev-Devops

# Advanced Shell Scripting: Automating Tasks and Managing Processes

This repository contains a collection of advanced shell scripts designed to automate complex tasks, manage system processes, and enhance productivity in a Unix-like environment.

## Overview

Shell scripting is a powerful tool that allows users to automate repetitive tasks by writing a sequence of commands in a script file. This project explores fundamental and advanced concepts, including:

- **Basic Syntax**: Variables, control structures (`if-else`, `for`, `while`), and functions.
- **Advanced Commands**: Text processing with `grep`, `awk`, and `sed`.
- **Process Management**: Handling foreground/background jobs with `jobs`, `fg`, `bg`, and `kill`.
- **Automation Scripts**: Practical scripts for tasks like backups and system monitoring.
- **Error Handling**: Building robust scripts with `exit` status checks, logging, and the `trap` command.

## Project Structure

```
.
├── Advanced_shell/
│   ├── apiAutomation-0x00      # Task 1: Automates API requests
│   └── ...                     # Other scripts will go here
├── .git/                       # Git directory for version control
└── README.md                   # This file
```

## Prerequisites

To run the scripts in this project, you will need a Unix-like environment (like Linux or macOS) with the following tools installed:

- **Bash**: The Bourne Again SHell.
- **curl**: A command-line tool for transferring data with URLs.
- **jq** (optional but recommended): A lightweight and flexible command-line JSON processor. It is used in some scripts for prettier output.

You can install `jq` on Debian/Ubuntu with:
`sudo apt-get install jq`

## Scripts and Usage

### Task 1: API Request Automation (`apiAutomation-0x00`)

This script automates the process of making API requests to the Pokémon API and saving the results.

**How to Run:**

1.  Navigate to the script's directory:
    ```bash
    cd Advanced_shell
    ```
2.  Make the script executable:
    ```bash
    chmod +x apiAutomation-0x00
    ```
3.  Execute the script:
    ```bash
    ./apiAutomation-0x00
    ```

**Behavior:**

- **On Success**: It creates a `data.json` file in the same directory with the Pokémon's data.
- **On Failure**: It creates an `errors.txt` file containing an error message, a timestamp, and the HTTP status code.

---

### Task 2: Extract Pokémon Data (`data_extraction_automation-0x01`)

This script uses `jq`, `awk`, and `sed` to extract data from `data.json` and format it into a sentence. It depends on `data.json` from Task 1.

**How to Run:**

```bash
cd Advanced_shell
chmod +x data_extraction_automation-0x01
./data_extraction_automation-0x01
```

**Expected Output:**

```
Pikachu is of type electric, weighs 6kg, and is 0.4m tall.
```

---
