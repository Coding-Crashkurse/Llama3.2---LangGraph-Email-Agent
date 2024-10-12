# Ollama Email Agent Setup Guide

## Prerequisites

1. **Enable Gmail API:**

   - Go to the Google Cloud Console, create a project, and enable the Gmail API.
   - Set up OAuth 2.0 credentials and download the `credentials.json` file.
   - Place `credentials.json` in the project directory.
   - Ensure the following scopes are enabled:
     - https://www.googleapis.com/auth/gmail.modify
     - https://www.googleapis.com/auth/gmail.send

2. **Install Ollama:**
   - Download and install Ollama from their official website.

## Setup

1. **Install Dependencies:**

- Run the following command to install the required packages:

`pip install -r requirements.txt`

2. **Run the Code:**

- Ensure `credentials.json` and `token.json` are in place.
- Run the code cells sequentially to authenticate and start the email checking process.
- The loop checks for new emails every 30 seconds on the first iteration, then every 2 seconds afterward.
