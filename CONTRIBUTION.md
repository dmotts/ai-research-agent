# AI Research Agent: Contributing Guidelines 📄

## Table of Contents
1. [Introduction](#introduction-)
2. [Tech Stack](#tech-stack-)
3. [Installation](#installation-)
4. [Contributing](#contributing-)
   - [Development Workflow](#development-workflow)
   - [Issue Report Process](#issue-report-process)
   - [Pull Request Process](#pull-request-process-)
   - [Contributing Using GitHub Desktop](#contributing-using-github-desktop)
5. [Resources for Beginners](#resources-for-beginners-)
6. [Documentation](#documentation-)
7. [Code Reviews](#code-reviews-)
8. [Feature Requests](#feature-requests-)
9. [Spreading the Word](#spreading-the-word-)
10. [Code of Conduct](#code-of-conduct-)
11. [Thank You](#thank-you-)

## Introduction 🖥️

Welcome to **Customer Support Bot**, a WordPress plugin that allows businesses to automate customer support using AI technology. We are excited to have you contribute to our project! No contribution is too small, and we appreciate your help in improving this plugin.

## Setup Instructions

### Prerequisites

- Python 3.x
- Poetry package manager
- API Keys for:
  - Browserless (for web scraping)
  - Serper (for web search)
  - OpenAI (for language model)
- Optional: A `.env` file to store environment variables

## Installation ⚙️

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

## Contributing 📝

We welcome contributions to **Customer Support Bot**! Please follow these guidelines to ensure a smooth contribution process.

### Development Workflow

- **Work on a New Branch:** Always create a new branch for each issue or feature you are working on.
- **Keep Your Branch Up to Date:** Regularly pull changes from the master branch to keep your branch up to date.
- **Write Clear Commit Messages:** Use descriptive commit messages to explain what your changes do.
- **Test Thoroughly:** Ensure your changes work correctly and do not break existing functionality.
- **Self-Review:** Review your code before submitting to catch any errors or areas for improvement.

### Issue Report Process 📌

1. **Check Existing Issues:** Before creating a new issue, check if it has already been reported.
2. **Create a New Issue:** Go to the project's [issues section](https://github.com/dmotts/customer-support-bot/issues) and select the appropriate template.
3. **Provide Details:** Give a clear and detailed description of the issue.
4. **Wait for Assignment:** Wait for the issue to be assigned to you before starting work.

### Pull Request Process 🚀

1. **Ensure Self-Review:** Make sure you have thoroughly reviewed your code.
2. **Provide Descriptions:** Add a clear description of the functionality and changes in your pull request.
3. **Comment Your Code:** Comment on complex or hard-to-understand areas of your code.
4. **Add Screenshots:** Include screenshots if they help explain your changes.
5. **Submit PR:** Submit your pull request using the provided template, and wait for the maintainers to review it.

### Contributing Using GitHub Desktop

If you prefer using GitHub Desktop, follow these steps:

1. **Open GitHub Desktop:** Launch GitHub Desktop and log in to your GitHub account.
2. **Clone the Repository:** Click on "File" > "Clone Repository" and select the repository to clone.
3. **Create a Branch:** Click on "Current Branch" and select "New Branch" to create a new branch for your work.
4. **Make Changes:** Edit the code using your preferred code editor.
5. **Commit Changes:**
   - In GitHub Desktop, select the files you changed.
   - Enter a summary and description for your commit.
   - Click "Commit to [branch-name]".
6. **Push Changes:** Click "Push origin" to push your changes to GitHub.
7. **Create a Pull Request:**
   - On GitHub, navigate to your forked repository.
   - Click on "Compare & pull request".
   - Review your changes and submit the pull request.
8. **Wait for Review:** Wait for the maintainers to review your pull request.

## Resources for Beginners 📚

If you're new to Git and GitHub, here are some resources to help you get started:

- [Forking a Repo](https://help.github.com/en/github/getting-started-with-github/fork-a-repo)
- [Cloning a Repo](https://help.github.com/en/desktop/contributing-to-projects/creating-an-issue-or-pull-request)
- [Creating a Pull Request](https://opensource.com/article/19/7/create-pull-request-github)
- [Getting Started with Git and GitHub](https://towardsdatascience.com/getting-started-with-git-and-github-6fcd0f2d4ac6)
- [Learn GitHub from Scratch](https://docs.github.com/en/get-started/start-your-journey/git-and-github-learning-resources)

## Documentation 📍

- **Update Documentation:** Document any significant changes or additions to the codebase.
- **Provide Clear Explanations:** Explain the functionality, usage, and any relevant considerations.
- **Use Comments:** Comment your code, especially in complex areas.

## Code Reviews 🔎

- **Be Open to Feedback:** Welcome feedback and constructive criticism from other contributors.
- **Participate in Reviews:** Help review others' code when possible.
- **Follow Guidelines:** Ensure your code meets the project's coding standards and guidelines.

## Feature Requests 🔥

- **Suggest Improvements:** Propose new features or enhancements that could benefit the project.
- **Provide Details:** Explain the rationale and potential impact of your suggestion.

## Spreading the Word 👐

- **Share Your Experience:** Share the project with others who might be interested.
- **Engage on Social Media:** Talk about the project on social media, developer forums, or relevant platforms.

## Code of Conduct 📜

Please note that we have a [Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.

## Thank You 💗

Thank you for contributing to **Customer Support Bot**! Together, we can make a significant impact. Happy coding! 🚀

Don't forget to ⭐ the repository!
