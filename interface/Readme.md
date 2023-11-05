# An Emoji-based Music Understanding and Generation Interface
Emotion is at the heart of music AI research, and we've created an innovative interface that brings emotions and music together in a unique way. In our project, we harness the power of emojis, a universally recognized medium for expressing emotions in text-based communication, to convey the emotional depth of music. Check out the [public website here](https://cassie72.pythonanywhere.com/).

Our system comprises three major components:

* Emoji-Based Music Representation: We've developed an innovative approach to representing music with emojis.  By treating lyric texts as intermediate weak labels, our system learns to associate music with emojis in a weakly supervised fashion.  This enables a nuanced and emotional connection to music.

* Emoji-to-Music Generation: The heart of our system lies in the generation of music from emojis.  We've created a pipeline that uses a large language model to convert emojis into detailed music descriptions through prompt engineering.  Subsequently, a dedicated music generation model brings these descriptions to life, resulting in the creation of music clips that capture the intended emotional essence.

* Emoji-Enhanced Music Interface: Our project features an intuitive emoji-based music interface.  This interface not only visually conveys emotions at both the song and segment levels through emoticons but also empowers users to interact with music in innovative ways.  Users can search for and generate songs based on their emotional preferences, making the listening experience more engaging and personalized.

## Overview
* [templates/](templates): This directory holds all the HTML code essential for building the user interface of our project.
* [static/js/](static/js): Inside this folder, you'll find all the JavaScript code that powers the interactive features of our interface.
* [static/css/](static/css): You can access the CSS code responsible for styling and layout design in our interface here.
* [static/music/](static/music): contains all the human-composed music tracks.
* [static/pregenrated_music/](static/pregenerated_music): contains all the AI-generated music pieces that showcase the innovative capabilities of our system.
* [init1.py](init1.py): contains the flask code.
* [emoji_MusicGen.py](emoji_MusicGen.py): contains the emoji-based music generation prompt engineering method.

## Getting Started
To get started with this project, follow these steps:
1. Clone the repository by manually downloading it and then
```bash
cd yourproject
```
2. Create and activate a virtual environment (optional but recommended);

3. Install the dependencies of the interface part using the `requirements.txt` file;

4. To enable the generation functionality in the interface, you need to install Audiocraft and OpenAI packages:
```bash
!pip install -U git+https://github.com/facebookresearch/audiocraft
```
```bash
!pip install openai
```
5. Run init1.py file using "python init1.py" command from the terminal.
6. Now create another tab in your browser, type "127.0.0.1:5000" in the address bar.
You should be able to see a web page with the music player interface.
