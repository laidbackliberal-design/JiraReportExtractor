# JIRA Accessibility Defects to Excel Generator

This Python app fetches accessibility defects from JIRA and generates an Excel workbook with tabs for global defects and each tested page.

## Requirements

- Python 3.8+
- JIRA API access (username and API token)

## Installation

1. Clone or download the project.
2. Install dependencies: `pip install -r requirements.txt`
3. Configure JIRA settings in `config.py` or environment variables.

## Usage

Run the script: `python main.py`

The Excel file will be generated as `accessibility_report.xlsx`.

## Configuration

Set the following in `config.py` or as environment variables:
- JIRA_URL: Your JIRA server URL
- JIRA_USERNAME: Your JIRA username
- JIRA_API_TOKEN: Your JIRA API token
- JIRA_PROJECT: Project key
- JQL_QUERY: JQL to filter accessibility defects (default: 'issuetype = Bug AND labels = accessibility')