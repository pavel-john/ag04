# ag04 - Travel Planning Chatbot

This repository contains the implementation of a travel planning chatbot, inspired by [Microsoft AutoGen's Travel Planning Sample](https://microsoft.github.io/autogen/dev/user-guide/agentchat-user-guide/examples/travel-planning.html). The bot is powered by Azure OpenAI resources and is optimized for use with the GPT-4 model.

Here’s the continuation to finish your README file:

---

## Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone https://github.com/pavel-john/ag04.git
   cd ag04
   ```

2. **Install Dependencies**

   This project uses `pipenv` for environment and dependency management. If you don’t have `pipenv` installed, you can install it using `pip`:

   ```bash
   pip install pipenv
   ```

   After that, install the dependencies:

   ```bash
   pipenv install
   ```

   If you need to activate the virtual environment:

   ```bash
   pipenv shell
   ```

3. **Configure Azure OpenAI**

   - Create a `.env` file based on the provided `.env.example`. Your `.env` should include the necessary configuration for your Azure OpenAI account:

   ```bash
   cp .env.example .env
   ```

   Edit the `.env` file to add your Azure OpenAI credentials and configuration:

   ```env
   AZURE_OPENAI_API_KEY=your_api_key
   AZURE_OPENAI_ENDPOINT=your_endpoint
   AZURE_OPENAI_GPT4_API_TYPE=azure
   AZURE_OPENAI_GPT4_API_VERSION=2023-03-15-preview
   AZURE_OPENAI_GPT4_DEPLOYMENT_MODEL_NAME=gpt-4
   AZURE_OPENAI_O1_API_VERSION=2024-08-01-preview
   AZURE_OPENAI_O1_DEPLOYMENT_MODEL_NAME=o1-preview
   ```

   Replace the placeholders (`your_api_key`, `your_endpoint`, etc.) with the actual values from your Azure OpenAI setup.

4. **Run the Application**

   Once everything is set up, you can start the chatbot by running the `main.py` file:

   ```bash
   python main.py
   ```

   This will initialize the travel planning chatbot, which you can interact with via the terminal or set up further with a UI for better usability.

5. **Testing the Application**

   To verify that the application is working correctly, you can run the provided test suite:

   ```bash
   python -m unittest discover tests/
   ```

   This will run all test cases located in the `tests/` directory.

---

## References

- [Microsoft AutoGen - Travel Planning Example](https://microsoft.github.io/autogen/dev/user-guide/agentchat-user-guide/examples/travel-planning.html)
- [Azure OpenAI Service Documentation](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/)
- [Pipenv Documentation](https://pipenv.pypa.io/en/latest/) 

