# API Setup Guide

The application now supports both **Gemini** and **OpenAI** APIs. You only need one of them.

## Option 1: Using Gemini API (Recommended for you)

1. Set your Gemini API key as an environment variable:
   ```bash
   export GEMINI_API_KEY="your_gemini_api_key_here"
   ```

2. Set your WolframAlpha App ID:
   ```bash
   export WOLFRAM_APP_ID="your_wolfram_app_id_here"
   ```

3. Run the app:
   ```bash
   /Users/bai/research/SocraticAI/.venv/bin/python app.py
   ```

## Option 2: Using OpenAI API

1. Set your OpenAI API key:
   ```bash
   export OPENAI_API_KEY="your_openai_api_key_here"
   export OPENAI_ORG="your_openai_org_id_here"  # Optional
   ```

2. Set your WolframAlpha App ID:
   ```bash
   export WOLFRAM_APP_ID="your_wolfram_app_id_here"
   ```

3. Run the app:
   ```bash
   /Users/bai/research/SocraticAI/.venv/bin/python app.py
   ```

## Quick Start with Gemini

Create a file `.env` and add:
```bash
export GEMINI_API_KEY="your_gemini_api_key"
export WOLFRAM_APP_ID="your_wolfram_app_id"
```

Then run:
```bash
source .env
/Users/bai/research/SocraticAI/.venv/bin/python app.py
```

## Model Selection

- **Gemini**: Uses `gemini-1.5-flash` by default (fast and efficient)
- **OpenAI**: Uses `gpt-3.5-turbo` by default

The application automatically detects which API key is available and uses the corresponding service.
