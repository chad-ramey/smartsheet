
# Smartsheet Automation Lab

This repository contains a collection of Python scripts that automate various tasks within Smartsheet, such as user delicensing and exporting user data.

## Table of Contents
  - [Scripts Overview](#scripts-overview)
  - [Requirements](#requirements)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [License](#license)

## Scripts Overview

### 1. [smartsheet_delicense_users.py](smartsheet_delicense_users.py)
**Description**: This script manages the delicensing of Smartsheet users. It handles accounts with data by transferring the data to a designated custodian account before delicensing. The script can operate using either email addresses or Smartsheet IDs based on the user’s choice.

### 2. [smartsheet_export_users.py](smartsheet_export_users.py)
**Description**: This script exports a list of Smartsheet users to a CSV file. It includes details such as user emails and last login information. The CSV file is saved with a timestamp in its name for easy identification and tracking.

## Requirements
- **Python 3.x**: Ensure you have Python 3.x installed on your system.
- **Smartsheet API Access**: The scripts require API access to Smartsheet. Generate an API token from your Smartsheet account.
- **Python Packages**: The scripts require certain Python packages, including `requests` and `csv`. Install them using the provided requirements file (`requirements.txt`).

## Installation
1. Clone the repository to your local machine using:
   ```bash
   git clone <repository-url>
   ```
2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your Smartsheet API token in an environment variable or `.env` file for secure access.

## Usage
1. **User Delicensing**:
   - Run `smartsheet_delicense_users.py` to delicense users. The script will prompt you to choose whether to use email addresses or Smartsheet IDs for the operation.
   - Example command:
     ```bash
     python smartsheet_delicense_users.py
     ```

2. **Exporting User Data**:
   - Use `smartsheet_export_users.py` to export user details to a CSV file. The script includes last login information for each user.
   - Example command:
     ```bash
     python smartsheet_export_users.py
     ```

## Contributing
Feel free to submit issues or pull requests if you would like to contribute to the scripts or improve automation workflows within Smartsheet.

## License
This project is licensed under the MIT License.