
# Lord of the Rings Chatbot

**This project is a simple chat bot that answers questions related to Lord of the rings.** I made this project to get some experience with adding the ability for the chatbots to call functions. The chatbot can call 2 different functions:

1. The first can generate an image of a Lord of the rings character if you provide it with a name and then ask it to generate an image.
2. The other function allows it to access a genealogy function that will provide information related to the genealogies of most major characters in Lord of the rings.

# To do:
1. Add in the ability to switch between different models
2. Add text streaming for responses


# Lord of the Rings Chat App Setup Guide

## Prerequisites

- Python 3.8 or higher
- OpenAI API key 

## Installation

1. Clone or download the project repository.

2. Install the required dependencies:
   ```bash
   pip install openai gradio pillow python-dotenv anthropic httpx
   ```

3. Create a `.env` file in your project root directory with your API keys:
   ```
   OPENAI_API_KEY=your_openai_api_key
   ANTHROPIC_API_KEY=your_anthropic_api_key
   ```

## Running the Application

1. Open a Jupyter notebook or Python script and import the code.

2. Execute the code blocks in order, ensuring that all functions and variables are defined.

3. The application will launch Gradio interface automatically at the end. You'll see a local URL where the app is hosted (typically http://127.0.0.1:7879).

4. If you want to run the app without launching a browser window, use:
   ```python
   ui.launch(inbrowser=False)
   ```

5. For a public link (temporary, for sharing), use:
   ```python
   ui.launch(share=True)
   ```

## Features

- **Character Information**: Ask about Lord of the Rings characters to get their genealogy data.
- **Image Generation**: The app automatically generates images of requested characters.
- **Streaming Responses**: Responses appear word by word for a more engaging experience.

## Example Usage

1. Ask about a character:
   ```
   Tell me about Frodo's family history
   ```

2. Request an image:
   ```
   Show me what Gandalf looks like
   ```

3. Ask general Lord of the Rings questions:
   ```
   What is the One Ring?
   ```

## Troubleshooting

- If you encounter SSL verification issues, the code already includes workarounds.
- Make sure your API keys are valid and have enough credits for both chat completions and image generation.
- Check that the correct model is specified in the `MODEL` variable (currently set to "gpt-4o-mini").
