# Gmail Job Application Automator

This project demonstrates the integration of the Gmail API and Google Sheets API to automate the job application process. It searches the user's Gmail for unread emails from a specific sender, checks if they're already logged in a Google Sheets document, and if not, adds them to the document and marks the email as read.

## Prerequisites

Before running the code, make sure you have the following:

- Python 3.6 or later
- Google API credentials (`credentials.json`)

## Getting Started

To get started with the Gmail API and Google Sheets API, you need to set up Google API credentials and obtain the `credentials.json` file. Follow the steps below:

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. Create a new project or select an existing project.
3. Enable the Gmail API and Google Sheets API for your project.
4. Create credentials by following these steps:
   - Go to the "APIs & Services" > "Credentials" page.
   - Click on "Create credentials" and select "OAuth client ID".
   - Choose "Desktop app" as the application type.
   - Click on "Create" to generate the credentials.
   - Download the credentials as a JSON file and save it as `credentials.json` in the `credentials/` directory of this project.

## Token File

The `token.pickle` file stores the user's access and refresh tokens. If the file does not exist or the credentials are expired, the code will guide you through the OAuth process to generate a new token.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/ayirtman/gmail-job-application-automator.git
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

1. Replace the placeholder for google sheets ID in main.py with the ID of your Google Sheets document.

2. Run the script:

```bash
python src/main.py
```

## License

This project is licensed under the MIT License.


