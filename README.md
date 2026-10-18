# College Assistant

A Streamlit college assistant that answers questions using the academic handbook and fee structure PDFs.

## Run locally

1. Create and activate a Python virtual environment.
2. Install dependencies: `pip install -r requirements.txt`
3. Copy `.env.example` to `.env` and add your `GROQ_API_KEY`.
4. Start the app: `streamlit run app.py`

## Deploy to Streamlit Community Cloud

1. Push this repository to GitHub.
2. In Streamlit Community Cloud, create an app from the repository and select `app.py` as the entry point.
3. Add `GROQ_API_KEY` in the app's **Settings → Secrets** using TOML syntax:

   ```toml
   GROQ_API_KEY = "your-key"
   ```

The PDF files are used as the app's knowledge base and should remain in the repository. Local `.env` files and Streamlit secrets are ignored by Git.
