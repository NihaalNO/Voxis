# 🎙️Voxis:Local Voice AI Assistant

A private, offline-capable Voice AI Assistant that runs locally on your machine. It listens to your voice, processes your request using **Ollama (Llama 3)**, and speaks back to you with a synthesized voice.

Built with Python, this project ensures complete data privacy by keeping all processing on your local device.

## ✨ Features

- **🗣️ Voice-to-Text**: Uses `SpeechRecognition` (Google API) to convert your speech into text.
- **🧠 Local Intelligence**: Powered by `Ollama` running the powerful **Llama 3** model for intelligent, context-aware responses.
- **🔊 Text-to-Speech**: Uses `pyttsx3` to convert the AI's response back into audible speech.
- **🔒 Privacy First**: Your conversations (text generation) happen locally on your machine.
- **🐍 Python Based**: Simple, readable usage in a Jupyter Notebook.

## 🛠️ Prerequisites

Before you begin, ensure you have the following installed:

1.  **Python 3.x**
2.  **[Ollama](https://ollama.com/)**: This is required to run the Llama 3 model locally.
    -   Download and install Ollama from [ollama.com](https://ollama.com/).
    -   Pull the Llama 3 model by running the following command in your terminal:
        ```bash
        ollama pull llama3
        ```

## 📦 Installation

1.  Clone this repository or download the source code.
2.  Install the required Python libraries:

    ```bash
    pip install speechrecognition ollama pyttsx3 pyaudio
    ```
    *Note: `pyaudio` may require additional system-level audio dependencies depending on your OS (e.g., `portaudio`).*

## 🚀 Usage

1.  Open the `main.ipynb` file in Jupyter Notebook or VS Code.
2.  Run the cells in order to satisfy dependencies and define the helper functions (`listen`, `think`, `speak`).
3.  Execute the final cell containing the `main()` loop.
4.  **Speak!** The assistant will print "Listening..." when it's ready.
    -   Say "Exit", "Stop", or "Quit" to end the session.

### Example Interaction

> **Assistant**: Hello, I am ready. You can start speaking.
>
> **You**: "What is the capital of France?"
>
> **Assistant**: (Thinking...)
>
> **Assistant**: "The capital of France is Paris."

## 🔧 Troubleshooting

-   **Microphone issues**: Ensure your microphone is set as the default recording device in your OS settings.
-   **Ollama connection error**: Make sure the Ollama app is running in the background before starting the script.
-   **"PyAudio" installation fails**: on Windows, pip usually handles this fine. On Linux/Mac, you might need to install `portaudio19-dev` or similar via your package manager.

## 📜 License

This project is open-source and available under the **MIT License**.
