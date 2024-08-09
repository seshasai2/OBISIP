# Voice Assistant

This is a simple Python-based voice assistant that can listen to your commands, respond with spoken output, tell you the time or date, and perform a basic Google search.

## Features

- **Speech Recognition:** Listens to your voice commands using `speech_recognition`.
- **Text-to-Speech:** Responds with spoken output using `pyttsx3`.
- **Current Time and Date:** Tells you the current time or date when requested.
- **Google Search:** Performs a basic Google search and reads out the top 5 results.
- **Command Handling:** Responds to simple commands like "hello", "time", "date", "search", and "stop".

## Requirements

To run this voice assistant, you need to install the following Python libraries:

```bash
pip install SpeechRecognition pyttsx3 requests beautifulsoup4
```

## Usage

1. **Run the script:**
   ```bash
   python voice_assistant.py
   ```

2. **Commands:**
   - Say "hello" to greet the assistant.
   - Ask for the "time" or "date" to get the current time or date.
   - Say "search" followed by your query to perform a Google search.
   - Say "stop" to terminate the assistant.

3. **Example Commands:**
   - "Hello"
   - "What time is it?"
   - "What is the date today?"
   - "Search Python programming tutorials"
   - "Stop"

## How It Works

- **Listening:** The assistant uses your microphone to listen for commands. It has a timeout of 5 seconds and a phrase time limit of 5 seconds.
- **Speech Recognition:** Converts spoken language into text using Google Web Speech API.
- **Text-to-Speech:** Converts the text responses back into spoken language.
- **Web Scraping:** Fetches search results from Google using `requests` and `BeautifulSoup`.

## Limitations

- The search feature only fetches the titles of the top 5 results and reads them out.
- It requires an active internet connection for the search feature and Google Web Speech API.

## License

This project is licensed under the MIT License.
