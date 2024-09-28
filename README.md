# GPT2-Chatbot-and-Google-Sheets-Integration
# Flask-Based Google Sheets Integration and Chatbot Project
A web application built with Flask that integrates Google Sheets for data storage, a chatbot interface. It includes frontend forms for submitting data and retrieving data from Google Sheets, along with chatbot.

## Features

- **Google Sheets Integration**: Submit and retrieve user data to/from a Google Sheet.
- **Chatbot Interface**: A simple chatbot that responds to user queries.


# Setup Instruction
## Step 1: Install Dependencies
``` bash
pip install -r requirements.txt
```

## Step 2: Running the Application
```bash
python app.py
```

## Step 3: Accessing the Web Interface
1) Go to http://localhost:5000 to access the homepage.
2) From there, you can:
    - Submit data to Google Sheets via the Google Sheets form.
    (The data will be updated in https://docs.google.com/spreadsheets/d/1AHwkl-9r0kY4O311oIkpu5ao-pCUhbmiXyNpTjoFcWI/edit?gid=0#gid=0)
    - Chat with the Chatbot.
    
## Step 4: API Testing

Open Postman then:
1) Submitting Data on Google Sheets
```POST http://localhost:5001/submit```

    Body(JSON):
    {
      "name": "John Doe",
      "address": "123 Main St",
      "contact": "1234567890",
      "email": "john.doe@example.com"
    }
    
    The data will be updated in https://docs.google.com/spreadsheets/d/1AHwkl-9r0kY4O311oIkpu5ao-pCUhbmiXyNpTjoFcWI/edit?gid=0#gid=0

2) Retrieving data from google Sheets
```GET http://localhost:5001/retrieve```

3) Chatbot Interaction
```POST http://localhost:5002/chatbot```

    Body(JSON):
    {
    "message": "what is your name"
    }



