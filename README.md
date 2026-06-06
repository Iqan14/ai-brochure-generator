# AI-Powered Brochure Generator

Automatically generates a company brochure by scraping and navigating its website using OpenAI's GPT-4.

## What It Does

- Scrapes a company's website and extracts all links
- Uses GPT-4 to intelligently select the most relevant pages (About, Careers, etc.)
- Fetches content from those pages
- Generates a professional markdown brochure with streaming output

## Tech Stack

- Python, Jupyter Notebook
- OpenAI API (GPT-4.1-mini)
- BeautifulSoup4 for web scraping
- python-dotenv for config

## Setup

1. Clone the repo
```
git clone https://github.com/Iqan14/ai-brochure-generator
cd ai-brochure-generator
```

2. Install dependencies
```
pip install -r requirements.txt
```

3. Add your API key
```
cp .env.example .env
```
Then open `.env` and replace with your real OpenAI API key.

4. Run the notebook
```
jupyter notebook brochure.ipynb
```

## Usage

```python
stream_brochure("HuggingFace", "https://huggingface.co")
stream_brochure("Anthropic", "https://anthropic.com")
```

## Project Structure

```
├── brochure.ipynb     # main notebook
├── scraper.py         # website scraping utilities
├── .env.example       # API key template
├── .gitignore         # ignored files
└── requirements.txt
```

---

Built as part of an AI Engineering course.