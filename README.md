# AI DEMO

## Prerequisites
- Git
- Python 3.12+
- pip (Python package manager)

## Project Clone
```bash
git clone <repository-url>
cd <project-directory>
```

## Environment Configuration

### 1. Environment Variables Setup
Copy the example environment file:
```bash
cp .env.example .env
```

### 2. Fill in Environment Variables
Open the `.env` file and populate the following variables:

#### Groq API
- **URL**: `https://console.groq.com/`
- Go to Groq Console
- Create an account
- Generate an API key
- Paste the API key in `.env` as `GROQ_API_KEY`

#### Tavily API
- **URL**: `https://tavily.com/`
- Visit Tavily website
- Sign up for an account
- Generate an API key
- Add to `.env` as `TAVILY_API_KEY`

#### Langsmith Tracing
- **URL**: `https://smith.langchain.com/`
- Create a Langsmith account
- Generate project and API keys
- Add to `.env`:
  - `LANGCHAIN_TRACING_V2=true`
  - `LANGCHAIN_API_KEY=your_api_key`
  - `LANGCHAIN_PROJECT=your_project_name`

### 3. Install Dependencies
Use whichever package manager suits you
```bash
pip install -r requirements.lock
```

## Running the Project
Open and run the Jupyter notebook:
```bash
jupyter notebook demo.ipynb
```

## Troubleshooting
- Ensure all API keys are correctly copied
- Check internet connectivity
- Verify Python and pip versions

## Additional Notes
- Keep your `.env` file private
- Do not commit sensitive credentials to version control