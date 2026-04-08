# AI Document Summarizer

A web-based application that uses AI to generate concise summaries of documents.

## Features

- Upload and summarize documents via a web interface
- AI-powered text summarization
- Clean, simple UI built with Flask and HTML templates

## Tech Stack

- **Backend:** Python 3.12, Flask
- **Frontend:** HTML5 (Jinja2 templates)
- **AI:** Configurable AI summarization backend (e.g., Anthropic Claude, OpenAI)

## Project Structure

```
AI-Document-Summarizer/
├── app.py              # Main Flask application
├── templates/
│   └── index.html      # Web UI template
├── requirements.txt    # Python dependencies
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.12+
- pip

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/sattenapalliakhilesh/ai-document-summarizer-.git
   cd ai-document-summarizer-
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate   # On Windows: .venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   ```bash
   cp .env.example .env
   # Edit .env with your API keys and configuration
   ```

### Running the Application

```bash
python app.py
```

The app will be available at `http://localhost:5000`.

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `FLASK_SECRET_KEY` | Flask session secret key | Yes |
| `AI_API_KEY` | API key for the AI summarization service | Yes |
| `FLASK_DEBUG` | Enable debug mode (`true`/`false`) | No |

## Usage

1. Open the app in your browser at `http://localhost:5000`
2. Upload a document or paste text into the input field
3. Click **Summarize** to generate a summary
4. View and copy the generated summary

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a pull request

## License

This project is licensed under the MIT License.
