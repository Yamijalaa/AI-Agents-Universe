###### Financial Analysis Crew ##########
Financial Analysis Crew is a Python application that leverages the power of the Crew library to coordinate the efforts of different agents in analyzing a company's financial health and providing investment recommendations.
Prerequisites
Before running this application, ensure that you have the following installed:

-Python 3.6 or later
-Poetry (for dependency management)


# Steps
Installation

Clone the repository:

git clone https://github.com/your-username/financial-analysis-crew.git

Sure, here's a detailed README file for your project:
Financial Analysis Crew
Financial Analysis Crew is a Python application that leverages the power of the Crew library to coordinate the efforts of different agents in analyzing a company's financial health and providing investment recommendations.
Prerequisites
Before running this application, ensure that you have the following installed:

Python 3.6 or later
Poetry (for dependency management)

Installation

Clone the repository:

Copy codegit clone https://github.com/your-username/stock_analyst.git

Navigate to the project directory:
cd stock_analyst

Install the dependencies using Poetry:
poetry install

Create a .env file in the project root directory and add the necessary environment variables (if any).

- Install Ollma
- Create custom local LLM made for CrewAI

Project Structure

main.py: The entry point of the application.
agents/: Directory containing the agent implementations.

__init__.py: Initializes the agents module.
stock_analysis_agents.py: Defines the agents used in the analysis process.


tasks/: Directory containing the task implementations.

__init__.py: Initializes the tasks module.
stock_analysis_tasks.py: Defines the tasks performed by the agents.


tools/: Directory containing the tool implementations (if any).
pyproject.toml: Poetry configuration file for dependency management.
poetry.lock: Locked dependency versions managed by Poetry.

Agents
The application uses the following agents:

ResearchAnalystAgent: Responsible for researching and gathering information about the company.
FinancialAnalystAgent: Responsible for analyzing the company's financial statements and filings.
InvestmentAdvisorAgent: Responsible for providing investment recommendations based on the analysis.

Tasks
The application defines the following tasks:

research: Task for researching and gathering information about the company.
financial_analysis: Task for analyzing the company's financial statements.
filings_analysis: Task for analyzing the company's filings.
recommend: Task for providing investment recommendations based on the analysis.

Contributing
Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.


# Tips

- If using multiple models,

# Warnings & Recommendations

- Ollama doesn't work with Async tasks and a bunch of newer CrewAI features yet.
- Lose context. Be very explicit in tasks. Not generic.



# Resources

- Want to find out which LLMs support which features in CrewAI? Here's the link for you:
  - https://python.langchain.com/docs/integrations/llms/
- Learn more about Modelfiles:
  - https://github.com/ollama/ollama/blob/main/docs/modelfile.md
- Check out CrewAI's instructions for working with Ollama and running LLMs locally:
  - https://docs.crewai.com/how-to/LLM-Connections/#connect-crewai-to-llms
