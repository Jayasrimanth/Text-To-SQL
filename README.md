# Text-to-SQL with Google Gemini

A simple Streamlit web application that converts natural language questions into SQL queries using the Google Gemini API and executes them against a local SQLite database.

---

## ✨ Features

- **Natural Language to SQL**: Ask questions like "How many students are in the Data Science class?" and get real database results.
- **Interactive Web UI**: Built with Streamlit for a clean and simple user interface.
- **Powered by Gemini**: Uses Google's powerful `gemini-1.5-pro-latest` or `gemini-1.5-flash-latest` models for accurate SQL generation.
- **Local Database**: Connects to a local `student.db` SQLite database that you can easily manage.

---

## 🛠️ Tech Stack

- **Language**: Python 3.10  
- **Framework**: Streamlit  
- **LLM API**: Google Gemini  
- **Database**: SQLite

---

## 🚀 Getting Started

Follow these steps to get a local copy up and running.

### Prerequisites

- Python 3.10 or higher
- A Google AI API Key. You can get one from [Google AI Studio](https://aistudio.google.com/app/apikey).

---

### Installation & Setup

#### 1. Clone the repository

```bash
git clone https://github.com/Jayasrimanth/Text-To-SQL.git
cd your-repo-name
````

#### 2. Create and activate a virtual environment (recommended)

```bash
# Using venv
python -m venv venv
source venv/bin/activate

# Or using Conda
conda create -p venv python=3.10 -y
conda activate ./venv
```

#### 3. Install the required packages

```bash
pip install -r requirements.txt
```

#### 4. Set up your API Key

* Create a file named `.env` in the project root.
* Add your API key to this file:

```env
GOOGLE_API_KEY="YOUR_API_KEY_HERE"
```

#### 5. Initialize the database

Run the `sql.py` script once to create the `student.db` file and populate it with initial data.

```bash
python sql.py
```

---

## 🏃‍♂️ How to Run

Launch the Streamlit application with the following command:

```bash
streamlit run app.py
```

Then open your web browser and navigate to:
[http://localhost:8501](http://localhost:8501)

---
