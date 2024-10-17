# LlamaIndex Project

## Overview

The **LlamaIndex Project** is designed to explore and evaluate various approaches and capabilities of the [LlamaIndex](https://github.com/jerryjliu/llama_index) library. By implementing different strategies and leveraging the flexibility of LlamaIndex, this project aims to demonstrate its effectiveness in handling complex data retrieval, agent-based interactions, and tool integrations.

## Purpose

The primary goal of this project is to test and showcase the diverse functionalities of LlamaIndex through practical implementations. This includes:

- **Agent-Based Systems:** Creating intelligent agents that can retrieve and process financial data.
- **Tool Integration:** Developing and integrating custom tools to enhance data fetching and processing capabilities.
- **Query Engines:** Implementing various query engines to handle different types of data retrieval tasks.
- **Function Calling:** Demonstrating how agents can call functions to perform specific operations based on user queries.

## Features

- **Financial Data Retrieval:** Utilize APIs like Financial Modeling Prep to fetch comprehensive financial information about companies.
- **Agent Creation:** Develop agents equipped with tools to answer financial queries effectively.
- **Router Query Engine:** Implement a router-based query engine to manage and direct queries to the appropriate tools.
- **Tool Calling Mechanism:** Showcase how agents can call predefined functions (tools) to process and respond to user queries.
- **Auto-Retrieval Tools:** Implement tools that automatically retrieve and filter information based on specific criteria.
- **Agentic RAG:** Integrate Retrieval-Augmented Generation (RAG) with agent-based systems to enhance the accuracy and relevance of responses by leveraging external data sources dynamically.
- **Multi Document Agent:** Develop agents capable of handling and synthesizing information from multiple documents simultaneously, enabling comprehensive analysis and more informed decision-making.

## Project Structure

The project is organized into several Jupyter notebooks, each focusing on different aspects of the implementation:

### 1. `agent.ipynb`

This notebook sets up an agentic system to retrieve financial data about companies. It includes:

- **Library Installations:** Installing necessary packages like `llama-index`, `llama-index-llms-anthropic`, and `python-dotenv`.
- **API Key Management:** Loading and managing API keys securely using environment variables.
- **Function Definitions:** Defining functions to fetch stock prices, company financials, and income statements.
- **Tool Integration:** Converting functions into tools that the agent can use.
- **Agent Configuration:** Creating an agent that utilizes the defined tools to answer user queries.
- **Chat Interface:** Demonstrating the agent's ability to respond to queries like fetching Tesla's current stock price and revenue.

### 2. `router_engine.ipynb`

This notebook focuses on building a router query engine over document data. Key components include:

- **Data Loading:** Reading and parsing documents (e.g., `metagpt.pdf`) using `SimpleDirectoryReader`.
- **Indexing:** Creating summary and vector indexes to facilitate efficient data retrieval.
- **Query Engines:** Defining summary and vector query engines with specific configurations.
- **Router Implementation:** Setting up a router query engine that selects the appropriate query engine based on the query type.
- **Query Execution:** Demonstrating queries for document summaries and specific information retrieval.

### 3. `tool_calling.ipynb`

This notebook illustrates the process of defining and utilizing simple and auto-retrieval tools within the LlamaIndex framework. It covers:

- **Tool Definitions:** Creating simple tools like `add` and `mystery` functions and converting them into `FunctionTool` instances.
- **Function Calling:** Demonstrating how the LLM can predict and call these tools based on user prompts.
- **Auto-Retrieval Tools:** Building tools that perform vector-based searches with metadata filtering to retrieve relevant information from documents.

### 4. `multi_document_agent.ipynb`

This notebook demonstrates the creation of a multi-document agent capable of handling and synthesizing information from multiple documents. It includes:

- **Data Loading:** Reading and parsing multiple documents using `SimpleDirectoryReader`.
- **Agent Configuration:** Creating an agent that can retrieve and synthesize information from these documents.
- **Query Execution:** Demonstrating queries that require the agent to retrieve and combine information from multiple documents.

### 5. `auto_retrieval_tools.ipynb`

This notebook showcases the implementation of auto-retrieval tools in LlamaIndex. It includes:

- **Tool Definitions:** Creating tools that perform vector-based searches with metadata filtering to retrieve relevant information from documents.
- **Function Calling:** Demonstrating how the LLM can predict and call these tools based on user prompts.
- **Agentic RAG:** Integrating Retrieval-Augmented Generation (RAG) with agent-based systems to enhance the accuracy and relevance of responses by leveraging external data sources dynamically.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your enhancements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [LlamaIndex](https://github.com/jerryjliu/llama_index) for providing the foundational library.
- [Financial Modeling Prep](https://financialmodelingprep.com/) for their financial data APIs.
- [OpenAI](https://openai.com/) for the LLMs used in this project.