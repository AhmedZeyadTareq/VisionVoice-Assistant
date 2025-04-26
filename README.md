# Screenshot Voice Assistant

## Project Title Placeholder

A Python-based desktop assistant that captures your screen, listens for your voice commands, uses OpenAI's Whisper for transcription and GPT-4o for understanding the command in the context of the screen content, and responds verbally using OpenAI's TTS.

## Features

* Captures desktop screenshots in real-time using a dedicated thread.
* Listens for voice input via microphone.
* Uses OpenAI Whisper for accurate speech-to-text transcription.
* Leverages LangChain to manage conversation history and integrate screen content with prompts.
* Utilizes OpenAI GPT-4o for multimodal understanding of the user's prompt and the current screenshot.
* Provides spoken responses using OpenAI Text-to-Speech (TTS).
* Displays the current screenshot in a window.
* Clean shutdown of resources (screenshot thread, audio listener, OpenCV windows).

## Requirements

* Python 3.7+
* An OpenAI API Key.
* Necessary system dependencies for `PyAudio` (often PortAudio) and `opencv-python`.

All required Python packages are listed in `requirements.txt`.

## Setup

1.  **Clone the Repository:**
    ```bash
    git clone <your-repo-url>
    cd <your-repo-directory>
    ```

2.  **Create a Virtual Environment (Recommended):**
    ```bash
    # For Windows PowerShell
    python -m venv .venv
    .\.venv\Scripts\Activate.ps1

    # For Windows Command Prompt
    python -m venv .venv
    .venv\Scripts\activate.bat

    # For macOS/Linux
    python3 -m venv .venv
    source .venv/bin/activate
    ```

3.  **Install Dependencies:**
    With the virtual environment activated:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up OpenAI API Key:**
    Create a file named `.env` in the root of your project directory (the same place as `screen_asis.py` and `requirements.txt`). Add your OpenAI API key to this file:
    ```dotenv
    OPENAI_API_KEY='your-api-key-here'
    ```
    Replace `'your-api-key-here'` with your actual OpenAI API Key. Do **not** commit this file to GitHub. Add `.env` to your `.gitignore` file.

5.  **Install PortAudio (for PyAudio):**
    `PyAudio` requires the PortAudio library to be installed on your system.
    * **Windows:** Pre-built wheels often include PortAudio, so `pip install PyAudio` might work directly. If not, you might need to install it separately or use a different `pyaudio` wheel.
    * **macOS (using Homebrew):** `brew install portaudio`
    * **Linux (Debian/Ubuntu):** `sudo apt-get install portaudio19-dev`
    * **Linux (Fedora):** `sudo dnf install portaudio-devel`

## How to Run

With your virtual environment activated, run the main script:

```bash
python screen_asis.py
 ```


👨‍💻 Developed By Eng. Ahmed Zeyad Tareq 📌 Data Scientist | 🎓 Master of AI Engineering

📷 Instagram: @adlm7

🔗 LinkedIn: AhmedZeyadTareq

📊 Kaggle: AhmedZeyadTareq

📄 License MIT License © Ahmed Zeyad Tareq

🌟 Support If you like this project, give it a ⭐ on GitHub and share Got ideas for improvements? Feel free to open a Pull Request or create an Issue. 🚀
