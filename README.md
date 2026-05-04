# ITPM Assignment 1: Transliteration Accuracy Testing

This repository contains the Playwright automation script used to test the Singlish to Sinhala chat transliteration tool for the IT3040-ITPM module.

## Prerequisites
* Python 3.11 or 3.12 installed
* Google Chrome installed

## Installation Instructions

1. Clone this repository to your local machine.
2. Open your Command Prompt and navigate to the extracted project folder.
3. Update pip to the latest version:
   ```bash
   python -m pip install -U pip
   ```
4. Install the required dependencies:
   ```bash
   python -m pip install playwright openpyxl
   ```
5. Install the Playwright browser binaries:
   ```bash
   python -m playwright install
   ```

## Running the Tests

1. Ensure your test data file (`Assignment 1 - Test cases.xlsx`) is located in the same directory as the Python script.
2. Open your Command Prompt, navigate to the folder, and run the following command:
   ```bash
   python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --input-col "Input" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
   ```
3. The script will automatically open the browser, enter the 50 Singlish test inputs, and record the Actual Output and Pass/Fail status into the Excel file.
