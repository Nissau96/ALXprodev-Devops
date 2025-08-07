# ALXprodev-Devops

# Advanced Shell Scripting: Automating Tasks and Managing Processes

This repository contains a collection of advanced shell scripts designed to automate complex tasks, manage system processes, and enhance productivity in a Unix-like environment.

## Table of Contents

1.  [Overview](#overview)
2.  [Project Structure](#project-structure)
3.  [Prerequisites](#prerequisites)
4.  [Project Scripts](#project-scripts)
    - [Core API & Data Handling](#core-api--data-handling)
    - [Advanced Text & Data Processing](#advanced-text--data-processing)
    - [Advanced Process Management](#advanced-process-management)

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
Advanced_shell/
├── .gitignore
├── README.md
└── Advanced_shell/
    ├── apiAutomation-0x00
    ├── data_extraction_automation-0x01
    ├── batchProcessing-0x02
    ├── summaryData-0x03
    └── batchProcessing-0x04
```

## Prerequisites

To run the scripts in this project, you will need a Unix-like environment (like Linux or macOS) with the following tools installed:

- **Bash**: The Bourne Again SHell.
- **curl**: A command-line tool for transferring data with URLs.
- **jq** (optional but recommended): A lightweight and flexible command-line JSON processor. It is used in some scripts for prettier output.

You can install `jq` on Debian/Ubuntu with:
`sudo apt-get install jq`

## Project Scripts

The scripts in this project are organized by their core function, demonstrating a progression from basic tasks to more advanced concepts.

### Core API & Data Handling

#### `apiAutomation-0x00`

- **Objective**: Automates making a single, basic API request to the Pokémon API and saving the result.
- **Run**: `./Advanced_shell/apiAutomation-0x00`

#### `batchProcessing-0x02`

- **Objective**: Fetches data for a list of Pokémon sequentially. This script is robust, featuring error handling with a retry mechanism (up to 3 attempts) for failed requests.
- **Run**: `./Advanced_shell/batchProcessing-0x02`

### Advanced Text & Data Processing

#### `data_extraction_automation-0x01`

- **Objective**: Parses a local `data.json` file using a `jq`, `awk`, and `sed` pipeline to extract specific fields and format them into a human-readable sentence.
- **Run**: `./Advanced_shell/data_extraction_automation-0x01`

#### `summaryData-0x03`

- **Objective**: Reads a directory of JSON files, aggregates the data into a single `pokemon_report.csv` file, and uses `awk` to calculate and display average statistics.
- **Run**: `./Advanced_shell/summaryData-0x03`

### Advanced Process Management

#### `batchProcessing-0x04`

- **Objective**: Demonstrates parallel data fetching by running multiple download processes in the background simultaneously to improve performance.
- **Run**: `./Advanced_shell/batchProcessing-0x04`

---
