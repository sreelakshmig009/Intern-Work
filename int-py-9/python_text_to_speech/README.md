# python_text_to_speech
## What is pyttsx3 ?
- A python library that will help us to convert text to speech. In short, it is a text-to-speech library.
- It works offline, and it is compatible with Python 2 as well as Python 3.

Installation:

    pip install pyttsx3
In case you receive such errors: 
- No module named win32com.client
- No module named win32
- No module named win32api

Then, install pypiwin32 by typing the below command in the terminal :

    pip install pypiwin32

After successfully installing pyttsx3, import this module into your program.

Usage:

    import pyttsx3

    engine = pyttsx3.init('sapi5')

### What is sapi5?
- Microsoft developed speech API.
- Helps in synthesis and recognition of voice.

Let's take an example

    # Import the required module for text to speech conversion
    import pyttsx3

    # init function to get an engine instance for the speech synthesis
    engine = pyttsx3.init('sapi5')

    # say method on the engine that passing input text to be spoken
    engine.say('Hello sir, how may I help you, sir.')

    # run and wait method, it processes the voice commands.
    engine.runAndWait()