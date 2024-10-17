# AutoGen Multi-Agent Framework

## Overview

The **AutoGen Multi-Agent Framework** is a versatile project that leverages the **AutoGen** library to facilitate the creation and management of intelligent, conversational agents. This framework encompasses various use-cases, including report generation, blog writing, multi-agent conversations, customer onboarding, financial analysis, and interactive gaming through conversational chess.

## Features

- **Planning and Stock Report Generation**: Automate the creation of detailed stock performance reports using agents that plan, write, and execute code to gather and analyze financial data.

- **Reflection and Blogpost Writing**: Generate engaging and concise blog posts with reflective feedback mechanisms to ensure content quality.

- **Multi-Agent Conversation**: Set up conversations between multiple agents, retaining memory of interactions for coherent dialogues.

- **Sequential Chats and Customer Onboarding**: Streamline the customer onboarding process through structured, sequential agent interactions that gather personal information and preferences.

- **Coding and Financial Analysis**: Integrate coding tasks with financial data analysis to produce insightful visualizations and reports.

- **Tool Use and Conversational Chess**: Create interactive chess games where agents can make moves, visualize the board, and engage in friendly chitchat to enhance the gaming experience.

## Configuration

Set up your environment variables by creating a `.env` file in the `autogen` directory:

```dotenv
OPENAI_API_KEY=your_openai_api_key_here
```

## Project Structure

```
autogen/
├── .gitignore
├── requirements.txt
├── utils.py
├── planning_and_stock_report_generation.ipynb
├── reflection_and_blogpost_writing.ipynb
├── multi-agent_conversation.ipynb
├── sequential_chats_and_customer_onboarding.ipynb
├── coding_and_financial_analysis.ipynb
├── tool_use_and_conversational_chess.ipynb
└── ...
```

- **.gitignore**: Specifies intentionally untracked files to ignore.
- **requirements.txt**: Lists project dependencies.
- **utils.py**: Contains utility functions for the project.
- ***.ipynb**: Jupyter Notebooks demonstrating various multi-agent applications.

## Usage

Each Jupyter Notebook in the `autogen` directory showcases a different application of the multi-agent framework. To explore these:

1. Navigate to the `autogen` directory.
2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

3. Open the desired notebook and follow the instructions within to execute and understand the agent interactions.

### Example: Planning and Stock Report Generation

This notebook demonstrates how to set up agents to generate a stock performance report for Nvidia over the past month. It includes agents for planning, engineering, writing, and executing code to gather and visualize stock data.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or additional features.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- [AutoGen Library](https://github.com/microsoft/autogen): The foundation for building conversational agents.
- [OpenAI](https://www.openai.com/): For providing powerful language models used in agent configurations.
