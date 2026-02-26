# AI Data Visualization Agent

AI Data Visualization Agent is a Streamlit app that lets you upload a CSV dataset, ask natural-language questions, and receive AI-generated analysis and visualizations powered by Together AI and the E2B Code Interpreter.

## Features
- Upload CSV files and preview your data.
- Ask questions about your dataset in natural language.
- Generate plots, tables, and insights with an LLM + sandboxed Python execution.

## Prerequisites
- Python 3
- Together AI API key
- E2B API key

## Setup
```bash
pip install -r requirements.txt
```

## Run the app
```bash
streamlit run app.py
```

## Usage
1. Open the app in your browser after running Streamlit.
2. Enter your Together AI API key and E2B API key in the sidebar.
3. Upload a CSV file.
4. Type a question about your data and click **Analyze**.

## Notes
- The app reads data from the uploaded CSV only.
- The model can be selected from the dropdown in the sidebar.
