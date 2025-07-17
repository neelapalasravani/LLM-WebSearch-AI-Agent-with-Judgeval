
# LLM Web Search AI Agent with Judgeval
Greetings! Here is an AI agent that helps you reply to questions with the power of web search and large language models. It also has smart tracing and evaluation tools to help you check and improve your results using judgeval SDK.

## What does this agent do?

- Tavily employs the web for searching for information
- Uses first-rate LLMs from Together AI(such as Llama-3.3-70B) to answer your questions
- Trace and evaluates the answers for quality using Judgeval
## Getting Started

### 1. Clone the Repository

Take a copy of the code first:
```bash
git clone https://github.com/neelapalasravani/LLM-WebSearch-AI-Agent-with-Judgeval.git
cd LLM-WebSearch-AI-Agent-with-Judgeval
```
### 2. Install the Requirements

Make sure you have Python 3.8 or higher. Then, install the packages required:
```bash
pip install -r requirements.txt
```
### 3. Add Your API Keys

Create the following in a `.env` file in the project directory. 
```

JUDGMENT_API_KEY=your_judgeval_api_key
JUDGMENT_ORG_ID=your_judgeval_org_id
TAVILY_API_KEY=your_tavily_api_key
TOGETHER_API_KEY=your_together_api_key

#OPENAI_API_KEY=your_openai_api_key #if necessary
```
### 4. Run the Agent

Run the agent with:
```bash
python main.py
You will be asked to enter a question. The agent will:

- Web search for helpful context
- Respond to your question using an LLM
- Show the response and the context it obtained
-  Assess how well the response is (basic and advanced evaluation)
## Example

```
❓ Ask a web search question: What is the capital of France?
Agent's Answer:
capital of France is Paris.
```.
 What were you thinking the response would be (for eval)?: Paris
 Basic Evaluation (String Containment): ✅ Match
Running LLM-based evaluation (GPT-4.1).
```
## Want to Extend or Customize?

- Add more LLMs with new functions like `run_llm`
- Compare different models' responses
- Change prompts or evaluation rules as necessary
## Troubleshooting

- API key errors? Check your `.env` file again.
- Judgeval project limit quota issues? Try redoing the project with a different name or waiting for a few minutes then trying again.
- Python errors? Check that you are running the latest version of Python and packages.
## What's in this folder?

- `main.py`: The main agent code
- `requirements.txt`: All Python packages you need
- `.env.example`: What environment variables you need
- `README.md`: This README
## Need Assistance?

If you're stuck, just open an issue in the repository. Happy coding!
