# A Tool for Text Extraction and Reading

## Project Overview

This project demonstrates a bilingual AI tool using Hugging Face pipelines for **text summarization**, **translation**, and **text-to-speech conversion**. The project provides functionality in both **English** and **Arabic**. It aims to explore the capabilities of Hugging Face models in natural language processing (NLP), text-to-audio, and audio transcription tasks.

### Features:
- **Text Summarization**: Generate concise summaries of input text using state-of-the-art Hugging Face models.
- **Translation**: Translate summarized English text into Arabic.
- **Text-to-Speech**: Convert text (both English and Arabic) into speech using `gTTS`.
- **Audio Transcription**: Convert uploaded audio to text using the Whisper and Wav2Vec2 models.
  
## Models and Pipelines

This project leverages the following Hugging Face models for different tasks:

1. **Text Summarization**:
   - **Model**: [`facebook/bart-large-cnn`](https://huggingface.co/facebook/bart-large-cnn)
   - **Explanation**: BART is an encoder-decoder model pre-trained for various language tasks. It is highly efficient for abstractive text summarization and was chosen due to its effectiveness in summarizing long documents with coherence.
   
2. **Translation**:
   - **Model**: [`Helsinki-NLP/opus-mt-en-ar`](https://huggingface.co/Helsinki-NLP/opus-mt-en-ar)
   - **Explanation**: This model is part of the OPUS-MT project, specifically trained for translation tasks between English and Arabic. It was chosen due to its high accuracy in generating grammatically correct translations between these two languages.

3. **Text-to-Speech**:
   - **Library**: `gTTS` (Google Text-to-Speech)
   - **Explanation**: gTTS was chosen due to its lightweight nature and multi-language support, including both English and Arabic. It provides a simple yet effective way to convert text into speech.

4. **Audio Transcription**:
   - **English Model**: [`openai/whisper-base`](https://huggingface.co/openai/whisper-base)
   - **Arabic Model**: [`jonatasgrosman/wav2vec2-large-xlsr-53-arabic`](https://huggingface.co/jonatasgrosman/wav2vec2-large-xlsr-53-arabic)
   - **Explanation**: Whisper is one of the latest advancements in speech recognition, offering high accuracy in English transcription. For Arabic, Wav2Vec2 is a state-of-the-art model for Automatic Speech Recognition (ASR) and was selected for its proven performance in transcribing Arabic speech.

### Justification for Model and Pipeline Choices

- **Text Summarization (BART)**: BART was chosen due to its robustness and fine-tuning capabilities for long-document summarization. The `facebook/bart-large-cnn` model is specifically tuned for abstractive summarization, making it suitable for generating high-quality, coherent summaries in English.
  
- **Translation (Helsinki-NLP/opus-mt-en-ar)**: This model is highly effective for translating between English and Arabic, making it a natural choice for bilingual applications. It ensures that the translation quality remains high for a wide variety of inputs.

- **Text-to-Speech (gTTS)**: Google Text-to-Speech was selected for its ease of use and multi-language support. It converts text to speech in both English and Arabic efficiently, providing an intuitive way to listen to the summarized text.

- **Audio Transcription (Whisper and Wav2Vec2)**: Whisper provides superior accuracy in English transcription, especially for diverse accents. For Arabic, Wav2Vec2 is a cutting-edge model fine-tuned for Arabic speech recognition, offering excellent transcription accuracy.


## Sample Run

**Sample 1  Text (English-Arabic):**

![Screenshot 2024-10-01 152046](https://github.com/user-attachments/assets/293fe7ba-9c9a-4908-95b9-9be98e53a421)


**Sample 2 (Audio - Text)[Arabic]:**

![Screenshot 2024-10-01 152557](https://github.com/user-attachments/assets/c41eb4d2-084b-4d29-b35f-27d8ac488ee2)


## Demo

You can view the live demo of this project on [Hugging Face Spaces](#).
- **Hugging Face Space**: [Link to Hugging Face Space](https://huggingface.co/spaces/Almahfouz/A_Tool_for_Text_Extraction_and_Reading)

## Presentation

[`Google Slides`](https://docs.google.com/presentation/d/1csnTqCqBjsmVmruqe7W-cSrLqkad8YsOxaVWsxYRYzQ/edit#slide=id.g3071364de31_1_24)


## Video

[`Video`](https://drive.google.com/file/d/1Vcti0m8QMUHWnQohQK_BXql4z0uy7GIo/view?usp=sharing)
