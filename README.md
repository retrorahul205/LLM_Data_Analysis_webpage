# 🐰 Talking Rabbitt AI – Conversational Data Analysis

Talking Rabbitt AI is a simple AI-powered data analysis tool that allows users to upload a CSV file and ask questions about the data using natural language.

The system uses a **Large Language Model (Llama 3.1 via Groq API)** to interpret questions and provide insights, along with automatic visualizations.

---

# 🚀 Features

• Upload CSV datasets
• Ask questions about the data in plain English
• AI-generated insights using an LLM
• Automatic data visualization using Plotly
• Simple and interactive Streamlit interface

---

# 🧠 Tech Stack

| Component       | Technology         |
| --------------- | ------------------ |
| Frontend UI     | Streamlit          |
| Data Processing | Pandas             |
| Visualization   | Plotly             |
| LLM Model       | Llama-3.1 via Groq |
| Language        | Python             |

---

# 📁 Project Structure

```
talking-rabbitt-mvp
│
├── app.py                # Main Streamlit application
├── requirements.txt      # Python dependencies
├── sample_sales.csv      # Example dataset
├── .streamlit
│     └── secrets.toml    # API key configuration (not included in repo)
└── README.md
```

---

# ⚙️ Setup Guide (Run Locally)

Follow these steps to run the project on your local machine.

---

## 1️⃣ Clone the Repository

```
git clone https://github.com/retrorahul205/LLM_Data_Analysis_webpage.git
cd talking-rabbitt-mvp
```

---

## 2️⃣ Create a Virtual Environment

Create a Python virtual environment.

```
python -m venv venv
```

---

## 3️⃣ Activate the Virtual Environment

### Windows

```
venv\Scripts\activate
```

### Mac / Linux

```
source venv/bin/activate
```

---

## 4️⃣ Install Dependencies

Install the required Python packages.

```
pip install -r requirements.txt
```

---

## 5️⃣ Add Your Groq API Key

Create a folder named:

```
.streamlit
```

Inside it create a file:

```
secrets.toml
```

Add your API key like this:

```
GROQ_API_KEY="your_groq_api_key_here"
```

You can get a free API key from:

https://console.groq.com

---

## 6️⃣ Run the Application

Start the Streamlit server.

```
streamlit run app.py
```

Your browser will open automatically at:

```
http://localhost:8501
```

---

# 📊 Example Usage

1. Upload the provided **sample_sales.csv** dataset
2. Ask a question like:

```
Which region had the highest revenue in Q1?
```

3. The system will generate:

• AI insight explaining the result
• Automatic visualization of the data

---

# 🧪 Example Dataset

The included dataset contains sample sales data with the following columns:

```
region
quarter
revenue
units_sold
```

---

# 🔐 Security Note

The `.streamlit/secrets.toml` file is **not included in the repository** because it contains API keys.

Each user must create their own `secrets.toml` file and add their own **Groq API key**.

---

# 📌 Future Improvements

• Allow AI to automatically generate Pandas queries
• Support multiple datasets
• Add more advanced analytics questions
• Deploy the application online

---

