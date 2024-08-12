# Personal Data Filtering

## Overview

This project is designed to demonstrate how to obfuscate Personally Identifiable Information (PII) in log messages. The primary focus is on creating a function that will replace sensitive fields in log messages with a redaction string. The project also includes functionality for password encryption and validation, as well as database authentication using environment variables.

## Requirements

- Python 3.7
- Ubuntu 18.04 LTS
- All files should be executable
- Files should follow `pycodestyle` version 2.5

## Files

### `filtered_logger.py`

This module contains the `filter_datum` function used to obfuscate sensitive information in log messages.

#### `filter_datum(fields, redaction, message, separator)`

- **fields**: A list of field names to obfuscate (e.g., `["password", "date_of_birth"]`).
- **redaction**: The string used to replace sensitive data (e.g., `'xxx'`).
- **message**: The log message containing fields to be obfuscated.
- **separator**: The character that separates fields in the log message (e.g., `';'`).

The function uses regular expressions to replace occurrences of specified fields with the redaction string.

### `main.py`

A script to test the `filter_datum` function.

#### How to Run

1. Ensure that both `filtered_logger.py` and `main.py` are executable:

   ```bash
   chmod +x filtered_logger.py
   chmod +x main.py

2. Run the main.py script:

./main.py

You should see output where the specified fields (password, date_of_birth) are replaced with 'xxx'

Example Output

name=egg;email=eggmin@eggsample.com;password=xxx;date_of_birth=xxx;
name=bob;email=bob@dylan.com;password=xxx;date_of_birth=xxx;

Additional Notes
Ensure that all your files end with a newline.
The filtered_logger.py file should start with #!/usr/bin/env python3.
Documentation for all modules, classes, and functions should be provided.


Acknowledgments
This project is inspired by best practices in data security and logging. Special thanks to the Python community for their contributions to regex handling and encryption practices.



### Key Points in the `README.md`:

- **Overview**: Provides a brief description of what the project does.
- **Requirements**: Lists the prerequisites for running the code.
- **Files**: Describes the purpose of each file and provides information on the `filter_datum` function.
- **How to Run**: Instructions for running the script.
- **Example Output**: Shows what the output should look like when the script is run.
- **Additional Notes**: Includes reminders about file requirements and documentation.
- **License and Acknowledgments**: Provides licensing information and thanks to contributors.

This `README.md` will help users understand what the project is about, how to set it up, and how to use it.
