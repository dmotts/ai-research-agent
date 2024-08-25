# AI Research Agent

## Project Overview

AI Research Agent is a versatile application that leverages multiple tools to conduct thorough research on any topic. The application integrates web search, website scraping, and summarization capabilities, all powered by OpenAI's language model. The agent is designed to gather, analyze, and summarize factual information, ensuring that the research output is accurate and well-supported by data.

## Features

- **Web Search:** Conduct searches using Serper API to gather information on any topic.
- **Website Scraping:** Scrape websites for relevant content and summarize large texts to extract key information.
- **Summarization:** Use AI-driven summarization techniques to condense large amounts of data into concise reports.
- **Streamlit Web App:** A user-friendly interface to input research queries and receive detailed responses.
- **FastAPI Endpoint:** Expose the research capabilities as an API for programmatic access.

## Setup Instructions

### Prerequisites

- Python 3.x
- Poetry package manager
- API Keys for:
  - Browserless (for web scraping)
  - Serper (for web search)
  - OpenAI (for language model)
- Optional: A `.env` file to store environment variables

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dmotts/ai-research-agent.git
   cd ai-research-agent
   ```

2. **Install dependencies:**
   ```bash
   poetry install
   ```

3. **Set up environment variables:**
   You can either export the required environment variables in your shell or create a `.env` file in the root directory with the following content:
   ```dotenv
   BROWSERLESS_API_KEY=your_browserless_api_key
   SERP_API_KEY=your_serper_api_key
   OPENAI_API_KEY=your_openai_api_key
   ```

4. **Run the application locally:**
   ```bash
   poetry run streamlit run app.py
   ```

5. **Access the Streamlit app:**
   Open your web browser and go to `http://localhost:8501` to interact with the AI Research Agent.

### Running the FastAPI Server

If you want to expose the research agent as an API:

1. **Start the FastAPI server:**
   ```bash
   poetry run uvicorn app:app --reload
   ```

2. **Access the FastAPI endpoint:**
   You can send POST requests to `http://localhost:8000/` with a JSON payload containing the research query.

## Usage

- **Streamlit Interface:** Enter your research goal in the text input field, and the agent will perform the research, presenting you with a detailed summary of the findings.
- **API Endpoint:** Use the FastAPI endpoint to integrate the research agent into other applications or services.

## Contributions

Contributions are welcome! It only takes five (5) steps!

To contribute:

1) Fork the repository.

2) Create a new branch: `git checkout -b my-feature-branch`.

3) Make your changes and commit them: `git commit -m 'Add some feature'`.

4) Push to the branch: `git push origin my-feature-branch`.

5) Open a pull request.

Please ensure your code follows the project's coding standards and includes tests where appropriate.

## Let's Connect

If you find this project useful, please consider connecting with me on GitHub:

[Daley Mottley (dmotts)](https://github.com/dmotts)
