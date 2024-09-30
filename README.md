# A Tool for Text Extraction and Reading

## Project Overview

This project demonstrates a bilingual AI tool using Hugging Face pipelines for **text summarization**, **translation**, and **text-to-speech conversion**. The project provides functionality in both **English** and **Arabic**. It aims to explore the capabilities of Hugging Face models in natural language processing (NLP), text-to-audio, and audio transcription tasks.

### Features:
- **Text Summarization**: Generate concise summaries of input text using state-of-the-art Hugging Face models.
- **Translation**: Translate summarized English text into Arabic.
- **Text-to-Speech**: Convert text (both English and Arabic) into speech using `gTTS`.
- **Audio Transcription**: Convert uploaded audio to text using the Whisper and Wav2Vec2 models.
  
This project is part of the AI course at Tuwaiq Academy, fulfilling the task of building a bilingual application (Arabic & English).

## Table of Contents
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Models and Pipelines](#models-and-pipelines)
- [Usage](#usage)
- [Demo](#demo)
- [Future Work](#future-work)

  
### Files:
- **app.py**: This file contains the Gradio interface code for summarizing text, translating it, converting it into speech, and handling audio-to-text transcription.
- **requirements.txt**: List of Python packages required to run the project.
- **presentation_slides.pdf**: A set of slides detailing the project objectives, implementation, and results (add your file here).
- **examples/**: A folder for storing example files like input texts or audio (add example files here).

## Models and Pipelines

This project uses several Hugging Face pipelines for different tasks:

1. **Text Summarization**:
   - Model: `facebook/bart-large-cnn`
   - Used to generate concise summaries of English input text.
   
2. **Translation**:
   - Model: `Helsinki-NLP/opus-mt-en-ar`
   - Translates English summaries into Arabic.

3. **Text-to-Speech**:
   - Library: `gTTS` (Google Text-to-Speech)
   - Converts text into speech for both English and Arabic summaries.

4. **Audio Transcription**:
   - English Model: `openai/whisper-base`
   - Arabic Model: `jonatasgrosman/wav2vec2-large-xlsr-53-arabic`
   - These models convert uploaded audio files into text.

## Usage

1. **Text Summarization and Translation**:
   - Enter your text in the input box.
   - Select a language option: either English or English-to-Arabic.
   - Click on "Summarize" to get a summary of the input text and its corresponding audio.

2. **Audio Transcription**:
   - Upload an audio file in English or Arabic.
   - Select the language of the audio and click "Transcribe" to get the transcribed text.

### Example Usage:
1. Input Text: `"Machine learning models are becoming highly efficient in solving complex problems."`
2. Select Language: `"English to Arabic"`
3. Output:
   - **English Summary**: `"Machine learning models are very effective in solving complex problems."`
   - **Arabic Translation**: `"نماذج التعلم الآلي فعالة للغاية في حل المشكلات المعقدة."`
   - **Audio Files**: Downloadable links for both English and Arabic speech.

## Demo

You can view the live demo of this project on [Hugging Face Spaces](#).
- **Hugging Face Space**: [Link to Hugging Face Space](https://huggingface.co/spaces/Almahfouz/A_Tool_for_Text_Extraction_and_Reading)

## Future Work

Here are some ideas for extending the project:
- **Multilingual Support**: Add support for additional languages besides English and Arabic.
- **Enhanced Audio-to-Text**: Improve the transcription accuracy by experimenting with more advanced models.
- **Zero-Shot Image Classification**: Explore integrating image-based AI tasks such as zero-shot image classification using CLIP.
