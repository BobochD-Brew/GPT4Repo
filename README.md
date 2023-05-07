# GPT4Repo

GPT4Repo is a simple script that packs all text files in the current folder into a single GPT-4 query and replace them with the result. This script follows the .gitignore rules, also make sure you keep the name gptWorker.py. Please note that this script assumes that your codebase is smaller than GPT-4's 8k context length (it may work with GPT-3 if you have extra-small codes).

## How to use

- Install python3 (make sure you have pip)
- Install the required packages by running the following command: ```python3 -m pip install openai dotenv```
- Create a file named ```.env``` and add your OpenAi api key there ```API_KEY=sk-...```
- Place the script in the desired folder.
- Run the script by executing the following command: ```python3 gptWorker.py```

The script will prompt you to enter a task on the codebase. Once the task is done, the changes are saved, and the script will ask for a new task. Please note that GPT does not have context or history about previous actions.

If you encounter any issues or have any feedback, please don't hesitate to open an issue on our GitHub repository.