# Image-Recognition-Using-AI

Project Overview:

This project explores the combination of speech recognition, image analysis, and text-to-speech for a user-friendly experience. It utilizes:

Whisper: for converting user voice input to text.
Llava pre-trained model: for analyzing a user-uploaded image.
gTTS: for converting the image analysis results into audio feedback for the user.
Developed by:

Ravi Solanki (BSc Data Science, Gujarat University): GitHub: (https://github.com/ravisolanki2674) | LinkedIn: https://www.linkedin.com/in/ravisolanki | Email: solankiravi2674@gmail.com

Meet Solanki (BSc AIML, Gujarat University): GitHub: [invalid URL removed] | LinkedIn: [invalid URL removed] | Email: 

Poria Jenil (BSc AIML, Gujarat University): GitHub: [invalid URL removed] | LinkedIn: [invalid URL removed] | Email:

Manav Patel (BSc AIML, Gujarat University): GitHub: [invalid URL removed] | LinkedIn: [invalid URL removed] | Email:

Ansh Darji (BSc AIML, Gujarat University): GitHub: [invalid URL removed] | LinkedIn: [invalid URL removed] | Email:

Project Context:

This project was developed during a hackathon at Ahmedabad University. The purpose was to showcase the potential of combining various AI tools to create an interactive and accessible application.

Technology Stack:

Python
Gradio
Whisper
Llava
gTTS
Execution Environment:

Google Colab

## How It Works 🛠️

1. User Interaction:

The Gradio interface launches in your web browser, accessible from within Colab.
The user sees two input widgets:
A microphone icon for recording audio input.
A file upload button for selecting an image.

2. Processing:

Whisper: When the user records audio, the recorded data is sent to the Whisper API (or a locally implemented Whisper function). Whisper converts the audio to text.
Llava Model: Once the user uploads an image, it's sent to the pre-trained Llava model. The model performs its designated analysis on the image, depending on its purpose:
Object Detection: It identifies and locates objects within the image and might return a list of detected objects and their locations.
Image Classification: It classifies the image into a predefined category (e.g., landscape, portrait, animal).
Caption Generation: It generates a caption describing the content of the image.
Text Processing: The text output received from either Whisper (speech recognition) or Llava (image analysis) is processed further (if needed) based on your project's logic. This might involve combining the information or formatting the text for better readability.

3. Output:

Speech to Text: The transcribed text from the user's voice is displayed in a designated output box within the Gradio interface.
Audio Response: The processed text output (from either speech or image analysis) is sent to the gTTS library. gTTS converts the text into an audio file.
Audio Playback: The generated audio file is automatically played through your computer's speakers, providing the user with spoken feedback about the image analysis results.


Overall, the project creates a loop where user interaction triggers processing through Whisper and the Llava model, leading to a combined textual and audio response that describes the user's voice input and the analysis of the uploaded image.
