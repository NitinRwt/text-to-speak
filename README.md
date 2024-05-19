<h1>Text-to-Speech Translation Using gTTS</h1>

<h2>Overview</h2>
This project demonstrates how to use the Google Text-to-Speech (gTTS) library to convert text into speech.<br>
The gTTS library is a Python interface to Google Translate's text-to-speech API. This project can be used to translate text into spoken words in various languages.

<h2>Features</h2>
1. Convert text to speech in multiple languages <br>
2. Save the speech as an audio file <br>
3. Play the generated speech directly

## Installation
1. Clone the repository
   ```bash
   git clone https://github.com/NitinRwt/text-to-speech.git

2. Install the required libraries
   ```bash
   pip install gtts playsound
   
## Usage
1. Basic Usage: Convert text to speech and save it as an MP3 file.
   ```bash
   from gtts import gTTS
   text = "Hello, how are you?"
   tts = gTTS(text=text, lang='en')
   tts.save("hello.mp3")
2. Playing the Audio: Use the playsound library to play the saved MP3 file.
   ```bash
   from playsound import playsound
   playsound("hello.mp3")
3. Multilingual Support: Convert text to speech in different languages.
   ```bash
   from gtts import gTTS
   text = "Bonjour, comment ça va?"
   tts = gTTS(text=text, lang='fr')
   tts.save("bonjour.mp3")
   playsound("bonjour.mp3")



