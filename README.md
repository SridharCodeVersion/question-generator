# AI Question Generator

An application that automatically generates questions from text documents using natural language processing.

## Features

- Upload any .txt document
- Automatic extraction of key sentences
- AI-generated questions based on content
- Downloadable results
- Responsive interface

## How to Use

1. Install requirements:
```bash
pip install -r requirements.txt
```

2. Run the app:
```bash
streamlit run app.py
```

3. Upload a text file and view the generated questions

## Deployment

To deploy on Streamlit Cloud:

1. Create a new repository with these files
2. Connect your Streamlit account to the repository
3. Set the main file path to `app.py`
4. Deploy!

## Technical Details

- Uses NLTK for text processing
- TF-IDF for sentence importance scoring
- T5 transformer model for question generation

## Key Features

**Robust File Handling:**

- Supports any UTF-8 text file
- Handles large documents efficiently
- Proper error messages for invalid files

**Efficient Processing:**

- Uses a smaller T5 model (t5-small-e2e-qg) that works well on CPU
- Caches the model between runs
- Optimized text processing

**User-Friendly Interface:**

- Clear instructions and feedback
- Progress indicators
- Results organized in tabs
- Download option for questions

**Error Handling:**

- Graceful fallbacks if processing fails
- Clear error messages
- Handles edge cases (empty files, etc.)

## How to Run

Create a new directory and add these files

Install dependencies:
```bash
pip install -r requirements.txt
```

Run the app:
```bash
streamlit run app.py
```

## Deployment to Streamlit Cloud

Push this to a GitHub repository

Go to Streamlit Cloud and connect to your repository

Set the main file path to app.py

Click "Deploy"
