

# TTS_Flet_Elevenlabs_API

**README: Text-to-Speech Application using Elevenlabs API**

**Introduction:**
This Python script provides a simple Text-to-Speech (TTS) application using the Elevenlabs API. Users can input text into a text box, select a voice from available options, and play or save the generated audio. The application also provides information about the user's subscription plan, character count, and limits.

**Dependencies:**
- flet: A library for building Flutter-like user interfaces in Python.
- elevenlabs: A library for interacting with the Elevenlabs API for Text-to-Speech functionality.
- requests: Used for making HTTP requests to the Elevenlabs API.
- webbrowser: Opens a web browser for certain actions.
- uuid: Generates UUIDs for file naming.
- os: Operating system-dependent functionality for file handling.
- dotenv: Loads environment variables from a .env file.

**Setup:**
1. Install the required dependencies using:
   ```
   conda create -p venv python==3.10.0
   conda activate venv
   pip install -r requirements.txt
   ```
2. Obtain an API key from Elevenlabs by signing up at [Elevenlabs](https://elevenlabs.io/).
3. Create a `.env` file in the project directory and add your API key:
   ```
   API_KEY=your_api_key_here
   ```

**Usage:**
1. Run the script: `python your_script_name.py`.
2. The application window will appear with a text box, voice selection dropdown, and control buttons.
3. Input text into the text box.
4. Choose a voice from the dropdown.
5. Click the play button to hear the generated audio.
6. Click the save button to save the audio file in the 'out' directory.
7. Information about the user's subscription plan, character count, and limits is displayed.
8. To upgrade the plan, click the "Upgrade Plan" button, which opens the Elevenlabs subscription page in a web browser.

**Important Notes:**
- Ensure that the API key provided in the `.env` file is valid and has the necessary permissions.
- The application checks if the API key is valid alphanumeric characters before execution.
- The default voice is set to the last available voice in the voices list.
- If using the free plan, the application displays information about free characters; otherwise, it indicates a subscriber.
- The application handles character count and limit information, updating it after generating audio.

**Additional Information:**
- For more information about Elevenlabs and their services, visit [Elevenlabs](https://elevenlabs.io/).
- Refer to the official documentation for flet, Elevenlabs, and requests for detailed information on their usage and functionalities.

