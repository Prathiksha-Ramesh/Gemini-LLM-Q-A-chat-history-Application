# Gemini LLM Q&A chat history Application
## Overview

The **Gemini LLM Application** is a simple conversational Q&A application built using Streamlit. It leverages Google's Generative AI for the LLM functionality and supports environment-specific configurations through the use of Python's `dotenv` module.

## Features
- **Conversational Interface:** A user-friendly web interface where users can input questions and receive responses from the LLM.
- **Chat History:** The application displays the chat history, showing both user queries and the LLM's responses.
- **Environment Configuration:** Use of `.env` files for environment-specific settings like API keys and other secrets.
- **Apache Licensed:** The project is open-source and distributed under the Apache License.

## Project Structure

``` bash 
Gemini_LLM_Application/
│
├── app.py # Main application file
├── .env # Environment variables
├── requirements.txt # List of dependencies
├── .gitignore # Git ignore file
├── LICENSE # Apache License file
├── venv/ # Virtual environment directory (not included in git)
└── README.md # This file
```


### app.py
This is the main application file that initializes the Streamlit interface, handles user input, and communicates with the LLM to generate responses. The responses are then displayed alongside the chat history.

### .env
This file contains environment-specific variables such as API keys, which are not committed to version control due to the `.gitignore` settings.

### requirements.txt
This file contains a list of Python dependencies needed to run the application. The dependencies are as follows:

- **streamlit:** For creating the web interface.
- **google-generativeai:** For interacting with the Google Generative AI service.
- **python-dotenv:** For loading environment variables from the `.env` file.

### .gitignore
This file ensures that sensitive information (like the `.env` file) and unnecessary files (like the `venv` folder) are not tracked by Git.

### LICENSE
This project is licensed under the Apache License, Version 2.0.

## Installation

### Prerequisites
- Python 3.x
- Virtual environment (optional but recommended)

### Setup

1. **Clone the Repository:**

``` bash 

git clone https://github.com/your-repo/Gemini_LLM_Application.git
cd Gemini_LLM_Application

```


2. **Create a Virtual Environment:**

``` bash 
python -m venv venv
source venv/bin/activate # On Windows use venv\Scripts\activate

``` 


3. **Install Dependencies:**

``` bash 
pip install -r requirements.txt
```


4. **Configure Environment Variables:**
- Rename `.env.example` to `.env`
- Update the variables as needed (e.g., API keys).

5. **Run the Application:**

``` bash 
streamlit run app.py
``` 


## Usage

- Navigate to `http://localhost:8501` in your browser.
- Enter your query in the input field and press "Ask the question".
- View the LLM's response along with the chat history.

## Screenshot

![Application Screenshot](Screenshot%202024-08-23%20082859.png)

## License
This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.



